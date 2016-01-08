# MiniZinc package for Sublime Text

Syntax highlighting for the MiniZinc modelling language (.mzn and .dzn files). Here's what it looks like:

![alt text](https://cloud.githubusercontent.com/assets/7506161/12205405/b5dfdfee-b63a-11e5-9d95-a86d1aa3c664.png "MZN with Cobalt color scheme")

![alt text](https://cloud.githubusercontent.com/assets/7506161/12205420/d04a3d8e-b63a-11e5-8a3e-60238f1f700b.png "MZN with Neon color scheme")

## Installation

Copy the MZN.* files into the Sublime Text "Packages" direcory.  This can be done either by cloning this repository, or by downloading the zip file.  The packages location can be found via `Preferences` -> `Browse Packages...`, or as follows:

* OS X:
    `~/Library/Application Support/Sublime Text 3/Packages/`
* Linux:
    `~/.Sublime Text 3/Packages/`
* Windows:
    `%APPDATA%/Sublime Text 3/Packages/`

Alternatively, navigate to the "Packages" directory and clone the git repository.

## About MiniZinc

MiniZinc is a medium-level constraint modelling language. It is high-level enough to express most constraint problems easily, but low-level enough that it can be mapped onto existing solvers easily and consistently. It is a subset of the higher-level language Zinc.

MiniZinc is available from http://www.minizinc.org/

## Features

This package adds syntax highlighting for all built-in functions and global constraints, as well as strings, numeric values, constants and keywords.

Comments are also highlighted. In MiniZinc, line comments are started by `%`, and block comments are enclosed in `/*` `*/`.

A very simple build system is also included.  To solve a model, `Ctrl-B` (or `Cmd-B` on OS X) invokes the `minizinc` program on the current model file.  However, do note that external data files cannot currently be specified in this build system.  It also requires that `minizinc` is visible to Sublime Text, which may not be the case in the default installation depending on your system.  Finally, the build system also does not allow changing any command line parameters or changing solvers.  But for very simple models it works.

## License

Copyright (c) 2015-2016 Andreas Stenmark

This is free software. It is licensed under the MIT License. Feel free to use this in your own work. However, if you modify and/or redistribute it, please attribute me in some way, and it would be great if you distribute your work under this or a similar license, but it's not required.
