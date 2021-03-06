# FictionBook Editor Changelog

## v.2.7beta1

* Drop Windows XP support
* High DPI fixes
* Use MUI as localization system
* Replace NuGet package system with Vcpkg. PCRE, Hunspell, Scintilla sources removed.
* Update Scintilla to v3.7.6
* Update PCRE to v8.41
* Update Hunspell to v1.6.1
* Use dynamic VCRuntime to reduce installation size and allow CRT updates via Windows Update

## v.2.6.13

* Fix v2.6.12 bug then document cannot be loaded and new images cannot be 
  inserted (issue https://github.com/evpobr/fictionbookeditor/issues/212)
* Source files converted to UTF8 to avoid various problems


## v.2.6.12

* File dialogs now are styled and look native under Windows XP and higher
* Fixed script bug https://github.com/evpobr/fictionbookeditor/issues/197

## v2.6.11

* Add thumbnail handler shell extension
* Use VS2017 compiler

## v2.6.10

* 64-bit FBShell build - now shell extension works under 64-bit OS. The installer will automatically install the correct version.
* FBE now uses MSXML 6.0 instead of 4.0. This version is default XML parser in WinXP SP3 and supported up to Windows 10.

## v2.6.9

* Fixed bug, introduced in 2.6.9 - FBE cannot find plugins

## v2.6.8

* Upgade Visual Studio solution and projects to VS2015 version;
* Add missing ExportHTML and FBV projects from [FBTools](https://haali.su/pocketpc/files/FictionBook%20Tools%20v2.0%20Setup.exe);
* Add missing files from FBE distribution (genres.txt_L, genres.rus.txt_L);
* Upgrade bundled [WTL v8.1](https://sourceforge.net/projects/wtl/) to v9.1 using [NuGet packaging system](https://www.nuget.org/). WTL sources are automatically restored when you build solution first time;
* Upgrade [PCRE v7.9](http://www.pcre.org/) to v8.37, PCRE is now build from sources;
* Upgrade [Hunspell](http://hunspell.sourceforge.net/) to v1.3.3, Hunspell is now build from sources;
* Fix installer to propertly work under Windows Vista and higher (set `RequestExecutionLevel` to `admin`);
* Remove references to [UAC plugin](http://nsis.sourceforge.net/UAC_plug-in) from installer, it's needed for Windows 2000 only, but we don't support it;
* Add version info to all exe's and dll's.