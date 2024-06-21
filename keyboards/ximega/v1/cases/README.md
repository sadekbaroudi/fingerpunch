# ximega

## overview

First and foremost, please note that there may be some files are for the left half, and don't have a corresponding right half. This means they can be mirrored to make the right half. For those that are asymmetrical and require different case models for each half, you'll notice there is a `left` and `right` version of that cover.  

To mirror a file, there are a variety of ways to do this:
* Mirror in your slicer before printing
* Import into a 3D modeling tool and mirror it
* Use an online tool to mirror the stl ( example: https://stl-mirror.beekeeb.com/ )

## parts for printing

To make a case for ximega, you'll need a minimum of 6 pieces:
* `ximega-base.stl` - left and right base, which are universal for MX or choc/glp (gateron low profile)
* `ximega-mx-switchplate.stl` or `ximega-choc-glp-switchplate.stl` - left and right switchplates
* An appropriate cover - There are `mx` and `choc-glp` versions of all covers, and there are different covers for the various VIK modules that you may be using. You'll need to select one for each half and print.
* Some covers require additional prints, like the trackball and display, which have an additional cover to go on top. The names should tell you which files to use. For example, `ximega-vik-pmw3360-34mm-trackball-cover.stl` would go with `ximega-mx-cover-vik-pmw3360-34mm-left.stl`

Note that the parts are testing using FDM 3D printing. Tolerances may vary depending on printing approach or materials used. Also, in my experience, some of the corners of the models lift a bit when using FDM if you don't have a finely tuned printer and good adhesion. If that's the case, I recommend using a brim, and then removing the brim with a deburring tool.

## parts for assembly

You'll need the following parts to assemble your board:
* 10-16 M2 heat set inserts, should be 3.6mm diameter and 3.5-4mm depth. You should use 5 per half, but if you want to really tightly secure the top cover to the body, you can use up to 8 per half.
* 10-16 M2 screws, 6mm length
* If you are using a VIK module, you may need 2-4 more heat set insert and screws per half. These are used to mount the VIK module PCB to the top cover
