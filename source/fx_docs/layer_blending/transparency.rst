.. _transparency:

Transparency
==================

|node|

Inputs:
-------

| **Source**, The image that will be affected.

Parameters:
-----------

| **Intensity**, Controls the overall strength of the effect.
| A value of 50 will produce a result halfway between the Source image and the full effect.

Usage Example:
--------------

We will see the transparency of a yellow circle on top of a black rectangle background

|circle| |background|


This is how the image levels are connected in the FX schematic; by connecting the circle level to the source input we can control the circle's transparency

|fx_schematic|

Here is the result; the first image is with zero percent transparency, the second image is with fifty percent transparency, and the third image is with seventy five percent transparency

|example_1| |example_2| |example_3|



.. Images
.. |node| image:: /_static/fx_docs/layer_blending/transparency/node.png
	:scale: 150%
.. |circle| image:: /_static/fx_docs/layer_blending/transparency/circle.png
	:scale: 50%
.. |background| image:: /_static/fx_docs/layer_blending/transparency/background.png
	:scale: 50%
.. |fx_schematic| image:: /_static/fx_docs/layer_blending/transparency/fx_schematic.png
	:scale: 100%
.. |example_1| image:: /_static/fx_docs/layer_blending/transparency/transparency_example_zero_percent.png
	:scale: 50%
.. |example_2| image:: /_static/fx_docs/layer_blending/transparency/transparency_example_fifty_percent.png
	:scale: 50%
.. |example_3| image:: /_static/fx_docs/layer_blending/transparency/transparency_example_seventy_five_percent.png
	:scale: 50%
