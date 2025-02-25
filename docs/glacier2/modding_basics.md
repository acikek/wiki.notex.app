---
sidebar_position: 3
description: A walkthrough of Glacier 2 and modding.
---

# Glacier 2 Modding Basics

## Background

The Glacier 2 Engine is a custom-built, private piece of software developed by IOI for the main purpose of running Hitman games. What is known about the engine is a result of reverse-engineering the files provided to the community via the game itself.

## Game Assets

In order to understand the basics of Glacier 2 modding, there are a few core concepts to grasp. First, navigate to the Hitman 3 game directory.

The `Runtime` folder contains files with the `rpkg` file extension. These are the game's assets, listed in a set order and separated by chunks. For example, `chunk0` contains the global assets used in all of the game's missions. You can view what each chunk represents [here](https://wiki.notex.app/glacier2/chunkdata).

> **Note**: You may also notice chunk "patch" files corresponding to the chunk files. These are updates to the original files. You'll be using chunk patches to mod the game.

`rpkg` files contain unique asset types within them. Assets contained in these files have a hash (an alphanumeric sequence generated from the asset's name) and the asset data itself. You can view the different file formats names and their details [here](https://wiki.notex.app/glacier2/fileformats/).

Asset data formats are diverse, but both readable and editable when using the proper tools. To make sense of these files, download the fittingly-named `rpkg` tool [here](https://www.notex.app/rpkg).<sup>1</sup> Make sure you have the [.NET Framework](https://dotnet.microsoft.com/download/dotnet-framework) installed on your machine.

Also included in the `Runtime` folder is a `packagedefinition.txt` file. This file tracks the patches - updates and mod additions - to the game's content. The included file in a retail installation limits the amount of patches that the file can contain, so it itself also needs to be patched! You can find the patched version as well as a decoder and encoder [here](https://www.notex.app/tools/online/xtea).

## Using RPKG

todo

---
<sup>1</sup>Please, for the love of god, do not run the program directly from the ZIP file/7zip/whatever program you use.
