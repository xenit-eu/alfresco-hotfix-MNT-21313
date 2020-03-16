# Hotfix for Alfresco issue [MNT-21313](https://issues.alfresco.com/jira/browse/MNT-21313)

This project is a hotfix for issue [MNT-21313](https://issues.alfresco.com/jira/browse/MNT-21313)
 (upgrade pdf.js to v1.10.100) that still affects Alfresco 5.x and 6.x.

Alfresco 6.x will get an updated version of pdf.js in one of the next service releases.  
Merge requests for Alfresco 6.x.N have already been merged.
- [MNT-21313 - upgrade pdf.js to version 1.10.100 6.0.N #168](https://github.com/Alfresco/share/pull/168)
- [MNT-21313 - upgrade pdf.js to version 1.10.100 6.1.N #169](https://github.com/Alfresco/share/pull/169)
- [MNT-21313 - upgrade pdf.js to version 1.10.100 6.2.N #170](https://github.com/Alfresco/share/pull/170)

## Problem

Alfresco 5.x and 6.x are still using an older version of pdf.js; version 1.5.188 released on 2016-04-21.
Pdf.js is a popular library for rendering PDF documents. The latest version of pdf.js is version 2.2.228
 released on 2019-07-10. Version 2.2.228 contains a lot of improvements and bugfixes compared to v1.5.188.
For more details consult the [pdf.sj release log](https://github.com/mozilla/pdf.js/releases)

## Solution

For Alfresco 6.x.N the pdf.js library is updated to version 1.10.100 released on 2018-06-06.
Version 1.10.100 is the latest v1.x release of pdf.js.

This AMP overrides the pdf.js component files in Alfresco Share and updates them to version v1.10.100.

## Building and Installing

This project uses the [alfresco-gradle-sdk](https://github.com/xenit-eu/alfresco-gradle-sdk). Clone
this project and use `./gradlew amp` to build. Find the resulting AMP at `./build/dist/` and install
it into Alfresco Share.
