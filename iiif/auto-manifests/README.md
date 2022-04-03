.ve-header "Visual Essays" "Auto-generated IIIF Manifests" sticky=true
    - img: wc:Zelfportret_met_strohoed_-_s0164V1962_-_Van_Gogh_Museum.jpg pct:0,25,80,20 center
    - nav:
        - [Home](/)
        - [About](/about)

# Examples

[IIIF Presentation API 3.0](https://iiif.io/api/presentation/3.0/)

# Rights

Each IIIF manifest must include a `rights` property that identifies a license or rights statement that applies to the image. The value must be drawn from the set of [Creative Commons](https://creativecommons.org/licenses/) license URIs or [RightsStatements.org](https://rightsstatements.org/page/1.0/) rights statement URIs.  A summary list of the recognized rights codes and associated URIs can be seen **[here](rights)**.

## Using a file naming convention

The easiest method for defining the rights for an image hosted in Github is to append a Creative Commons or Rights Statements code to the end (but before the file extension) of the Gihub file name.  The naming convention recognized by the Visual Essays IIIF manifest generator splits the file name into two segments.  The segments are separated by the first `-` in the file name.  The first segment is the image label (or caption) and the second is the rights code.  The rights code is one of the Creative Commons or RightsStatements.org codes defined in the section above.

## Using IIIF property files

An alternative to adding the rights code to the file name is to associate a property file with an image.  The properties file approach provides a mechanism for defining a wide range of properties for an image.  A properties file can be associated with a single image or all images contained in a folder hierarchy.

### Associating IIIF properties with a single image

IIIF properties can be associated with a single image by creating a `.yaml` file with the same root file name as the image but with the `.yaml` extension instead of the image extension (typically `.jpg` or `.png`).  For instance, to associate a properties file with the image named `Fiordo_de_Furore.jpg` the file `Fiordo_de_Furore.yaml` would be created in the same directory.

### Associating IIIF properties with multiple images

Properties can be associated with multiple files by grouping the files in a folder and adding a `iiif-props.yaml` file in the same folder.  Property files can be defined at any level in a folder hierarchy.  Properties defined at a lower-level in the hierarchy override the same properties defined in a higher-level folder.  This technique can be convenient for defining default values, such as might be done for the `provider`, `rights` and `requiredStatement` properties that would be the same for a group of images.

# Image metadata file format

Property files for single images or groups of images in a folder follow the structure defined for the [IIIF Presentation API v3.0](https://iiif.io/api/presentation/3.0/#42-resource-representations).  A template for defining IIIF properties in an `iiif-props.yaml` file can be seen at [iiif-props.template.yaml](https://raw.githubusercontent.com/rdsnyder/examples/main/iiif-props.template.yaml).

# Using a metadata file for external files

In addition to defining metadata for files hosted in Github, metadata files may also be used to associate metadata (for manifest generation) with files hosted on other sites.  An example of this can be seen with the [Westgate_today.yaml](https://github.com/rdsnyder/examples/blob/main/images/kent-maps/Westgate_today.yaml) file.

- https://iiif.visual-essays.net/gh:rdsnyder/examples/images/kent-maps/Westgate_today

# Examples

# Defining rights using the file naming convention

## Open Access Images with Public Domain Dedication (Creative Commos CC0)

- https://iiif.visual-essays.net/gh:rdsnyder/examples/images/Italy_2022/Riomaggiore_sunset-CC0.jpg
- https://iiif.visual-essays.net/gh:rdsnyder/examples/images/Italy_2022/Vernazza-CC0.png

## Open Access Images with Attribution Requirement (Creative Commos CC BY)

- https://iiif.visual-essays.net/gh:rdsnyder/examples/images/Italy_2022/Positano-CC-BY.jpg
