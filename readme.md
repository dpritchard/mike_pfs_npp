# mike_pfs_npp

## Overview

Very simple code folding and syntax highlighting in [Notepad++][npp] for files created by the [MIKE by DHI][mike] hydrodyanmic modelling software.  Currently auto-detects files with `.m21fm` and `.ecolab` extentions.  Requires [Notepad++][npp] (obviously).  Developed for MIKE 2011 but may work with other versions.  

## Usage

Notepad++ allows you to add new languages by adding language definitions to a userDefineLang.xml file. Add the MIKE_PFS definition like this:

1. Download the language definition file [userDefineLang.xml][direct_download] from GitHub to your computer.
2. Click Start > Run, and type (or paste in) `%APPDATA%\Notepad++`, then click OK.  This will open the settings directory for Notepad++.
3. If it does not already exist, copy the downloaded `userDefineLang.xml` file into the Notepad++ settings directory. Skip to step 7.
4. If it _does_ exist, open the active `userDefineLang.xml` with a text editor.
5. Copy the contents of the MIKE_PFS definition file between the `<UserLang>...</UserLang>` tags into the active `userDefineLang.xml`, at the end right before `</NotepadPlus>`.
6. Save `userDefineLang.xml`.
7. Restart Notepad++.

## Screenshot

![code_folding](https://raw.github.com/dpritchard/mike_pfs_npp/master/with_highlight_crop.png "Code folding in DHI PFS files!")

## Credit
Inspired by (and much of this readme stolen from) [thomsmits'][thomsmits] [markdown_npp][mdnpp] project.  

## Licence
Created by Daniel Pritchard (www.pritchard.co)  
Distributed under a creative commons CC BY-SA licence.  See here:  
http://creativecommons.org/licenses/by-sa/3.0/

[thomsmits]: https://github.com/thomsmits
[mike]: http://www.dhisoftware.com
[mdnpp]: https://github.com/thomsmits/markdown_npp
[direct_download]: https://github.com/dpritchard/mike_pfs_npp/blob/master/userDefineLang.xml
[npp]: http://notepad-plus-plus.org