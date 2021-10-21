# svg-renderer-flex-library
Detached fork of lucaslorentz/AS3SVGRenderer/SVGRendererFlex

AS3SVGRenderer
==============

An AS3 SVG Renderer for Flash Player.

It parses and translates svg elements to Flash display objects. Rendering it and letting you interact with the output.

Requirements:
* Flash Player 10+

Features:
* Supports basic shapes and paths.
* Supports texts, right-to-left scripts, subscript, superscript.
* Has 3 text renderers engines (TextField, TLF, FTE), supports CFF and non-CFF fonts.
* Supports coordinates system rules, transformations and units.
* Supports masking and clipping.
* Supports filling, strokes, gradients.
* Supports marker symbols.
* Supports basic document structure (g, defs, symbol, use, image).
* Supported filters: ColorMatrix, GaussianBlur.
* Rendered display objects keeps the svg structure, so you can code mouse/touch interactions with svg elements.
* AS3 only.
* Flex component.

Missing features:
* Text stroke.
* Some filters.
* Scripting.
* Animation.

INTRODUCTION
==============

The library has display classes that represents each SVG element.  
The SVGDocument class is the class responsible to hold the SVG display object tree.  
The library has an asynchronously parser that processes the SVG file and create all necessary display objects.  
You can listen to the RENDERED event to know when graphics was completely rendered for the first time.  

USAGE
==============

1. Clone and build [svg-renderer-library](https://github.com/ciacob/svg-renderer-library.git). It should produce **svg-renderer-library.swc**. Add it to your Flex/AIR project path.

2. Add the SVG component to your MXML, and set the property "Source" on the component to:
  * a string with the URL of the SVG file.
  * an urlRequest to achieve the SVG file.
  * a string with the content of the SVG file.
  * an XML object with the content of the SVG file (not recommended).

3. Done :-). The SVG file will appear on the screen.

LICENSE
==============
Licensed under the MIT License.  
http://opensource.org/licenses/mit-license.php
