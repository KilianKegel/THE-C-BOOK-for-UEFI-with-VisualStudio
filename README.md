# THE C BOOK — reloaded with Microsoft Visual Studio

Build sample programs from my first C book, [THE C BOOK](https://publications.gbdirect.co.uk/c_book/) by 
[Mike Banahan](https://www.linkedin.com/in/mike-banahan-60a548/), [Declan Brady](https://www.linkedin.com/in/declantbrady/), and [Mark Doran](https://www.linkedin.com/in/mark-doran-81ba3281/).

The book was published in 1991 and is now [available for free](https://publications.gbdirect.co.uk/c_book/copyright.html).<br>

<p align="center">
	<img src="https://github.com/KilianKegel/4KPages-THECBOOK/blob/main/images/THECBOOK_FFF.jpg" width="300" height="439">
</p>

[Full copy of the original book is here.](https://github.com/KilianKegel/4KPages-THECBOOK/blob/main/README.md#4kpages-thecbook)

## Intention
1. Demonstrate that UEFI applications can be developed without **EDK2/tianocore** build environment.
2. Get the **THE C BOOK** sample programs running on **UEFI**
3. Get the **THE C BOOK** sample programs running on **Windows 64-bit**
	* demonstrate the full-blown debug capabilities with Visual Studio in the Windows environment
	* enable debugging through the entire source code including the [C-Library](https://github.com/KilianKegel/toro-C-Library?tab=readme-ov-file#toro-c-library-formerly-known-as-torito-c-library) [source code](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI) used here
4. Demonstrate the portability of the sample programs to different platforms
5. Make clear that **cross-platform-development** is:<br>
   **A very strong feature to develop, debug and maintain** ***big and complex software projects*** **for platforms with very limited development capabilities, like** ***UEFI***

## Approach
Use the *monolithic* Standard C Library [**toro C Library**](https://github.com/KilianKegel/toro-C-Library?tab=readme-ov-file#toro-c-library-formerly-known-as-torito-c-library).
This library is a C90-compatible clone of the original Microsoft C Library LIBCMT.LIB
and integrates seamlessly into the Visual Studio environment. 
It is used to develop for **UEFI** and **Windows** targets.

[License](https://github.com/KilianKegel/toro-C-Library?tab=License-1-ov-file)

The source code of [**toro C Library**](https://github.com/KilianKegel/toro-C-Library?tab=readme-ov-file#toro-c-library-formerly-known-as-torito-c-library) is
provided under the **GNU General Public License v3.0** [here](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI).

## Howto
1. install Microsoft Visual Studio 2022 on your Windows 64-bit machine: https://github.com/KilianKegel/Howto-setup-a-UEFI-Development-PC?tab=readme-ov-file#install-visual-studio-2022
2. get entire project from here: https://github.com/KilianKegel/THE-C-BOOK-for-UEFI-with-VisualStudio
3. open the solution file **Visual-THE-C-BOOK-for-UEFI.sln** in Visual Studio 2022

**ATTENTION:** Sample programs rely on ASCII character set. UEFI UNICODE files can't be handled.

## Revision history
### 20250906
* support **VS2022 v17.14**
    * update **toro C Library 20250906, v0.9.6 Build 757**
### 20241031
* add C Library sourcecode
### 20240922
* Initial release
