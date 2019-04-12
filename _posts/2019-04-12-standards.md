---
layout: post
permalink: /standards
title: "Standards"
date: 2019-04-12
---

A full documentation of the standards can be found at [https://github.com/gm4-consortia/standards](https://github.com/gm4-consortia/standards)

-----

## General

### File Content Standard

**Standard ID** `GEN:0001-r1`  
**Base Numerical ID** `0001`  
**Location** `general/0001-r1.md`  
**Effects** `General`  
**Last updated** `2019-04-11`

#### Overview
1. File Content Standard (`GEN-0001`) lays out the format for the content in the files for all standards.
2. All standard files state what category they affect.
3. The standard number is based off of what category is affected.
4. Both `Overview` and `Technical Information` follow the format of an indent for each sub-note.
5. Every standard documentation terminates at `END OF STANDARD`.
5. This layout must be followed in every standard's documentation.


#### Technical Information
1. Standard Number [`O2`]
   1. The first three letters define the area of effect
      1. `GEN` for General
      2. `NET` for Nether
      3. `END` for The End
      4. `OVR` for Overworld
      5. `MDP` for Module Data Packs
      6. `GRP` for Global Resource Pack
      7. `GIT` for GitHub
   2. The standard ID after follows a 4-digit pattern
      1. Each iteration is sequential for each further addition starting at `0001`.
      2. The length of all IDs is 4.
      3. All other numbers are placeholdered with a 0 if unused - as in `0001` or `0274`.
2. Categories [`O2`-`O3`]
   1. In the template...
      1. Replace `category` with the full category name in lowercase-underscore format; for example, `general` or `the_end`.
      2. Replace `Category` with the full category name in upper-sentence case; for example, `General` or `The End`.
      3. Replace `CAT` with a category's ID (found at `T-1.1`).
      4. Replace `STID` with the standard's base numerical ID; for example, `0001` or `0274`.
      5. Replace `#` in `r#` with the standard's revision number
      6. Replace `#` in `O#` with the overview point number referenced
      7. Any file extensions (such as `.md`) or markdown formatting do not need to be changed
      8. Last updated date format follows [`ISO-8601`](https://en.m.wikipedia.org/wiki/ISO_8601)
3. Format layout [`O5`]
   1. The template can be found at `standards:master/template/standard.md`.
   2. Files are named `STID-r#.md` and formatted in markdown.

`END OF STANDARD`

-----

## Global Resource Pack

### File Structure and Content Standard

**Standard Number** `GRP:0001-r1`  
**Base Numerical ID** `0001`  
**Location** `global_resource_pack/0001-r1.md`  
**Effects** `Global Resource Pack`  
**Last Updated** `2019-04-12`

#### Overview
1. File Structure and Content Standard (`GRP-0001`) lays out the format for the contents and structure of files in the optional, `CustomModelData`-driven resource pack.
2. The resource pack is one pack for all Gamemode 4 modules.
3. All features must work in vanilla Minecraft.
	
#### Technical Notes
1. File structure [`O2`]
   1. All Gamemode 4 textures and models should be under the namespace `gm4`.
2. File content [`O2`]
   1. Models must...
      1. Be correctly formatted; not one-line.
   2. Textures must...
      1. Fit the vanilla 'feel'.
      2. Keep whatever resolution the affected file is by default; for example, blocks and items are 16x16.
      3. Be approved by the Gamemode 4 admins prior to addition.
   3. `CustomModelData`/`custom_model_data` values should be kept per-model; for example, if `Item A` has a CMD defined at 1, `Item B` can have a CMD defined at 1 as well, not 2.

`END OF STANDARD`
