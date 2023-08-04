# This fork is no longer maintained.  I leave it for anyone wanting sailfin for voron heatserts or old sharkfin.  [Sharkfin is updated and now has it's own repo.](https://github.com/KayosMaker/Sharkfin_Extruder)
# For Sailfin, visit the home repo.

# Sailfin-Extruder
A lightweight compact extruder with 5:1 gearing using BMG dual drive.   It is capable of pushing up to 48mm^3/s through a 0.4 nozzle.

Footprint is a very compact 41x45mm and weighs 107g (with steel fasteners).

Regular and mirrored version.   STEP files provided.  

There also is a version of the middle body which is compatible with toolheads designed for the Sherpa extruder.

Special thanks to Anlin over at Annex Engineering and his Sherpa mini extruder for inspiring the creation of Sailfin.

![Sailfin](https://github.com/CroXY3D/Sailfin-Extruder/blob/main/images/sailfin_large.png)

![Sailfin Scale](https://github.com/CroXY3D/Sailfin-Extruder/blob/main/images/sailfin_scale.jpg)


# BOM
* [LDO 17mm Nema14 Stepper with gear LDO-36STH17-1004AHG](https://www.printedsolid.com/products/ldo-nema-14-motor-ldo-36sth17-1004ahg?variant=32690500370517) or 20mm version LDO-36STH20-0504AHG which has more torque.
* [Bondtech BMG or clone internals.  Triangle Lab preferred](https://www.aliexpress.com/item/4000021186440.html)
* 1x M3x25 BHCS (SHCS may be used as well for all BHCS)
* 2x M3x14 BHCS
* 2x M3x10 BHCS
* 5x M3 Heatserts [McMaster](https://www.mcmaster.com/94459A130/) [AliExpress M3xD4.6x4](https://www.aliexpress.com/item/4000232858343.html)
* Short length 2mm ID, 4mm OD PTFE tube.
* Optional [Nema14 heatsink](https://www.filastruder.com/products/heatsink-for-pg35l-geared-stepper-motor?_pos=5&_sid=4f2b94743&_ss=r).  Enables higher motor current and more torque.  The motor is same diam as other 540 size RC motors so there are other heatsinks available from RC shops.
* Optional [Thermal tape for the heatsink](https://smile.amazon.com/Thermal-Adhesive-Performance-Heatsink-Computer/dp/B085CLXM7J/ref=sr_1_3?dchild=1&keywords=thermal+tape&qid=1617072316&sr=8-3)

# ASSEMBLY
Assembly is fairly straightforward.  

There are two parts with small membranes in holes to make printing a solid bridge.  Drill with 3mm drill bit the membrane on the lever and the membrane on the rear piece.

You may need to either push the white gear down 1-2 mm if it rubs on the Nema 14 motor.  Alternatively you may carefully grind off 1-2mm of the shaft.  Be careful of heat so you don't melt the nylon gear.

The cut guide helper is intended to help you cut the PTFE tube.   Place the PTFE tube in your toolhead and position the cut guide above it.  Use a razor blade to cut the tube.  It's helpful to countersink the top end of the tube with a chamfer bit or a conical deburring tool.

# TOOLHEADS

Toolheads are available for the following:
* Tiny-M V3 Gantry Dragon Toolhead
* Tiny-M V4 Gantry Toolhead (on Tiny-M GitHub)
* Voron V0 Dragon
* Voron V0 V6 Screw Mount

There is a version of the middle body that should be compatible with most Sherpa toolheads.  The motor sits a couple mm lower on the Sailfin, so you may also need a 2mm thick printed spacer to raise the Sailfin.

If you design a toolhead around it, let me know and i'll link or post STLs here.

There will be a Sailfin toolhead for CroXY soon.   


[Nice V0 toolhead that supports Sailfin](https://github.com/KurioHonoo/Mini-AfterSherpa/)

# MODS

[Sharkfin now has it's own repo.](https://github.com/KayosMaker/Sharkfin_Extruder)

[Sharkfin](https://github.com/KayosMaker/Sailfin-Extruder/tree/main/Usermods/KayosMaker/Sharkfin)

Sharkfin is a slightly reimagined Sailfin.  These mods were more to satisfy my own neurosis, than actually being strictly necessary.  My goals were as follows: 
* alter the motor location so that a spacer isn't needed to mount the extruder on Mantis
* move the motor enough so that the extruder mounting screw and lower motor mounting screw do not interfere with each other
* lengthen tension arm slightly so it's actually possible to move it with your thumb while its mounted in the tight space on Mantis
* add 3rd screw to front piece, so both the tension arm pivot and the driven gear are supported on both sides
* maintain sailfin motor mounting angle, so pcb mounting brackets made for sailfin work on sharkfin as well

[Sailfin for Voron Heat Inserts](https://github.com/KayosMaker/Sailfin-Extruder/tree/main/Usermods/KayosMaker/Sailfin_for_Voron_heat_inserts)

Sailfin for Voron heat inserts is just that.  It's a very minorly finessed stock Sailfin with holes altered to fit our standard heatsert in Voron land.  I like to debadge things so I also did that while I was at it.  

[PCB Mount](https://github.com/KayosMaker/Sailfin-Extruder/tree/main/Usermods/KayosMaker/Sailfin_PCB_mounts)

Mounting plate for the pancake PCB or Timmit PCB common on v0 and other Printers for Ants.  

[CAN Toolhead Board Mounts](https://github.com/KayosMaker/CANboard_Mounts)

This link leads to a seperate repository.  Included in that repo are mounts for Sailfin that work with the Mellow SHT-36 board, as well as mounts for the BTT EBB-36.  Included are basic no strain relief mounting plates, as well as mounting plates with built in strain relief.
