# Factorio-Resources
A Resource module for Factorio, Which is needed by DyTech, 5DIM, and Bob's Modules

This is a modders resource for Factorio. Every mod can use this, but it is most used by DyTech, 5DIM and Bob's modules.

How to use this?

start by editing you info.json:
this line:

"dependencies": ["base"]

becomes:

"dependencies": ["base", "Factorio-Resources"]

now start changing recipes:
in your recipes, use the following items (internal names):

ardite-plate, cobalt-plate, tin-plate, zinc-plate, gold-plate, silver-plate, tungsten-plate, lead-plate

if you wanna use the ores, replace the -plate with -ore.

Want to use the technologies to unlock something?
here is the simple code that needs to be in .lua file:

table.insert(data.raw["technology"]["NAME-processing"].effects,{type = "unlock-recipe",recipe = "RECIPE-NAME"})

replace NAME with the ore you want to use (for example, gold) and replace RECIPE-NAME with your internal recipe name

Have fun,

Dysoch, MagicLegend, Odin_Spain, McGuten, bobingabout
