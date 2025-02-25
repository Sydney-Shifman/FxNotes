# JavaFX Overview
([Source documentation](https://docs.oracle.com/javase/8/javafx/get-started-tutorial/jfx-overview.htm#JFXST784))
## Key Features

* Java ([API](#api)): designed in Java and is written to be a relatively friendly alternative to other Java-based frameworks like JRuby (in [Ruby](#ruby)) and Scala.
* FXML: is a ([XML](#xml))-based markup language used to construct JavaFX user interfaces. You can write in FXML code directly or use the SceneBuilder tool to design the GUI interactively. SceneBuilder generates FXML, which can be ported to an IDE where developers add the necessary logic.
    * SceneBuilder Guide
* WebView: a ([web component](#web-component)) that uses ([WebKitHTML](#webkithtml)) technology to embed web pages in JavaFX applications. JavaScript in WebView can call Java APIs, and Java APIs can call JavaScript running in WebView. JavaFX 8 added support for additional ([HTML5](#html5)) features such as ([Web Sockets](#web-sockets)), ([Web Workers](#web-workers)), ([Web Fonts](#web-fonts)), and printing capabilities.
    * Adding HTML Content to JavaFX Applications
* Swing interoperability: ([Swing applications](#swing-applications)) can be enhanced with JavaFX features like media playback and embedded web content. The ([SwingNode](#swingnode)) class allows embedding Swing content into JavaFX applications.
    * SwingNode API javadoc
    * Embedding Swing Content in JavaFX Applications
* Built-in ([UI controls](#ui-controls)) and ([CSS](#css)): JavaFX provides UI components that can be styled using standard Web technologies like CSS. JavaFX 8 introduced ([DatePicker](#datepicker)) and ([TreeTableView](#treetableview)). The ([CSS Styleable](#css-styleable)) classes have been made public, allowing objects to be styled dynamically.
    * Using JavaFX UI Controls
* Modena theme: JavaFX 8 introduced ([Modena](#modena)) as the default theme, replacing ([Caspian](#caspians)). Caspian is still available using `setUserAgentStylesheet(STYLESHEET_CASPIAN)`.
    * Can be accessed through Scene Builder.
    * Modena Blog
* 3D Graphics Features: New API classes for ([Shape3D](#shape3d)) like ([Box](#box)), ([Cylinder](#cylinder)), ([MeshView](#meshview)), and ([Sphere](#sphere)). Other additions include ([SubScene](#subscene)), ([Material](#material)), ([PickResult](#pickresult)), and lighting classes like ([AmbientLight](#ambientlight)) and ([PointLight](#pointlight)). The ([Camera API](#camera-api)) has also been updated.
    * This is not very useful for our project.
    * JavaFX 3D Graphics Guide
* Canvas API: Enables drawing directly within a JavaFX scene using a single graphical element (node).
* Printing API: The ([javafx.print](#javafxprint)) package provides public classes for JavaFX printing.
    * Uses print jobs to manage more specific image, graph, and gradient rendering. We likely will not use this for Monopoly.
* Rich Text Support: JavaFX 8 enhances text handling, including ([bi-directional text](#bi-directional-text)) support and complex scripts (e.g., Thai, Hindu). Multi-line, multi-style text is now supported in ([text nodes](#text-nodes)).
* Multitouch Support: JavaFX supports multitouch gestures based on platform capabilities.
* Hi-DPI support: JavaFX 8 includes improved support for high-resolution ([Hi-DPI](#hi-dpi)) displays.
* Hardware-accelerated graphics pipeline: JavaFX graphics use the ([Prism](#prism)) rendering pipeline, enabling smooth rendering when a supported ([GPU](#gpu)) is available. If no compatible GPU is found, Prism defaults to software rendering.
* High-performance media engine: The JavaFX media pipeline supports web multimedia playback with low latency. It is based on the ([GStreamer](#gstreamer)) framework.
* Self-contained application deployment model: JavaFX applications can be packaged with all necessary resources and a private Java runtime. These packages behave like native applications for their respective OS.

---

# Definitions

## API
A set of routines, protocols, and tools for building software applications. It specifies how software components should interact.

## Ruby
A dynamic, open-source programming language designed for simplicity and productivity.

## XML
Extensible Markup Language, a flexible text format used to store and transport data.

## Web Component
A reusable piece of UI that can be embedded in different applications.

## WebKitHTML
An open-source web browser engine used to render HTML and CSS.

## HTML5
The latest version of the HTML standard, including new features like native audio/video support, APIs, and improved semantics.

## Web Sockets
A protocol providing full-duplex communication channels over a single TCP connection.

## Web Workers
A JavaScript API that allows running scripts in background threads to perform non-blocking operations.

## Web Fonts
Fonts that are hosted on the web and can be used in web pages via CSS.

## Swing Applications
Applications built using the Swing framework, a part of Java for creating graphical user interfaces.

## SwingNode
A class that allows embedding Swing components into JavaFX applications.

## UI Controls
Predefined JavaFX components like buttons, labels, text fields, etc., used to build user interfaces.

## CSS
Cascading Style Sheets, a style sheet language used for describing the presentation of a document written in HTML or XML.

## DatePicker
A JavaFX UI control that allows users to select a date from a calendar view.

## TreeTableView
A JavaFX control used to display hierarchical data in a table format.

## CSS Styleable
Classes in JavaFX that allow styling of JavaFX objects using CSS.

## Modena
The default theme for JavaFX applications starting in JavaFX 8, providing a modern, flat UI look.

## Caspian
The previous default theme for JavaFX, which can still be used if specified.

## Shape3D
JavaFX API classes for creating 3D shapes like Box, Cylinder, MeshView, and Sphere.

## Box
A 3D shape in JavaFX representing a rectangular prism.

## Cylinder
A 3D shape in JavaFX representing a cylindrical object.

## MeshView
A 3D shape in JavaFX that renders meshes (complex 3D models).

## Sphere
A 3D shape in JavaFX representing a spherical object.

## SubScene
A JavaFX class representing a subscene, a smaller 3D scene within a larger scene.

## Material
A class representing material properties such as color, texture, and lighting effects for 3D objects.

## PickResult
Represents the result of a 3D object being picked (selected) by the user.

## AmbientLight
A type of light in JavaFX that uniformly illuminates all 3D objects in the scene.

## PointLight
A type of light in JavaFX that emits light from a single point and radiates in all directions.

## Camera API
The JavaFX API for managing camera perspectives and views in 3D scenes.

## javafx.print
The JavaFX package for handling printing functionality, such as managing print jobs.

## Bi-directional Text
Text that can be displayed in both left-to-right and right-to-left orientations, typically used for languages like Arabic and Hebrew.

## Text Nodes
A JavaFX node used to display text in a scene.

## Hi-DPI
High Dots Per Inch displays, typically referring to screens with higher resolutions for better visual clarity.

## Prism
The JavaFX graphics rendering pipeline that allows efficient rendering using hardware acceleration.

## GPU
Graphics Processing Unit, a specialized processor used for rendering images and videos efficiently.

## GStreamer
An open-source multimedia framework used for handling media content such as video and audio.
