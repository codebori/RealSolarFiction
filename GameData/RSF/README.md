https://forum.kerbalspaceprogram.com/index.php?/topic/196996-real-world-sci-fi-mod-collection/

The goal is to create a real world semi realistic sci-fi mod collection with the focus on (but not limited to) achieving off world self sufficient bases.

It will probably be in the form of a "mod" (Real Solar Fiction) containing patches to glue everything together, based on my old project SpaceBori’s resource patches.

I am not a developer, nor a graphic designer and I don't want to do work that has already been done. So the project should not be so realistic that it becomes too complex.

For now we'll have 2 forks. One depending on Real Fuels and the other on Rational Resources. Both combinations will need to be tested and everything can still change.

We are starting with RSF+RF:
```diff
+ Compatible 
! Needs some patches 
- Incompatible
# Testing

Depends:
+ Real Fuels (https://forum.kerbalspaceprogram.com/index.php?showtopic=58236)
+ RealFuels-Stock ()
+ LRTR ()
+ RSS ()
+ Kerbal Construction Time ()
+ Module Manager ()

Recommends:
+ Kerbalism ()
+ Kerbalism - LRTR Config (https://forum.kerbalspaceprogram.com/index.php?/topic/189978-*)
! Procedural Parts ()
! Completely Non-Aggressive Rocketry (V-2) (https://forum.kerbalspaceprogram.com/index.php?/topic/188554-19-completely-non-aggressive-rocketry-v2-rocket-add-on/)
! SXT Continued ()
# Taerobee (https://forum.kerbalspaceprogram.com/index.php?/topic/119858-14x-taerobee-stockalike-x-1-and-more-27012017/)

Suggests:
+ Kerbal Engineer Redux ()
! RealAntennas ()
+ Gordon's RealAntennas patches ()

Compatible:
! Airplane Plus ()
+ Ferram Aerospace Research Continued ()
+ Kerbal Alarm Clock ()
+ Kerbal Joint Reinforcement - Continued ()
! Tantares (https://forum.kerbalspaceprogram.com/index.php?/topic/73686-110x-tantares-stockalike-soyuz-and-mir-23201112020/)
+ WasdEditorCameraContinued (http://forum.kerbalspaceprogram.com/index.php?/topic/121386-*)

# Currently testing:
        Advanced Fly-By-Wire
        Advanced Jet Engine
        AirlockPlus
        Auto Actions
        B9 Aerospace Procedural Wings - Fork
        BetterBurnTime
        blackheart612's Procedural Part Textures
        CapCom - Mission Control On The Go
        Cryo Tanks
        Cryogenic Engines
        DMagic Orbital Science -> Incompatible with LRTR's Kerbalism Config
        Hangar Extender
        KAX
        Kerbal Atomics
        Kerbal Attachment System
        Kerbal Inventory System
        Kerbal Stats
        Kerbal Planetary Base Systems
        KRASH
        KSP AVC
        KSP Rescue Pod Fix
        KSP Resonant Orbit Calculator
        Mark IV Spaceplane System
        MechJeb 2
        Mk2 Stockalike Expansion
        Near Future Aeronautics
        Near Future Construction
        Near Future Exploration
        Near Future Propulsion
        Near Future Solar
        Near Future Spacecraft
        Not So SimpleConstruction (NSSC)
        OhScrap!
        OPT
        OSE Workshop
        Patch Manager
        Portrait Stats
        Procedural Fairings
        QuickSearch
        RCS Build Aid Continued
        Real Plume
        RealChute
        RealHeat
        ReStock
        ReStock Extra - Rigid Legs
        ReStock+
        Retracting/vectoring engines, Critter Crawler
        RSS DateTime Formatter
        SCANsat
        ScrapYard
        Ship Manifest
        Smart Parts
        StageRecovery
        Stockalike Station Parts Expansion Redux
        Talisar Parts
        Universal Storage II

To be tested:
        Airline Kuisine
        BARIS
        Duna Direct
        Extraplanetary Launchpads
        Global Construction
        Pathfinder
        Rational Resources
        SMURFF
	KSPIE

Incompatible:

All:
- Crew R&R -> Overlaps with LRTR RP-1 functionality.
- Realism Overhaul -> Incompatible with/same functionality as LRTR.
- TAC-LS and Remote Tech -> Incompatible with/same functionality as Kerbalism.
- Hide Empty Tech Tree Nodes -> Incompatible with LRTR RP-1 functionality.
- Procedural Fairings for Everything -> Seems to be incompatible with most mods, in this case it seems to mess up the Tech Tree.
- Advanced Jet Engine -> Old, broken and seemingly no longer maintained.
RF:
- Mark IV Spaceplane System -> Incompatible with RF while OPT provides similar compatible parts so it is not worth the effort to write patches for Mark IV.
```

I don't want to do this alone and just for myself. So who's interested in playing (more or less) realistic career sci-fi KSP? And who wants to help put this together?

Discord: https://discord.gg/kA6BQVD 

## Known Issues:

- [] "DMagic Orbital Science" is incompatible with LRTR's Kerbalism Config  
- [] "OhScrap!" overlaps with Kerbalism functionality
- [] SXT LV-405 Vanguard still has Liquid Fuel and Oxidizer for its additional RCS engine 
- [] "Restock" Oscar B tank volumes are inconsistent with the stock one
- [] Procedural Part Tanks are to big at the start and too small later on
- [] TantaresSP Zircon RCS Series require Liquid Fuel and Oxidizer 
- [] Some Tantares engines have very high ISP  
 
## To Do
 
- [] Write installation instructions: 
	- [] Dependencies: 
		- [] Kerbalism -> Kerbalism LRTR Config
	- [] Configuration:
		- [] Turn off Real Fuels or Kerbalism ignition limit
- [] Make "DMagic Orbital Science" compatible with LRTR's Kerbalism Config  
- [] Suggest more configuration options for "OhScrap!" to turn of some functionality
- [] Move Airplane parts (Stock and from mods) around in the Tech Tree (mainly earlier)
- [] [SXT LV-405 Vanguard](https://github.com/linuxgurugamer/SXTContinued/blob/master/GameData/SXT/Parts/Rocketry/Engine/Vanguard/X405.cfg) still has Liquid Fuel and Oxidizer for its additional RCS engine -> write patch and submit it to RealFuels-Stock 
- [] Fix Oscar B tank volumes: https://forum.kerbalspaceprogram.com/index.php?/topic/196996-real-world-sci-fi-mod-collection/&do=findComment&comment=3862324
- [] Make sure there are ullage motors available early in the tech tree
- [] Remove the Size restrictions from PP tanks, leave only the volume related upgrade path
- [] Fix TantaresSP Zircon RCS Series require Liquid Fuel and Oxidizer and submit it to RealFuels-Stock
- [] Check Tantares engines ISP

## Changelog

- [x] 31.10.2020: B9 Wings Tech Tree patch by Sirata89: https://github.com/codebori/RealSolarFiction/commit/aa4443fc79d3f54f85e24adc63e2887291c68260
- [x] 31.10.2020: Changed size limits for Procedural Fuel tanks (multiple commits) 
- [x] 31.10.2020: Replace Oxidizer with LqdOxygen in Fuel Cells: https://github.com/codebori/RealSolarFiction/commit/db999402aebc87a303337b3e3f9dca50ae1a7a36
- [x] 31.10.2020: Added CKAN modpack list to Github
- [x] 31.10.2020: Created a Changelog


### Before there was order: 
- [x] Adapted LRTR KCT config to allow for faster build time with recovered parts. -> RSF_KCT_Presets.cfg
- [x] Kerbalism built-in antennas not sending data -> seems intentional
- [x] Added early (propellor) plane mods -> [SXT Continued](https://forum.kerbalspaceprogram.com/index.php?/topic/151129-19x-sxt-continued/), [KAX?](https://forum.kerbalspaceprogram.com/index.php?/topic/180268-131/), [Airplane Plus](https://forum.kerbalspaceprogram.com/index.php?/topic/140262-14x-18x-airplane-plus-r264-fixed-issuesgithub-is-up-to-date-dec-21-2019/)
- [x] Fixed fairing sizes (currently in career only smallest fairing when bigger parts already available) -> RSF_TT.cfg
- [x] Fixed procedural tank sizes -> RP_Tree_ProcSizes.cfg
- [x] Added mod for early LRTR tech tree for FAR -> Aerodynamic sounding rockets etc. -> [CNAR-V2](https://forum.kerbalspaceprogram.com/index.php?/topic/188554-19-completely-non-aggressive-rocketry-v2-rocket-add-on/)
- [x] Fixed no tank type selection for any tank except the procedural tanks. -> RP_PartHacks.cfg
- [x] Pressurized tanks (Service module) when you get pressure fed engines. -> RP_PartHacks.cfg  & RP_Tree_ProcSizes.cfg
- [x] Fixed EVA Fuel (monoprop -> hydrazine)
