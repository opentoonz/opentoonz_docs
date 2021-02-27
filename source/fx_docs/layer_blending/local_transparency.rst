.. _local_transparency:

Local Transparency
==================

|node|

Inputs:
-------

| **Source**, The image that will be affected.

| **Reference**, The luminance of the Reference image will control the opacity of the Source.
| The Source will be made transparent where the Reference is light, and opaque where the Reference is dark.

Parameters:
-----------

| **Intensity**, Controls the overall strength of the effect.
| A value of 50 will produce a result halfway between the Source image and the full effect.

Usage Example:
--------------

We can use a checker pattern to control the opacity of a circle

|circle| |checker|


This is how the two levels are connected in the FX Schematic; by connecting the checker level to the Reference input, we will use its luminance to mask portions of the circle

|graph|

Here is the result; the red circle is visible within the black areas of the checker pattern and not in the white areas

|example| |example_2|



.. Images
.. |node| image:: /_static/fx_docs/layer_blending/local_transparency/local_transparency_node.png
	:scale: 150%
.. |circle| image:: /_static/fx_docs/layer_blending/local_transparency/local_transparency_circle.png 
	:scale: 50%
.. |checker| image:: /_static/fx_docs/layer_blending/local_transparency/local_transparency_checker.png 
	:scale: 50%
.. |graph| image:: /_static/fx_docs/layer_blending/local_transparency/local_transparency_graph.png
	:scale: 100%
.. |example| image:: /_static/fx_docs/layer_blending/local_transparency/local_transparency_example.png
	:scale: 50%
.. |example_2| image:: /_static/fx_docs/layer_blending/local_transparency/local_transparency_example_2.png
	:scale: 50%
