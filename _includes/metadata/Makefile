##
## Programmer:    Craig Stuart Sapp <craig@ccrma.stanford.edu>
## Creation Date: Thu Jun  8 19:45:08 PDT 2023
## Last Modified: Thu Jun  8 19:45:11 PDT 2023
## Syntax:        GNU Makefile
## Filename:      _includes/metadata/Makefile
## vim:           ts=3:nowrap
##
## Description: Download metadata for the 1520s project from the Google Spreadsheet
##              for the project's metadata.  You need to update the SID variable below
##              when the deployment of the Google Apps Script has changed.
##
##              Type "make" in this directory to download the JSON files for the metadata.
##

SID = AKfycbxvTwAz1p_uYLUKK00MFpqLth2bAc5obeEGzBC-_FInT5ybUOl03F_p1Bc6PVmyNyklkw

all: download

download: works composers modern_editions

works:
	curl -L "https://script.google.com/macros/s/$(SID)/exec?sheet=works" > works.json

composers:
	curl -L "https://script.google.com/macros/s/$(SID)/exec?sheet=composers" > composers.json

modern_editions:
	curl -L "https://script.google.com/macros/s/$(SID)/exec?sheet=modern_editions" > modern_editions.json