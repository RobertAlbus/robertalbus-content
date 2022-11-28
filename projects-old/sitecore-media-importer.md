@@@ PROJECT_TITLE
Sitecore CMS Media Importer
@@@

@@@ TAGS
C#, .NET Framework, Sitecore CMS
@@@

@@@ DESCRIPTION
Automation tool for the bulk-import of media assets to the CMS database
@@@

@@@ DISPLAY
true
@@@

This automation tool imports objects from the filesystem into a specific location in the Sitecore content tree. The existing import options for the CMS are somewhat limited, and this tool addresses some of these limitations. 

Notable features:
* Implements various flags to modify the import strategy
    * Overwrite DB objects if FS object is newer
    * Flat-structure import or maintain FS tree structure
    * Recursive
* Implements a custom Experience Ribbon section for integration into the existing CMS GUI
* Implemented as a Feature Module in accordance with Sitecore's Helix architectural principals
