## Microsoft Open Source Code of Conduct

### Product Tree

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

### Configuration

#### DocFX

```
"< contososerver-2.0": { 
  "dest": "legacy",
  "toc_rel": "legacy/toc-different.yml"
}, 
">= contososerver-2.0 || >= contosoclient-1.0": { 
  "dest": "active" 
}
```

#### Content

* index.md - Available for all monikers in folder.
* overivew.md - Available for all monikers in folder; configured with moniker zones and shared content.
* Quick Starts - Folder should have at least one item available for all monikers.
  * quick-start-1.md - Available only for some monikers; configured through file-level metadata.
  * quick-start-2.md - Available only for some monikers; configured through file-level metadata.
* Tutorials - Folder should have at least one item available for all monikers.
  * tutorial-1.md - Available for some monikers; All content in zones. No shared content. Purposefully left out file-level metadata.
  * tutorial-1.md - Available for some monikers; All content in zones. No shared content. Purposefully left out file-level metadata.