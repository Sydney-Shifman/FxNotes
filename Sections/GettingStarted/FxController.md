# JavaFX Controller
([Source documentation](https://docs.oracle.com/javase/8/javafx/api/javafx/scene/control/Control.html))

## **Overview**
* Control is the base class for all UI controls in JavaFX.
* Inherits from Region and implements Skinnable.
* Controls represent UI elements that can be interacted with by users.
* Supports skinning to customize appearance while retaining default functionality.

## **Key Properties**
* **contextMenu**: Displays a context menu for the control.
* **skin**: Represents the visual rendering of the control. 
* **tooltip**: Displays a tooltip for the control. 
* **focusTraversable**: Most controls have this set to true by default, except for certain read-only or container controls (like Label, ProgressIndicator, ScrollPane, and ToolBar).

## **Important Methods**
* **computeMinWidth and computeMinHeight**: Calculate the minimum size based on other dimensions.
* **computeMaxWidth and computeMaxHeight**: Calculate the maximum size based on other dimensions.
* **computePrefWidth and computePrefHeight**: Compute the preferred size based on available dimensions.
* **createDefaultSkin**: Creates a default skin for the control if not provided explicitly.
* **layoutChildren**: Invoked during layout to arrange child nodes.
*** set/getSkin**: Used to set and retrieve the visual skin of the control.

## **Accessibility Support**
Supports accessible actions and attributes for assistive technologies (e.g., screen readers).

## **Resizability**
All Control objects are resizable by default.

## **Styling**
Controls support CSS styling and provide a getCssMetaData method to handle custom styling.

## **Subclasses**
Accordion, ButtonBar, ChoiceBox, ComboBoxBase, HTMLEditor, ListView, MenuBar, Pagination, ProgressIndicator, ScrollBar, Slider, Spinner, TabPane, TextInputControl, ToolBar, TreeView, TreeTableView, etc.

## **Constructors**
The default constructor creates a new Control.

---
