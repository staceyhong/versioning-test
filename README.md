# Versioning Test

## Product Tree

* Contoso Platform (Family)
  * Contoso Server (Product)
    * contososerver-1.0
    * contososerver-1.1
    * contososerver-1.2
    * contososerver-2.0
    * contososerver-2.1
  * Contoso Client (Product)
    * contosoclient-1.0
    * contosoclient-2.0

## Configuration

### OPS

The moniker ranges under which content is published are:

* `< contososerver-2.0`
* `>= contososerver-2.0 || >= contosoclient-1.0`

### DocFX

The docfx.json file maps content from the legacy and active folders into similarly named groups. These groups are then mapped to the published moniker ranges as follows:

* `< contososerver-2.0` maps to the `legacy` folder
* `>= contososerver-2.0 || >= contosoclient-1.0` maps to the `active` folder

## Content

The content has been created to model various scenarios that are expected to appear in real docsets.

* index.md - Available for all monikers in folder.
* overivew.md - Available for all monikers in folder; configured with moniker zones and shared content.
* quickstarts - Folder should have at least one item available for all monikers.
  * quick-start-1.md - Available only for some monikers; configured through file-level metadata.
  * quick-start-2.md - Available only for some monikers; configured through file-level metadata.
* tutorials - Folder should have at least one item available for all monikers.
  * tutorial-1.md - Available for some monikers; All content in zones. No shared content. Purposefully left out file-level metadata.
  * tutorial-1.md - Available for some monikers; All content in zones. No shared content. Purposefully left out file-level metadata.
* samples - Folder will be removed for some monikers.
  * sample-1.md - Available for some; configured through file-level metadata.
  * sample-2.md - Available for some; configured through file-level metadata.
* concepts - Folder will be removed for some monikers
  * sub-concepts - Folder will be removed for some monikers
    * sub-concept-1.md - Available for some; configured through file-level metadata.
    * sub-concept-2.md - Available for some; configured through file-level metadata.
  * concept-1.md - Available for some; configured through file-level metadata.
  * concept-2.md - Available for some; configured through file-level metadata.
* reference - TODO: demo with includes
* resources - TODO: demo with content that nests moniker ranges, e.g. block quotes and tabs