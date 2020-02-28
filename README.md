The main goal of **OpenITI mARkdown** is to provide a simple system for tagging structural, morphological and semantic elements in premodern and early modern Islamicate texts of the [OpenITI corpus](https://github.com/OpenITI). The use of **OpenITI mARkdown** will allow one to engage in the computational analysis of texts in the same way as allowed by the more complex and time-consuming tagging schemes such as TEI XML; **OpenITI mARkdown** will also facilitate the conversion of the large volume of Islamicate texts into TEI XML, which is now the standard format for digital editions. In principle, **OpenITI mARkdown** does not require any special editor, but the current implementation relies on [EditPad Pro](https://www.editpadpro.com/), which supports right-to-left languages, Unicode, and large files. However, it is the support of custom highlighting and navigation schemes that makes this text editor particularly convenient for **OpenITI mARkdown**.

**OpenITI mARkdown** is not meant to be a comprehensive standard, but rather a light-weight tagging scheme that renders texts machine readable and can be adapted to specific research tasks. The scheme consists of a set of unified patterns, but also includes custom patterns that facilitate analysis of specific types of data. These patterns can be divided into structural (unified), morphological (unified, customizable) and semantic (unified customizable, but also custom). The scheme currently accommodates a variety of research inquiries. 

# A Very Brief Intro

Texts in **OpenITI** are automatically converted into **OpenITI mARkdown**, and in most cases, only structural tagging is required—in other words, tagging headers of chapters, sections,  subsections and and other logical units. 


1. Download and install [EditPad Pro](http://www.editpadpro.com/). **EditPad Pro** works on Windows only; if you are using Mac or Linux, you can still use it with some virtualization option; the combination of **Parallels**, **Windows 10** and **EditPad Pro** works well on Macs.
	1. **IMPORTANT!!!** Before you begin, make sure that EditPadPro is completely shut down, which must be done via *`FILE > Exit`* (not just click on the `x` in the top right corner, which does not properly shut down the program).
	2. Download **OpenITI mARkdown** schemes from GitHub:
		a. You can use the following link to download schemes for both EditPadPro 7 and EditPadPro 8: [https://github.com/OpenITI/mARkdown_scheme/archive/master.zip](https://github.com/OpenITI/mARkdown_scheme/archive/master.zip). You will need to unzip this file and then unzip the files with the desired scheme.
		a. Alternatively, you can download the file for a specific version of EditPadPro, which have the following filename pattern: `EditPadProV_YYYYMMDD_HHMMSS.zip`, where `V` is the version of EditPadPro (7 or 8), `YYYYMMDD` is the date (year, month, day), and `HHMMSS` is time (hour, minutes, seconds); `YYYYMMDD_HHMMSS` is a timestamp of when the version of mARkdown was generated. Fore example: `EditPadPro8_20200228_174919.zip`, `EditPadPro7_20200228_174919.zip`. If there are multiple files for the same version of EditPadPro, please, choose the latest one.
	3. Unzip the file with the mARkdown scheme (names like `EditPadProV_YYYYMMDD_HHMMSS.zip`) into a separate folder.
	4. Go into this new folder:
		- Select all files there (`Ctrl+a` on Windows; `Command+a` on Mac);
		- Copy the selected files into buffer (`Ctrl+c` on Windows; `Command+c` on Mac).
		- Double-click on the link `_Follow_this_link_to_paste_...` which will take you to a different folder
			- This link takes to `%APPDATA%\JGsoft\EditPad Pro 7` in case of EditPadPro7 and `%APPDATA%\JGsoft\EditPad Pro 8` in case of EditPadPro8
		- In that folder, paste copied files (`Ctrl+v` on Windows; `Command+v` on Mac).
	5. Now, open EditPadPro.		
		- If you done everything correctly, the background in EditPadPro should be of yellowish color
		- If the background is still white, you need to repeat the whole procedure; npow, make absolutely sure to shut down EditPadPro (*not just click on the `x` in the top right corner, but shut it down through `FILE > Exit`*), then repeat steps. 	
1. The scheme is automatically activated in EditPad Pro by the first line in the file, which must be: `#####OpenITI#` (called *magic value* in EditPad Pro).
1. Texts in the repositories of the [OpenITI Project](https://github.com/OpenITI) have already been preprocessed. Opening any of these texts in EditPad Pro should automatically activate **OpenITI mARkdown** scheme.
1. The tagging of structural elements of the text boils down to the following:
	1. the headers of chapters (`### |`), sections (`### ||`), subsections (`### |||`), etc. The entire text of a header must be on the same line (the entire text will be highlighted, if everything is correct).
	2. and information units: biographies (`### $`), descriptions of events (`### @`), and dictionary entries (also `### $`).
	3. If a structural/logical unit is tagged correctly, the color of the tagged unit will change accordingly.
1. Tagging must be done through the collation of the electronic text of a book with the printed edition on which the electronic text is based. Most editions can be easily found online as PDF files (‘googling’ the title—in the original language—usually brings up a lot of results; PDFs are most likely to be on [Archive.org](https://archive.org/)).

For more details on OpenITI mARkdown, see: [https://maximromanov.github.io/mARkdown](https://maximromanov.github.io/mARkdown)
