# ximi v1 case

There are a lot of files in here, so allow me to explain the name format!

## body

The file name format for the body is as follows: 
`xi-{5|6}-{mx|choc}-{tr|c|trth|np}-{ec|ne}-{3wt|_}-{disp}-{left|right}.stl`

* `5|6` - This is 5 or 6 column
* `mx|choc` - The heights are adjusted such that it's suitable for MX or choc switches 
* `tr|c|trth|np` - trackball, cirque, thumb trackball (trth), or no pointing device 
* `ec|ne` - ec11 or no encoders 
* `3wt|_` - three way thumb switches or none (I stopped adding the ones that don't have the cutouts since the 3 way thumb switches are pre-soldered on the pcb for current pcbs) 
* `disp` - mounting for waveshare 1.47inch display (sku 22224)
* `left|right` - left or right half. There may not be a right half in all cases, simply because you can mirror the left stl. In some cases, like the cirque, you cannot mirror the stl since the mount for the cirque won't work that way. You need to actually print the right half in that case, as provided here. 

## bottom plate

The file name format for the bottom is as follows: 
`xi-{5|6}-bot-{2.8mm|_}-{trackball|cirque|trth|_}-left.stl`

* `5|6` - This is 5 or 6 column 
* `2.8mm|_` - This is a slightly taller bottom plate, which gives you 1.4mm extra space under the pcb. This was made to accommodate the haptic feedback module, since it takes up a bit more space 
* `trackball|cirque|trth|_` - this should match the body that you used 

Similar to the body, you can mirror the bottom plate to get the right side

## trackball covers

`xi-trackball-cover-{slimmer|slim|wide|wider}.stl`

These are 4 versions of the trackball cover with slightly wider and wider bottom edges. This is to accommodate the fact that different printers will produce different results. Hopefully one of these should produce a trackball cover that has a nice pressure fit into the trackball case.

Personal experience and feedback:
* In my current FDM printer (Snapmaker A350T), the "wider" stl works best.
* Printing via JLCPCB MJF, the slimmer option should work best. I received feedback that the slim one worked, but required a little bit of filing at the bottom.
