# Operating Instructions

## Images

Images

This is the full syntax for the wiki image mark up:

{{image\|alt text\|align\|max size}}

* image can be a URL to an image, or the name of an image assigned to the current page or a defined library page
* alt text is an optional, but strongly recommended, description of the image for accessibility uses when images are not displayed. For images assigned to the page, this will default to the text specified in the image definition if omitted.
* align is an option parameter used to force left, right or center alignment of the image
* max size is an option parameter specifying the maximum pixel dimension for the image. 

  For example, if a max size of 150 is specified the maximum possible displayed size would be 150x150 pixels, and the image will be scaled respecting the aspect ratio to fit completely within this size.

For images assigned to the page \(or a defined image library page\) the image name can be prefixed with "thumb:" to force display of a thumbnail that links to the full image. If max size is not specified, the Default Thumbnail Size from module preferences will be used.

If a page or library page image is specified with a max size, a resized version will be created or updated as needed, and served from a cached copy if possible.

If the image is specified as a URL, the prefix "siteurl:" will be replaced with the URL for the site.

```markup
{{siteurl:/modules/gwiki/images/icon.png|Module Icon|center}}
```

![](.gitbook/assets/logomodule%20%281%29.png)

Module Icon

## Image Editor

While editing a page, you can invoke the Image Editor using the image editor icon ![](.gitbook/assets/imageicon.png)

The Image Editor allows an author to add images to the page being edited, so it can be accessed only within the page editor. Each page has its own virtual space in which to hold its images. Normally an image is entirely private to the single page to which it is connected. The administrator can designate special library pages that can share their images with the entire wiki. The Image Editor is divided into three areas, the Image Library, the Image Detail and the Image Insertion Tool.

**Images**

* Library - Use this control to choose the source of the images shown in the editor, either the current page, or a special library page.
* List of Images - Any images available in the selected library are shown here. Select an image to display it in the Image Detail area for editing.

**Image Detail**

* Choose File or \(Drop File Here\) - select an image file to upload
* Name - Name to use for this image. This is how this image will be specified in the image directive.
* Alt Text - Alternate text for this image
* Use this image to represent the page - Display this image when this page is used in recent and page display blocks.
* Start New Image - clean all image data to start a new image
* Delete Image - delete the current image.

**Image Insertion Tool**

This tool can be used to build the wiki markup needed to display the current image in the page being edited.

* Align - align image left, right, center or no alignment
* Max Size in Pixels - specifies the maximum pixel dimension for the image, leave blank for no reduction.
* ![](.gitbook/assets/insimgicon.png)  Insert the wiki markup for the image and options selected into the page being edited, and close the image editor.

**Gallery**

{gallery}

This directive will display a thumbnail gallery of all of the images defined to the current page.

