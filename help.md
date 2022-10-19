.ve-meta title="Juncture Documentation"

.ve-header "Juncture Documentation" background=#5B152E logo=https://raw.githubusercontent.com/visual-essays/media/main/images/Juncture_Logo.png
   
# Visual Essays Help

### Quick links

**Viewer Tags**

  - [.ve-header](#ve-header)
  - [.ve-image](#ve-image)
  - [.ve-image-grid](#ve-image-grid)
  - [.ve-meta](#ve-meta)
  - [.ve-style](#ve-style)

**Howto's**

- [Marking text for interactions](#marking-text)
- [Creating a **zoom to** interaction](#zoom-to)

# Viewer Tags
Custom tags are added to essay text to define viewers that are inserted into the generated page.  Each viewer tag includes a **.ve-** prefix and must appear at the beginning of a new line.  Viewer tags accept one or more positional and/or key-value arguments.  A positional argument is simply a text string that follows the tag.  Some viewers can accept multiple positional arguments, in which case the ordering is important.   Key-value arguments take the form of `<KEY>=<VALUE>`, explicitly defining the attribute name and value.  Key-value arguments must follow any positional arguments used.  For both positional and key-value arguments a value with a space must be enclosed in quotes.  

## .ve-header {#ve-header .no-offset}

The `.ve-header` tag is used to define an optional header that appears at the start of the essay.  The header can be used to:

- Define a title and subtitle for the essay
- Display a banner image
- Create a navigation menu for linking to sections within the current essay, to other essays, or to arbitrary web pages

As with the images displayed by the `.ve-image` tag, the banner image used by the `.ve-header` tag is a IIIF image and can be cropped or otherwise manipulated when displayed in the header.

### .ve-header Attributes

- **label**:  The text to use for the essay title. 
- **subtitle**:  The text to use for the essay subtitle.
- **height**:  The height of the header (before collapsing when in `sticky` mode).  The default value is `300` pixels.
- **background**:  The URL to the IIIF manifest for the image to display as a banner image in the header. 
- **options**:  The `options` attribute is used to define the [IIIF image request parameters](https://iiif.io/api/image/2.1/#image-request-parameters) for an image.  This attribute is most commonly used to define a coordinates for displaying an image region.   
- **position**:  The portion of a cropped banner image to display.  The default is `center`.  Other recognized values are `top` and `bottom`.
- **sticky**:  If set to `true` the header will collapse into a condensed form and remain fixed at the top of the page.

**Positional attributes**:  `label background subtitle options position sticky`

### Examples

- A sticky header defined with positional attributes and navigation menu options in a nested Markdown list.
```Markdown
.ve-header "My Essay Title" wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg "A Subtitle" pct:3,23,80,20 center true
    - [Home](/)
    - [About](/about)
```

## .ve-image {#ve-image .no-offset}

The `.ve-image` tag is the most commonly used essay tag.  The tag creates an IIIF image viewer that is able to display one or more images.

### .ve-image Attributes

- **src**:  The URL to the IIIF manifest for the image to display in the viewer.  This attribute can be omitted when multiple using the viewer in multi-image mode.  
- **seq**:  A number defining the image to use in a multi-image manifest.  If not specified the dafault value is `1`.
- **id**:  An optional.
- **options**:  The `options` attribute is used to define the [IIIF image request parameters](https://iiif.io/api/image/2.1/#image-request-parameters) for an image.  This attribute is most commonly used to define a coordinates for displaying an image region.    
- **fit**:  The `fit` attribute controls the display of an image in the viewer viewport.  In the default mode (`contain`) the entire image is show with letter-boxing applied to the top and bottom or left and right when the image aspect ratio differs from the viewers.  When the value `cover` is used the entire viewport is filled and the image display is cropped as needed to fit.
- **compare**:  The `compare` attribute is used in multi-image mode to compare 2 or 3 images.  The compare attribute accepts two possible values, `curtain` and `sync`, defining the comparison mode used.  In `curtain` mode the images are stacked on top of each other and cursor movements over the image will reveal or hide relevant sections of each image in the stack.  In `sync` mode the images to compare are displayed side-by-side with zoom and panning actions applied to each simultaneously.
- **alt**:  The text to use in the `alt` tag used by screen readers.  If not provided an `alt` tag is automatically generated from the manifest label property.

**Positional attributes**:  `src options seq fit`

### Multiple images mode

To use more than one image with a `.ve-image` viewer the Markdown nested list notation is used.  A Markdown list is defined by prefixing the `    - ` text to each list element on separate lines.   Each list element can include positional and/or key-value attributes for the associated image.

### Manifest URLs

The manifest URL is a URL to an IIIF presentation manifest that is compliant to version 2.x or version 3.0 of the IIIF Presentation Standard.

When referring to a manifest automatically generated by visual-essays.net a short-form version of the auto-generated URL may be used.  The short-form version takes the form of `<SOURCE>:<SOURCE_ID>`, where `<SOURCE>` is the a site code for one of the image hosting sites supporting manifest generation by visual-essays.net.  The `<SOURCE_ID>` value is a unique resource ID applicable to the site.  For example, visual-essays.net is able to automatically generate IIIF manifests for images hosted on [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page).  A full auto-generated manifest for the image at [https://commons.wikimedia.org/wiki/File:Sunflower.jpg](https://commons.wikimedia.org/wiki/File:Sunflower.jpg){target=_blank} would be [https://iiif.visual-essays.net/wc:Sunflow.jpg/manifest.json](https://iiif.visual-essays.net/wc:Sunflow.jpg/manifest.json).  The short form version of this URL (**wc:Sunflower.jpg**) can be used with any visual-essay.net tag (.ve-image, .ve-header, .ve-image-grid, and others) that accept IIIF manifest attributes.

### Examples

Using a Wikimedia Commons image using the short-form version of the manifest URL and an `alt` attribute.
```Markdown
.ve-image wc:Sunflower.jpg alt="Sunflowers in a field"
```

Using a JSTOR Community Collections image using the short-form version of the manifest URL and `options` as positional attributes.
```Markdown
.ve-image jstor:community.24604882 pct:35,42,10,25
```

Above example using key-value attributes rather than positional.
```Markdown
.ve-image src=jstor:community.24604882 options=pct:35,42,10,25
```

Using a full manifest URL.
```Markdown
.ve-image https://iiif.harvardartmuseums.org/manifests/object/299843
```

Using multiple images:
```Markdown
.ve-image
    - wc:Sunflower.jpg
    - jstor:community.24604882
```

## .ve-image-grid {#ve-image-grid .no-offset}

TODO

## .ve-meta {#ve-meta .no-offset}

The `.ve-meta` tag is used to define metadata attributes for the page.  Defining `.ve-meta` tag in an essay enables the rendered to be indexed by search engines.  When the tag is not found in an essay a `noindex` tag is added to the generated page by default.

### .ve-meta Attributes

- **title**:  A short title for the page.  This title will be added to the browser window or tab.  When indexed by search engines this title will also appear in the search results item.   
- **description**:  A short description of the page.  When indexed by search engines this description will appear in the search results item. 

###  Example

```Markdown
.ve-meta title="The Page Title" description="A brief description of the page.  This will appear in Google search results."
```

## .ve-style {#ve-style .no-offset}

The `.ve-style` tag is used to replace the default stylesheet with a custom one loaded from the URL defined in the tags `href` attribute.

###  Example

```Markdown
.ve-style href=https://www.example.com/my/custom/stylesheet.css
```
# How To's

## Marking Text {#marking-text .no-offset}

Essay text is "marked" by surrounding the applicable text with double equal signs (`==`) followed by an element attributes definition with the action to be performed.  Element attributes are defined by text enclosed with `{` and `}` characters.  For example:

```Markdown
Lorem ipsum ==dolor=={100,100,400,400} sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam
```

In the example above the text `dolor` is marked and associated with the attribute `100,100,400,400`.  This has the effect of highlighting the `dolor` text in the rendered essay and creating a `zoom to` interaction when the text is selected (clicked or tapped).  The `zoom to` interaction causes the closest image zoom to the region specified by the coordinates in the  attribute.  More information about the `zoom to` interaction, including how to define the coordinates, is provided below.

## Zoom To {#zoom-to .no-offset}

TODO