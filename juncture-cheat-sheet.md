<style>
  .section3 ul strong { color: red; }
</style>

# Juncture Cheat Sheat

## Juncture tagging

Juncture extends the Markdown language with tags for adding viewer components to the generated web page.

## Juncture components

- [Animated Image Viewer](#animated-image-viewer)
- [Audio Player](#audio-player)
- [Image Carousel](#image-carousel)
- [IFrame Viewer](#iframe-viewer)
- [Image Compare Viewer](#image-compare-viewer)
- [Image Gallery](#image-gallery)
- [Image Viewer](#image-viewer)
- [Map Viewer](#map-viewer)
- [Mermaid Diagram Viewer](#mermaid-diagram-viewer)
- [Plant Specimen Viewer](#plant-specimen-viewer)
- [Video Player](#video-player)
- [VisJS Diagram Viewer](#visjs-diagram-viewer)

### Animated Image Viewer 

The `animated-image` tag creates a viewer that is able to play animated GIFs.

####
`.mcol`

#####

**Tag Attributes**

- **src** (_string_): The URL to the animated GIF image.  Wikimedia Commons short form URLs are supported.
- **caption** (_string_): Defines the text to use for a caption that is displayed below the image.
- **autoplay** (_boolean_): Automatically play animation when viewer is displayed.

#####

**Examples**

<ve-snippet collapsible label="Click to view basic example">
`animated-image https://upload.wikimedia.org/wikipedia/commons/e/e3/Animhorse.gif`
</ve-snippet>

For more examples visit the [animated-image documentation page](https://docs.juncture-digital.org/components/animated-image-viewer).

### Audio Player

The `audio` tag creates a viewer that is able to play audio content.

####
`.mcol`

#####

**Tag Attributes**

- **src** (_string_): The URL to the animated GIF image.  Wikimedia Commons short form URLs are supported.
- **caption** (_string_): Defines the text to use for a caption that is displayed below the image.
- **autoplay** (_boolean_): Automatically play animation when viewer is displayed.
- **start** (_number_): Time position to start playing audio clip.
- **end** (_number_): Time position to stop playing audio clip.
- **muted** (_boolean_): Mute audio when initially played.
- **sync** (_boolean_): Synchronize playback with timestamps in text headline.

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
`audio wc:Interview_with_Warren_Hanson_regarding_Hundred_Flowers.ogg caption="Interview with Warren Hanson regarding Hundred Flowers"`
 </ve-snippet>
 
For more examples visit the [audio documentation page](https://docs.juncture-digital.org/components/audio-player).

### Image Carousel

The `carousel` tag displays an arbitrary number of images along a horizontal or vertical axis.  The carousel is a Juncture wrapper for the [Shoelace](https://shoelace.style/) [sl-carousel](https://shoelace.style/components/carousel) component.

####
`.mcol`

#####

**Tag Attributes**

- **aspect-ratio**: (_string_) :  Use the `aspect-ratio` attribute to customize the size of the carousel’s viewport from the default value of **16/9**.  Other values include **3/2** and **1/1**.
- **autoplay** (_boolean_) :  The carousel will automatically advance when the `autoplay` attribute is used. To change how long a slide is shown before advancing, set autoplay-interval to the desired number of milliseconds. For best results, use the loop attribute when autoplay is enabled. Note that autoplay will pause while the user interacts with the carousel.
- **caption** (_string_) :  A caption for the carousel viewer.  Image-specific captions are set in the image list.
- **fit** (_string_) :  The `fit` attribute is used to define how an image should be resized to fit its container.
	- *contain* (_default_) - The image keeps its aspect ratio, but is resized to fit within the available space.
	- *cover* - The image keeps its aspect ratio and fills the the available space. The image will be clipped to fit.
- **gallery** (_boolean_) :  The `gallery` attribute syncs the active slide with a set of thumbnails, creating a gallery-style carousel.
- **loop** (_boolean_) :  By default, the carousel will not advanced beyond the first and last slides. You can change this behavior and force the carousel to "wrap" with the `loop` attribute.
- **navigation** (_boolean_) :  Use the `navigation` attribute to show previous and next buttons.
- **orientation** (_string_) :  Setting the `orientation` attribute to **vertical** will render the carousel in a vertical layout. If the content of your slides vary in height, you will need to set amn explicit height or max-height on the carousel using CSS.
- **pagination** (_boolean_) :  Use the `pagination` attribute to show the total number of slides and the current slide as a set of interactive dots.
- **scroll-hint** (_boolean_) :  Use the `scroll-hint` attribute to add inline padding in horizontal carousels and block padding in vertical carousels. This will make the closest slides slightly visible, hinting that there are more items in the carousel.
- **slides-per-page** (_number_) :  The `slides-per-page` attribute makes it possible to display multiple slides at a time. You can also use the `slides-per-move` attribute to advance more than once slide at a time, if desired.
- **slides-per-move** (_number_) :  Generally used in conjunction with the `slides-per-page` attribute to advance more than one slide at a time.

**Images List**

A list of one or more images to be displayed in the carousel.  At a minimum, the `src` attribute must be defined for each image.  Other optional attributes may be defined as needed.

- **src** (_string_): The URL to the image IIIF manifest.  Wikimedia Commons and Github short form URLs are supported.
- **caption** (_string_) :  A caption for the image.
- **fit** (_string_) :  The `fit` attribute is used to define how an image should be resized to fit its container.
	- *contain* (_default_) - The image keeps its aspect ratio, but is resized to fit within the available space.
	- *cover* - The image keeps its aspect ratio and fills the the available space. The image will be clipped to fit.

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
```
carousel navigation fit=cover
- wc:Atrani_(Costiera_Amalfitana,_23-8-2011).jpg
- wc:Amalfi_Coast_Italy_6.JPG
- wc:Costiera-amalfitana-_panorama_from_the_sea_129.jpg
- wc:Amalfi_Coast_(247891371).jpeg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_73_(50557616528).jpg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_72_(50558479917).jpg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_14_(50558382446).jpg
```
</ve-snippet>

For more examples visit the [carousel documentation page](https://docs.juncture-digital.org/components/image-carousel).

### IFrame Viewer

The `iframe` tag allows arbitrary web pages to be embedded in an essay. The Juncture iframe viewer is a light wrapper around the standard HTML iframe that is used to embed another document within the current HTML document.

####
`.mcol`

#####

**Tag Attributes**

#####

**Examples**
 
<ve-snippet collapsible label="Click to view example">
`iframe https://archive.org/embed/slaveryinunit00ballcha/page/172/mode/1up`
</ve-snippet>

For more examples visit the [iframe documentation page](https://docs.juncture-digital.org/components/iframe-viewer).

### Image Compare Viewer

The `image-compare` tag creates a viewer that is able to display 2 high-resolution in a stacked compare viewer.

####
`.mcol`

#####

**Tag Attributes**

**Images List**

#####

**Examples**
 
<ve-snippet collapsible label="Click to view example">
```
compare caption="Comparison of Van Gogh Sketch and Painting"
wc:Vincent_van_Gogh_-_Vincent's_Bedroom_in_Arles_-_Letter_Sketch_October_1888.jpg
wc:Vincent_van_Gogh’s_famous_painting,_digitally_enhanced_by_rawpixel-com_49.jpg
```
</ve-snippet>

For more examples visit the [image-compare documentation page](https://docs.juncture-digital.org/components/image-compare-viewer).

### Image Gallery

The `gallery` tag displays an arbitrary number of image thumbnails in a grid. By default only the thumbnail is displayed. An image caption cah be shown using the show-caption boolean attribute. When the thumbnail is clicked, the full image is shown in a popup window.

####
`.mcol`

#####

**Tag Attributes**

- **src** (_string_): something about src
- **caption** (_string_): something about caption
- **fit** (_string_): something about fit
- **cover** (_boolean_): something about boolean

**Images List**

- **src** (_string_): something about src
- **caption** (_string_): something about caption
- **fit** (_string_): something about fit
- **cover** (_boolean_): something about boolean

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
`gallery`
- wc:Atrani_(Costiera_Amalfitana,_23-8-2011).jpg
- wc:Costiera-amalfitana-_panorama_from_the_sea_129.jpg
- wc:Amalfi_Coast_(247891371).jpeg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_73_(50557616528).jpg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_72_(50558479917).jpg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_14_(50558382446).jpg
</ve-snippet>

For more examples visit the [gallery documentation page](https://docs.juncture-digital.org/components/image-gallery).

### Image Viewer

The `image` tag will render a high-resolution image with full interactivity (deep-zoom and panning) enabled.

####
`.mcol`

#####

**Tag attributes**

- **src** (_string_, _positional_): something about src
- **caption** (_string_, _positional_): something about caption
- **fit** (_string_): something about fit
- **cover** (_boolean_): something about boolean

**Images List**

- *src*
- *caption*
- *cover*

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
`image wc:Sunflower_sky_backdrop.jpg`
</ve-snippet>

For more examples visit the [image documentation page](https://docs.juncture-digital.org/components/image-viewer).
  
### Map Viewer

The `map` tagcreates a map viewer that displays a base map with optional map layers. The map viewer supports zooming and panning. 

####
`.mcol`

#####

**Tag attributes**

**Layers List**

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
`map`
</ve-snippet>

For more examples visit the [map documentation page](https://docs.juncture-digital.org/components/map-viewer).

### Mermaid Diagram Viewer

The `mermaid` tag uses the [mermaid.js](https://mermaid.js.org/intro/) JavaScript library to create diagram visualizations. With this tag, you can create charts and diagrams with Markdown-inspired text definitions used by Mermaid. This page will show you the different diagram types supported by Mermaid that you can include in your visual essay.

####
`.mcol`

#####

**Tag attributes**

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
```
mermaid
mindmap
  root((mindmap))
    Origins
      Long history
      ::icon(fa fa-book)
      Popularisation
        British popular psychology author Tony Buzan
    Research
      On effectiveness<br/>and features
      On Automatic creation
        Uses
            Creative techniques
            Strategic planning
            Argument mapping
    Tools
      Pen and paper
      Mermaid
```
</ve-snippet>

For more examples visit the [mermaid documentation page](https://docs.juncture-digital.org/components/mermaid-diagram-viewer).

### Plant Specimen Viewer

The `plant-specimen` tag is used to display one or more plant specimens obtained from JSTOR Global Plants. The component is a wrapper for the .ve-media viewer which is used to display the high-resolution specimen images.

####
`.mcol`

#####

**Tag attributes**

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
`plant-specimen Q11575`
</ve-snippet>

For more examples visit the [plant-specimen documentation page](https://docs.juncture-digital.org/components/plant-specimen-viewer).

### Video Player

The `video` tag creates a viewer that is able to play video content, including streaming video from YouTube and Vimeo.

####
`.mcol`

#####

**Tag attributes**

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
`video Zy3K2Lcw7hQ`
</ve-snippet>

For more examples visit the [video documentation page](https://docs.juncture-digital.org/components/video-player).

### VisJS Diagram Viewer

The `visjs` tag uses the [vis.js](https://visjs.org/) JavaScript library to create diagram visualizations. With this tag, you can create network, timeline, and other types of diagrams.

####
`.mcol`

#####

**Tag attributes**

#####

**Examples**

<ve-snippet collapsible label="Click to view example">
|id |     label     |
|---|---------------|
| 1 | Node 1        |
| 2 | Node 2        |
| 3 | Node 3        |
| 4 | Node 4        |
| 5 | Node 5        |
`#nodes`

|from|to |
|----|---|
| 1 | 3  |
| 1 | 2  |
| 2 | 4  |
| 2 | 5  |
| 3 | 3  |
`#edges`
</ve-snippet>

For more examples visit the [visjs documentation page](https://docs.juncture-digital.org/components/visjs-diagram-viewer).
