The main goal of **OpenITI mARkdown** is to provide a simple system for tagging structural, morphological and semantic elements in premodern and early modern Islamicate texts of the [OpenITI corpus](https://github.com/OpenITI). The use of **OpenITI mARkdown** will allow one to engage in the computational analysis of texts in the same way as allowed by the more complex and time-consuming tagging schemes such as TEI XML; **OpenITI mARkdown** will also facilitate the conversion of the large volume of Islamicate texts into TEI XML, which is now the standard format for digital editions. In principle, **OpenITI mARkdown** does not require any special editor, but the current implementation relies on [EditPad Pro](https://www.editpadpro.com/), which supports right-to-left languages, Unicode, and large files. However, it is the support of custom highlighting and navigation schemes that makes this text editor particularly convenient for **OpenITI mARkdown**.

**OpenITI mARkdown** is not meant to be a comprehensive standard, but rather a light-weight tagging scheme that renders texts machine readable and can be adapted to specific research tasks. The scheme consists of a set of unified patterns, but also includes custom patterns that facilitate analysis of specific types of data. These patterns can be divided into structural (unified), morphological (unified, customizable) and semantic (unified customizable, but also custom). The scheme currently accommodates a variety of research inquiries. 

# A Very Brief Intro

Texts in **OpenITI** are automatically converted into **OpenITI mARkdown**, and in most cases, only structural tagging is required—in other words, tagging headers of chapters, sections,  subsections and and other logical units. 


1. Download and install [EditPad Pro](http://www.editpadpro.com/). **EditPad Pro** works on Windows only; if you are using Mac or Linux, you can still use it with some virtualization option; the combination of **Parallels**, **Windows 10** and **EditPad Pro** works well on Macs.
	- Download **OpenITI mARkdown** schemes from GitHub using this link: [https://github.com/OpenITI/mARkdown_scheme/archive/master.zip](https://github.com/OpenITI/mARkdown_scheme/archive/master.zip).
	- the downloaded file should have the name `mARkdown_scheme-master.zip`. Unzip this file.
	- Within the unzipped folder, find the file with the name like `20190904_154432.zip` (which is the date of the creation of the file; if there are more than one, choose the latest one) and unzip it.
	- Within this new unzipped folder, select all the files and copy them into buffer (`Ctrl+c` on Windows; `Command+c` on Mac).
	- *Note*: **make sure that EditPad Pro is not running: you need to do `File > Exit` to completely shut it down.**
	- Now, final step, paste all the copied files from that folder into `%APPDATA%\JGsoft\EditPad Pro 7` (you can either paste this path into Explorer and hit `Enter`; or, you can double-click the shortcut *Follow_this_link_to_paste_mARkdownScheme* in the first unzipped folder.
	- When you open EditPadPro after this, the background in EditPadPro should be of yellowish color!
	- *Another note:* if the background is still white, you need to repeat the whole procedure; make sure to shut down EditPadPro (*not just click on the `x` in the top right corner, but shut it down through `FILE > Exit`*), then copy-paste the files of the scheme into folder `%APPDATA%\JGsoft\EditPad Pro 7`. 
	
1. The scheme is automatically activated in EditPad Pro by the first line in the file, which must be: `#####OpenITI#` (called *magic value* in EditPad Pro).
1. Texts in the repositories of the [OpenITI Project](https://github.com/OpenITI) have already been preprocessed. Opening any of these texts in EditPad Pro should automatically activate **OpenITI mARkdown** scheme.
1. The tagging of structural elements of the text boils down to the following:
	1. the headers of chapters (`### |`), sections (`### ||`), subsections (`### |||`), etc. The entire text of a header must be on the same line (the entire text will be highlighted, if everything is correct).
	2. and information units: biographies (`### $`), descriptions of events (`### @`), and dictionary entries (also `### $`).
	3. If a structural/logical unit is tagged correctly, the color of the tagged unit will change accordingly.
1. Tagging must be done through the collation of the electronic text of a book with the printed edition on which the electronic text is based. Most editions can be easily found online as PDF files (‘googling’ the title—in the original language—usually brings up a lot of results; PDFs are most likely to be on [Archive.org](https://archive.org/)).

For more details, see: [https://alraqmiyyat.github.io/](https://alraqmiyyat.github.io/)
