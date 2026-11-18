IB's Flora



Author: ipebloom (Discord)  

Toolbar: IB's flora  

Platform: Roblox Studio  

Version: 0.1a 

Subversion: alpha

Type: Multi-purpose Plugin Suite



IB's Flora is a multi-purpose Roblox Studio plugin that brings several development tools together under one toolbar. It currently includes utilities for browsing scripts, editing UI elements, manipulating instances, managing reusable assets, and customizing the plugin's interface.



The suite is split into three components: CodeTree, Fertilizer, and Herbarium. Each has its own set of tools and a different role within Studio.



THIS WHOLE THING WAS VIBECODED BTW, don't expect it to work perfectly every time, again this was made because I'm lazy and didn't want to download 100+ plugins for all this stuff.



\---



Included Tools



1\. CodeTree — Script \& Hierarchy Explorer



CodeTree provides a collapsible tree view of commonly used Roblox services and their contents. The layout takes inspiration from Godot's scene tree, with branch connectors and expandable entries that make navigating nested instances more manageable.



Supported services:

\- `ServerScriptService`

\- `ServerStorage`

\- `ReplicatedStorage`

\- `ReplicatedFirst`

\- `StarterPlayer`

\- `StarterGui`

\- `Workspace`



Features:



\- Tree Navigation: Displays instances in a nested hierarchy using visual branch connectors (`├─`, `└─`, `│`).

\- Script Type Icons: Assigns different icon colors to `Script`, `LocalScript`, and `ModuleScript` instances, making them easier to identify while browsing.

\- Live Search: Filters the displayed hierarchy as you type, without requiring manual navigation through folders.

\- Quick Script Creation: Hover over a folder to reveal a `+` button. Clicking it creates a script directly inside that folder.



The explorer is particularly useful when a project has scripts scattered across several services and nested folders.



2\. Fertilizer — Development Utilities \& Customization



Fertilizer contains the smaller utilities used throughout everyday Studio development. Its interface organizes tools into individual cards, with a favorites system for pinning frequently accessed ones.



Favorites \& Organization

\- Pin utility cards to keep frequently used tools accessible.

\- Manage favorites without having to browse through the entire tool collection.



UI Development

\- Automatically insert `UIAspectRatioConstraint` instances into selected UI elements.

\- Convert `Size` and `Position` values between Scale and Offset.

\- Interactive 3×3 `AnchorPoint` selector.

\- Freely drag an element's `AnchorPoint`, with optional snapping for more controlled positioning.



Instance Manipulation

\- Auto-Anchor and Auto-Collision listeners.

\- Batch transparency adjustment.

\- Quick material cycling.

\- Align and distribute instances along the X, Y, and Z axes.

\- Pivot to Center.

\- Quick Weld for connecting parts.

\- Convert Parts into Terrain.

\- Generate a 20-stud `TemplateGrid` Baseplate.



Workflow Utilities

\- Batch Rename: Change the names of multiple instances in a single operation.

\- Quick Duplicate: Duplicate instances with a configurable positional offset.

\- Property Clipboard: Copy properties from one instance and apply them to another.

\- Camera Light: Add additional lighting to the camera view when working in darker environments.

\- Clean Screenshot Mode: Hide interface clutter for unobstructed Studio screenshots.



Theme Hub



Fertilizer has a built-in theme manager that supports importing and switching between custom interface themes.



\- Load `.css` theme files directly from your computer.

\- Switch between installed themes using a dropdown.

\- Includes `Default Blue`, `Nightshade`, and `Snowy Christmas` presets.

\- Supports custom CSS themes through a variable-based configuration format.



3\. Herbarium — Asset Library \& Archival System



Herbarium is the asset storage and archival tool in IB's Flora. It lets you save models, parts, and other reusable content in a library, then retrieve them in other Roblox Studio projects.



Stored assets can have their own previews, categories, and tags. The library also includes insertion options for placing assets into the current project without manually copying them from older places.



Asset Library \& Quick Insert



\- Store serialized assets in a reusable library accessible across projects.

\- Generate framed previews with `ViewportFrame`.

\- Organize entries using categories and tags.

\- Insert assets through three placement modes:

&#x20; - `Workspace` — Places the asset directly into Workspace.

&#x20; - `In Selected` — Inserts the asset into the currently selected instance.

&#x20; - `Raycast Placement` — Uses raycasting to determine the placement position in the 3D world.



Asset Organization



\- Create, rename, and manage custom asset categories.

\- Batch rename stored assets.

\- Search for potential duplicates using structural signatures instead of comparing names alone.



The structural comparison is useful when two assets have different names but share a similar internal composition.



Material Library



\- Save color, material, and surface presets.

\- Reuse saved configurations in other Studio places.

\- Keep frequently used material combinations available without recreating them manually.



Snapshots \& Versioning



\- Capture versioned snapshots of Models and Parts.

\- Restore previously captured versions.

\- Compare snapshots to inspect changes in part counts and volume deltas.



\---



Custom CSS Theme System



Fertilizer's theme system uses CSS custom properties to control the appearance of IB's Flora. Rather than editing interface styles individually, users can define their preferred colors and effects in a single `.css` file.



The available variables cover backgrounds, sidebars, hover and selection states, typography, folder icons, and script-specific colors. Optional effects can also be configured through the same file.



Importing a theme



1\. Create a `.css` file on your computer.

2\. Add your theme variables using the structure below.

3\. Open `IB's flora` in Roblox Studio.

4\. Navigate to Fertilizer → Utilities.

5\. Click Import .css and select your file.



Example theme configuration:



```css

:root {

&#x20;   --theme-name: "Default Blue";



&#x20;   /\* Interface \*/

&#x20;   --background: #1d2229;

&#x20;   --sidebar-bg: #252b34;

&#x20;   --item-hover: #2f3742;

&#x20;   --item-selected: #3b4654;



&#x20;   /\* Typography \*/

&#x20;   --text-primary: #cdcfd2;

&#x20;   --text-secondary: #7d8590;



&#x20;   /\* Accent Colors \*/

&#x20;   --accent: #57b3ff;

&#x20;   --folder-color: #6ea8fe;



&#x20;   /\* Script Class Colors \*/

&#x20;   --script-color: #75e6b8;

&#x20;   --local-script-color: #7cc4fa;

&#x20;   --module-script-color: #a855f7;



&#x20;   /\* Optional Effects \*/

&#x20;   --has-snow: false;

&#x20;   --snow-color: #ffffff;

}

```



The same theme configuration is used throughout CodeTree, Fertilizer, and Herbarium, keeping their interface colors consistent when switching themes

