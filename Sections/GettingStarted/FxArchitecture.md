# **JavaFX Architecture Summary**

## **Overview**
JavaFX architecture comprises multiple components that work together to support rich client application development. The core elements include:

- [Scene Graph](#scene-graph)
- [Java Public APIs](#java-public-apis)
- [Graphics System](#graphics-system)
- [Glass Windowing Toolkit](#glass-windowing-toolkit)
- [Media & Images](#media--images)
- [Web Component](#web-component)
- [CSS](#css-styling)
- [UI Controls](#ui-controls)
- [Layout](#layout)
- [2D & 3D Transformations](#2d--3d-transformations)
- [Visual Effects](#visual-effects)

---

## **Scene Graph**
The **[Scene Graph](#scene-graph-definition)** is a hierarchical tree structure of visual elements in a JavaFX application.

### **Components:**
- **Nodes** (each has an ID, style class, and bounding volume)
  - The components that do/display things in the UI
- **Effects** (blurs, shadows)
- **Opacity & Transforms**
- **Event Handlers** (mouse, key, input)
- **Application-specific states**

### **Advantages:**
- Simplifies UI creation.
- Supports rich UI animations via `javafx.animation`.
- Works well with declarative XML-based UI.

---

## **Java Public APIs**
JavaFX provides a set of **[Java Public APIs](#java-public-apis-definition)** for developing applications.

### **Key Features:**
- Supports **generics, annotations, multithreading, and lambda expressions**.
- Facilitates JavaFX integration with **Groovy, JavaScript, and other JVM-based languages**.
- Includes **binding mechanisms** for UI and data synchronization.
- Uses **CSS for styling** and **ARIA for accessibility**.

---

## **Graphics System**
The **[Graphics System](#graphics-system-definition)** handles rendering of both 2D & 3D scene graphs.

### **Key Components:**
- **Prism**: Graphics pipeline that supports DirectX 9, DirectX 11, OpenGL, and software rendering.
- **Quantum Toolkit**: Bridges Prism and the **[Glass Windowing Toolkit](#glass-windowing-toolkit-definition)**.

---

## **Glass Windowing Toolkit**
The **[Glass Windowing Toolkit](#glass-windowing-toolkit-definition)** manages native OS services such as windows, timers, and surfaces.

### **Event Queue Handling:**
- Uses native OS event queues.
- Runs on the **JavaFX Application Thread**.

### **Threads:**
- **JavaFX Application Thread**: Handles UI updates.
- **Prism Render Thread**: Separates rendering from event handling.
- **Media Thread**: Manages media playback.

---

## **Media & Images**
The **[Media Engine](#media-engine-definition)** enables JavaFX applications to play visual and audio media.

### **Supported Formats:**
- **Audio**: MP3, AIFF, WAV
  - Use this for dice rolling noise or even monopoly man voice lines.
- **Video**: FLV

### **Key Components:**
- **Media**: Represents a media file.
- **MediaPlayer**: Plays a media file.
- **MediaView**: Displays media content.

---

## **Web Component**
The **[Web Component](#web-component-definition)** provides a built-in Web viewer using WebKit.

### **Features:**
- Render HTML content from local/remote URLs.
- Support history navigation (Back/Forward).
- Execute JavaScript commands.
- Apply effects to web content.

### **Main Classes:**
- **WebEngine**: Handles webpage loading.
- **WebView**: Displays web content.

---

## **CSS Styling**
The **[CSS](#css-definition)** system allows JavaFX applications to apply styles dynamically.

### **Key Points:**
- Based on **W3C CSS 2.1** with some CSS3 additions.
- Uses `-fx-` prefix for JavaFX-specific properties.
- Enables dynamic theming at runtime.

---

## **UI Controls**
The **[UI Controls](#ui-controls-definition)** in JavaFX are built using the scene graph.

### **Examples:**
- Buttons, Labels, TextFields, Checkboxes
- ListView, TableView, TreeView
- ProgressBars, Sliders, Menus

### **Customization:**
- Fully stylable via **CSS**.
- Can be extended using **custom skins**.

---

## **Layout**
The **[Layout System](#layout-definition)** provides various layout containers for arranging UI elements.

### **Common Layouts:**
- **BorderPane**: Top, bottom, left, right, center regions.
- **HBox & VBox**: Horizontal and vertical layouts.
- **StackPane**: Overlapping elements in a stack.
- **GridPane**: Grid-based arrangement.
  - We Will likely use this if we don't use strictly CSS for formatting 
- **FlowPane & TilePane**: Flowing or tiled layouts.
- **AnchorPane**: Anchored positioning.

---

## **2D & 3D Transformations**
The **[Transformation System](#transformation-system-definition)** enables positioning and modifying UI elements.

### **Transformation Types:**
- **Translate**: Moves a node along the X, Y, Z axes.
- **Scale**: Resizes a node.
- **Shear**: Skews an axis.
- **Rotate**: Rotates a node.
- **Affine**: Performs linear mapping for transformations.

---

## **Visual Effects**
The **[Effects System](#effects-definition)** enhances JavaFX applications using real-time graphical effects.

### **Common Effects:**
- **Drop Shadow**: Adds shadow behind elements.
- **Reflection**: Creates mirror-like reflections.
- **Lighting**: Simulates light sources for 3D effects.

---

# **Definitions**
### **Scene Graph Definition**
A hierarchical tree of UI elements in a JavaFX application.

### **Java Public APIs Definition**
A set of JavaFX libraries that enable developers to build rich UI applications.

### **Graphics System Definition**
The rendering engine for JavaFX, supporting 2D/3D scenes and hardware acceleration.

### **Glass Windowing Toolkit Definition**
The low-level toolkit managing native OS interactions for JavaFX applications.

### **Media Engine Definition**
A system that provides media playback capabilities in JavaFX.

### **Web Component Definition**
An embedded WebKit-based browser allowing JavaFX applications to render HTML content.

### **CSS Definition**
A styling system that enables JavaFX applications to use Cascading Style Sheets.

### **UI Controls Definition**
Prebuilt JavaFX components like buttons, text fields, and tables.

### **Layout Definition**
A system that provides flexible and dynamic positioning of UI elements.

### **Transformation System Definition**
JavaFX classes that allow moving, scaling, rotating, and skewing UI elements.

### **Effects Definition**
Graphical enhancements like shadows, reflections, and lighting in JavaFX.
