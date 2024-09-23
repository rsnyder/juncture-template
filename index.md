# juncture

## Markdown

## Juncture tagging

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

The [animated-image](https://docs.juncture-digital.org/components/animated-image-viewer) tag creates a viewer that is able to play animated GIFs.

`animated-image https://upload.wikimedia.org/wikipedia/commons/e/e3/Animhorse.gif left`

### Audio Player

The [audio](https://docs.juncture-digital.org/components/audio-player) tag creates a viewer that is able to play audio content.

`audio wc:Interview_with_Warren_Hanson_regarding_Hundred_Flowers.ogg caption="Interview with Warren Hanson regarding Hundred Flowers" left`

### Image Carousel

The [carousel](https://docs.juncture-digital.org/components/image-carousel) displays an arbitrary number of images along a horizontal or vertical axis.  The carousel is a Juncture wrapper for the [Shoelace](https://shoelace.style/) [sl-carousel](https://shoelace.style/components/carousel) component.

```
carousel navigation left fit=cover
- wc:Atrani_(Costiera_Amalfitana,_23-8-2011).jpg
- wc:Amalfi_Coast_Italy_6.JPG
- wc:Costiera-amalfitana-_panorama_from_the_sea_129.jpg
- wc:Amalfi_Coast_(247891371).jpeg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_73_(50557616528).jpg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_72_(50558479917).jpg
- wc:Amalfi_Coast_(Italy,_October_2020)_-_14_(50558382446).jpg
```

### IFrame Viewer

The [iframe](https://docs.juncture-digital.org/components/iframe-viewer) tag allows arbitrary web pages to be embedded in an essay. The Juncture iframe viewer is a light wrapper around the standard HTML iframe that is used to embed another document within the current HTML document.

`iframe https://archive.org/embed/slaveryinunit00ballcha/page/172/mode/1up left`

### Image Compare Viewer

The [image-compare](https://docs.juncture-digital.org/components/image-compare-viewer) creates a viewer that is able to display 2 high-resolution in a stacked compare viewer.

```
compare caption="Comparison of Van Gogh Sketch and Painting"
wc:Vincent_van_Gogh_-_Vincent's_Bedroom_in_Arles_-_Letter_Sketch_October_1888.jpg
wc:Vincent_van_Gogh’s_famous_painting,_digitally_enhanced_by_rawpixel-com_49.jpg
```

### Image Gallery

The [gallery](https://docs.juncture-digital.org/components/image-gallery) displays an arbitrary number of image thumbnails in a grid. By default only the thumbnail is displayed. An image caption cah be shown using the show-caption boolean attribute. When the thumbnail is clicked, the full image is shown in a popup window.

```
gallery
wc:Atrani_(Costiera_Amalfitana,_23-8-2011).jpg
wc:Costiera-amalfitana-_panorama_from_the_sea_129.jpg
wc:Amalfi_Coast_(247891371).jpeg
wc:Amalfi_Coast_(Italy,_October_2020)_-_73_(50557616528).jpg
wc:Amalfi_Coast_(Italy,_October_2020)_-_72_(50558479917).jpg
wc:Amalfi_Coast_(Italy,_October_2020)_-_14_(50558382446).jpg
```

### Image Viewer

The [image viewer](https://docs.juncture-digital.org/components/image-viewer) will render a high-resolution image with full interactivity (deep-zoom and panning) enabled.

`image wc:Sunflower_sky_backdrop.jpg left`

### Map Viewer

The [map viewer](https://docs.juncture-digital.org/components/map-viewer) creates a map viewer that displays a base map with optional map layers. The map viewer supports zooming and panning. 

`map left`

### Mermaid Diagram Viewer

Lorem ipsum odor amet, consectetuer adipiscing elit. Aenean pulvinar proin consequat neque eleifend pharetra facilisis litora. Ornare magnis cubilia cras aenean torquent lacinia curabitur. Quisque porttitor tristique donec senectus ridiculus nascetur. Tempor luctus tristique cras posuere lectus. Amet conubia aptent; eu vivamus sapien posuere sodales velit netus. Etiam sem phasellus netus vulputate dui lacinia felis. Finibus donec porta eleifend porta imperdiet faucibus condimentum. Felis malesuada phasellus porttitor habitasse facilisi rhoncus urna.

More information can be found [here](https://docs.juncture-digital.org/components/mermaid-diagram-viewer).

### Plant Specimen Viewer

Lorem ipsum odor amet, consectetuer adipiscing elit. Aenean pulvinar proin consequat neque eleifend pharetra facilisis litora. Ornare magnis cubilia cras aenean torquent lacinia curabitur. Quisque porttitor tristique donec senectus ridiculus nascetur. Tempor luctus tristique cras posuere lectus. Amet conubia aptent; eu vivamus sapien posuere sodales velit netus. Etiam sem phasellus netus vulputate dui lacinia felis. Finibus donec porta eleifend porta imperdiet faucibus condimentum. Felis malesuada phasellus porttitor habitasse facilisi rhoncus urna.

More information can be found [here](https://docs.juncture-digital.org/components/plant-specimen-viewer).

### Video Player

Lorem ipsum odor amet, consectetuer adipiscing elit. Aenean pulvinar proin consequat neque eleifend pharetra facilisis litora. Ornare magnis cubilia cras aenean torquent lacinia curabitur. Quisque porttitor tristique donec senectus ridiculus nascetur. Tempor luctus tristique cras posuere lectus. Amet conubia aptent; eu vivamus sapien posuere sodales velit netus. Etiam sem phasellus netus vulputate dui lacinia felis. Finibus donec porta eleifend porta imperdiet faucibus condimentum. Felis malesuada phasellus porttitor habitasse facilisi rhoncus urna.

More information can be found [here](https://docs.juncture-digital.org/components/video-player).

### VisJS Diagram Viewer

Lorem ipsum odor amet, consectetuer adipiscing elit. Aenean pulvinar proin consequat neque eleifend pharetra facilisis litora. Ornare magnis cubilia cras aenean torquent lacinia curabitur. Quisque porttitor tristique donec senectus ridiculus nascetur. Tempor luctus tristique cras posuere lectus. Amet conubia aptent; eu vivamus sapien posuere sodales velit netus. Etiam sem phasellus netus vulputate dui lacinia felis. Finibus donec porta eleifend porta imperdiet faucibus condimentum. Felis malesuada phasellus porttitor habitasse facilisi rhoncus urna.

More information can be found [here](https://docs.juncture-digital.org/components/visjs-diagram-viewer).
