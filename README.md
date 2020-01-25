# TheFinalChessCard

TheFinalChessCard for C64/C128, replicated using SprintLayout. Here are the sprint and gerber files.

The scanned images are from the World of Jani blog article about this card. See also the forum64.de threads.
- http://blog.worldofjani.com/?p=3460
- https://www.forum64.de/index.php?thread/73757-the-final-chesscard/

## preview images from SprintLayout

![replica top](tfcc_replica_top.JPG?raw=true)
![replica bottom](tfcc_replica_bottom.JPG?raw=true)

# The Replica 1.0 prototype

The PCB Rev 1.0 has been [prototyped by Amon_RA on twitter](https://twitter.com/Amon_RA/status/1220659582181224448 "The tweets"). Thank you so much! Here are two images from his setup:

Image 1            |  Image 2
:-------------------------:|:-------------------------:
![cart](working_replica_1_0_amon_ra_1.jpg?raw=true)  |  ![screen](working_replica_1_0_amon_ra_2.jpg?raw=true)


The Rev 1.0 had a grounded READ pin near the top edge. To find it look at the 74LS32 closest to the CPU, pin 8. If you have Rev 1.0, cut this trace betwen pin8 and GND at top edge. This is fixed in Rev 1.1

![replica 1_0 cut here](tfcc_replica_top_1_0_cut_here.png?raw=true)

I would also like to thank the work by lvr for the schematics draft he posted in [a forum64.de thread](https://www.forum64.de/index.php?thread/73757-the-final-chesscard/&postID=1139564#post1139564 "A draft of the schematics for TheFinalChessCart"). With this schematic I was able to match my gerbers against a netlist generated from his schematics, and in this way the error in Rev 1.0 was easy to spot. The draft was very close to the layout. Thanks also to [@thilographie_de](https://twitter.com/thilographie_de) for hunting the error with me.

# Links

After doing the C64 KU-motherboard and the videoseries, I still hadn't shown my viewers how I went from images to gerber files. This is where I got the motivation for doing this TFCC replica. I made two videos. The first video got linked on Jani's website and also ended up in an article about it on hackaday called [Reverse Engineer PCBs With SprintLayout](https://hackaday.com/2019/12/31/reverse-engineer-pcbs-with-sprintlayout/). :-)


[![first video](https://img.youtube.com/vi/g0nkLJ4YQ2c/0.jpg)](https://www.youtube.com/watch?v=g0nkLJ4YQ2c)

[![update video](https://img.youtube.com/vi/2UtY5fDaRgo/0.jpg)](https://www.youtube.com/watch?v=2UtY5fDaRgo)


## Change log

* 2020-01-25 Rev 1.1:
  * pin 8 "READ" on 74LS32 (near CPU) was grounded. Removed GND.
  * A trace stopped too early before a via. Still connected. Fixed.
* 2019-12-31 Rev 1.0: Touched up traces on a finer grid. 45degree bends.
* shown in video: traced up. quick 90 degree bends
