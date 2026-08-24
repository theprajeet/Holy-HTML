# Media Tags

## Video and Audio Tags

### **The `<video>` Tag**

The **`<video>`** tag is used to embed video files in an HTML document. It supports multiple attributes to control the video playback.

Example usage:

`<video src="video.mp4" controls></video>`

#### **Attributes for `<video>` Tag**

- **src**: Specifies the path to the video file.
- **controls**: Adds video controls, like play, pause, and volume.
- **autoplay**: Automatically starts playing the video when the page loads.
- **loop**: Repeats the video once it ends.
- **muted**: Mutes the video by default.
- **poster**: Specifies an image to be displayed before the video starts playing.
- **width** and **height**: Specifies the dimensions of the video.

---

### **The `<audio>` Tag**

The **`<audio>`** tag is used to embed audio files in an HTML document. It also supports multiple attributes for control.

Example usage:

`<audio src="audio.mp3" controls></audio>`

#### **Attributes for `<audio>` Tag**

- **src**: Specifies the path to the audio file.
- **controls**: Adds audio controls, like play, pause, and volume.
- **autoplay**: Automatically starts playing the audio when the page loads.
- **loop**: Repeats the audio once it ends.
- **muted**: Mutes the audio by default.
- **preload**: Specifies if and how the audio should be loaded when the page loads ('auto', 'metadata', 'none').

The "preload" attribute can have the following values:

1. **none**: This is the default value. It indicates that the browser should not preload the audio file at all. The audio file will only start downloading when the user initiates playback.
2. **metadata**: This value tells the browser to preload only the metadata of the audio file, such as its duration and basic information about the audio. This can be useful if you want to display the audio duration to the user without fully loading the audio data.
3. **auto**: This value instructs the browser to preload the entire audio file as much as possible without delaying the loading of other important page content. The browser will try to load the audio file in the background so that it's ready to play when the user decides to start it.

---

## SVGs

SVG stands for Scalable Vector Graphics. Unlike raster images like PNGs or JPGs, SVGs are not pixel-based. They're composed of vectors—mathematical formulas that describe shapes, paths, and fills. This means SVGs can be resized without losing quality.

#### **Why Use SVG?**

- SVG images can be scaled indefinitely without losing quality, which is ideal for responsive web design.
- SVG files are often smaller than their raster counterparts, especially for simple shapes and icons.
- SVGs can be styled, animated, and manipulated using CSS and JavaScript.

#### **How to Embed SVG in HTML**

SVG can be embedded in HTML in several ways:

1. Inline SVG: Directly writing the SVG XML code within HTML.
2. Using an **`<img>`** tag: Point the src attribute to an SVG file.
3. Using CSS: Setting SVG as a background image in a CSS file.

#### **Example**

```html
<svg height="100" width="100">
    <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red" />
</svg>

<svg height="30" width="30">
    <rect width="30" height="30" style="fill:rgb(0,0,255);stroke-width:1;stroke:rgb(0,0,0)" />
</svg>

<img src="image.svg" alt="Sample SVG">

```

#### **SVG Attributes**

SVG comes with a set of attributes to control its behaviour:

- **`width`** and **`height`**: To set the dimensions.
- **`viewBox`**: To set the coordinate system.
- **`fill`** and **`stroke`**: To set the colors.

---

## iFrames in HTML

An iFrame is an HTML element that enables an inline frame for the embedding of external content. Essentially, you can load another web page within a designated area of your current webpage.

iFrames offer a variety of use-cases:

- **Content Isolation**: iFrames allow you to isolate third-party content, which can improve security.
- **Modularity**: Easily embed external plugins, widgets, or content.
- **Resource Separation**: Content within an iFrame can load separately from the rest of the page.

#### **Basic Syntax**

The basic syntax of an iFrame is quite straightforward:

```html
<iframe src="URL" width="width" height="height"></iframe>
```

#### **Attributes of iFrame**

Several attributes can enhance the functionality of an iFrame:

- **src**: Specifies the URL of the page to embed.
- **height** and **width**: Define the dimensions.
- **frameborder**: Indicates whether to display a border.
- **scrolling**: Controls the scrollbars.
- **name**: For targeting the iFrame in JavaScript.

#### **Examples**

**Embedding a YouTube Video**

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/dQw4w9WgXcQ?si=EPT0xcQdydphvMhB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
```

**Embedding Google Maps**

```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d497632.1325127385!2d77.29231040230371!3d12.987769307571995!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3bae1670c9b44e6d%3A0xf8dfc3e8517e4fe0!2sBengaluru%2C%20Karnataka!5e0!3m2!1sen!2sin!4v1787604448085!5m2!1sen!2sin" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="strict-origin-when-cross-origin"></iframe>
```

---