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

#### Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.