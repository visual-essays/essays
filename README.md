.ve-header "Juncture" wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg options=pct:3,23,80,20 position=center sticky=true
    - [Home](/)
    - [About](/about)

# visual-essays.net

[visual-essays.net](https://visual-essays.net) is  home to a suite of tools and services used to create and display visual essays.  A __visual essay__ is a  web page that combines text content with interactive visualizations.  Visual essays are defined using Markdown text augmented with a simple set of custom tags for adding visualizations and creating user interactions.

The visual-essays.net tools were inspired by the [Juncture](https://juncture-digital.org) tools developed by the [JSTOR Labs team](https://labs.jstor.org).  visual-essays.net builds on the concepts represented in Juncture, providing improvements in essay authoring and the use of [IIIF (International Image Interoperability Framework)](https://iiif.io) images.  visual-essays.net provides an environment for evolving and improving the Juncture concepts without the restriction to provide backwards compatibility.  It is expected that many of the improvements developed for visual-essays.net will eventually be incorporated into a next-generation version of Juncture.

IIIF (pronounced “Triple-Eye-Eff”) is a set of open standards for delivering high-quality, attributed digital objects online at scale. The IIIF specifications are designed to support uniform and rich access to resources hosted around the world. IIIF supports rich zoom & pan delivery of high-resolution images, with options for size, scale, region of interest, rotation, quality and format.

IIIF offers many benefits for use in visual essays beyond the ability to just zoom & pan high-resolution images.  For visual essays the IIIF support for attribution and annotation are especially useful.

While offering many benefits, finding, creating, and using IIIF images can be daunting.  That's where the visual-essays.net tools come in.  They are designed to make this as easy as possible.  In many cases as easy as dragging an image from a file hosting site into the visual essays editor.  Behind the scenes the visual-essays.net software performs the work needed to turn a simple image into an IIIF resource providing rich user interaction (zoom, pan, cropping, etc), reuse rights assertions, image attribution, and a support for features like multi-image comparison and annotation.

In addition to rich IIIF support, future versions visual-essays.net will also include easy-to-use visualizations for maps, similar to that currently provided by [Juncture](https://juncture-digital.org).

## Example

.ve-image wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg sticky

Visual essays are plain text files with a few simple tags for text formatting and adding visualizations and defining user interactions.  The essay file is transformed into a web page by a back end service.  All pages on the visual-essays.net site are constructed using this approach and are thus visual essays.

To illustrate the use of a tag to add a IIIF image viewer, the following tag is included in the source text for this page.  This tag references [this image hosted by Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg) (note that this is the same image that is cropped for use in the page heading above).

```html
.ve-image wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg
```

This represents the simplest (and most common) use of the `ve-image` tag.  In this case the tag is followed by a reference to an IIIF manifest for an image to be displayed.

The IIIF reference can be provided as a full URL or in a short form version (as in the example here) when the source image is hosted on a site for which visual-essays.net is able to perform automatic manifest generation (as is the case with Wikimedia Commons).  The short form version of the IIIF manifest reference in the tag used in this example is equivalent to [https://iiif.visual-essays.net/wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg/manifest.json](https://iiif.visual-essays.net/wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg/manifest.json)

The IIIF image viewer displayed to right provides full image zoom and pan.  This can be accomplished with mouse interactions (or touch interactions on tablets and smartphones) or by using the control icons available in the top right corner of the image.  The icons are hidden by default and are shown when the mouse pointer is positioned over the image.  In addition to zoom and pan within the embedded viewer, the viewer can also be expanded to full screen by selecting the `Toggle full page` icon in the controls bar.

Selecting the menu icon (three vertical dots), located in the left portion of the caption bar at the bottom of the image, will open an image information panel where additional information about the image is displayed.  This includes reuse rights and any attribution statements associated with the image.

This example also illustrates the use of a simple user interaction.  The interaction causes the viewer to zoom to a region of the image when a ==marked section of text=={1608,1902,1550,1941} is clicked.  Text is "marked" by wapping the text with `==` strings.  The marked text can then be associated with an interaction that is performed on the closest viewer, in this case the viewer displaying the Van Gogh self-portrait image.  The default interaction is to zoom to a specific region of the image.  The region is defined by bounding box coordinates provided in an attributes tag following the marked text.  Attributes are defined by wrapping text with `{` and `}` characters.  The snippet below shows the use of marked text and an attribute tag to create the `zoom to` interaction used in this example.

```
...image when a ==marked section of text=={1608,1902,1550,1941} is clicked...
```

At this point the question would naturally be - "how do I get the `zoom to` bounding box coordinates?".  This is easily accomplished by positioning the image in the desired location in the viewer and then. hovering over the bottom right corner of the caption bar.  When hovering over this section the bounding box coordinates are displayed and can be copied by clicking on them.  After clicking on the the coordinates they can be pasted into the attributes tag.

## Essay Editor

An [online editor](https://editor.visual-essays.net) is available for writing and previewing visual essays. The editor supports drag-and-drop creation of image viewer tags from IIIF manifests.  IIII image manifests are available from a number of sites and can also be automatically generated for some popular image hosting sites.

### Authorization and Access

All visual essays are public and visible to anyone with a link.  Creating an essay using the visual-essays.net authoring tools requires user login.  This can be accomplished via an existing Google account or creating a simple login identity with visual-essays.net with an email address and password.

### Essay file storage

Essay files are simple text files that are stored in Google Cloud.  

## IIIF Tools

All images used in visual essays are rendered as IIIF images.  The use of IIIF provides deep zooming and panning of high resolution images and image manipulation features like cropping, rotating, and mirroring.  The IIIF viewer used by visual-essays.net also provides viewing options for comparing 2 or 3 images in side-by side or stacked image modes.  Image annotations can also be created and incorporated into an essay.

### Manifest Generator and Server

The visual-essays.net IIIF server 

### Automatic IIIF Manifest generation

visual-essays.net is able to automatically generate IIIF Presentation manifests for some popular image hosting sites.  In generating the manifest the highest resolution version of the image offered is used and relevant image metadata is obtained from APIs provided by the site.  For those interested in the details, these are single images manifests that are compliant with the IIIF Presentation 3.0 standard.

The visual-essays.net tool caches the manifest and image tiles for performance but does not retain a copy of the original image or metadata.  Manifests and image tiles are removed from the cache if not used within 30 days.  

visual-essays.net is currently able to automatically generate IIIF manifests for the following sites.
- [Wikimedia Commons](https://commons.wikimedia.org/wiki/Main_Page)
- [Flickr](https://www.flickr.com/explore)
- [JSTOR Community Collections](https://about.jstor.org/whats-in-jstor/open-community-collections/)
- [Openverse](https://wordpress.org/openverse/)
- [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page)
- [The Metropolitan Museum of Art](https://www.metmuseum.org/art/collection/search)

In addition to the sites listed above, visual-essays.net is also able to automatically generate IIIF manifests for Self-hosted Image Collections in Github.  More information about this can be found [here]().

### Image Server

- Standard
- Performant

### Image Annotator

Image Annotations

### Github Image Collections

## API

### Markdown to HTML Conversion

Wikidata entity tagging
