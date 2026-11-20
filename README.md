# Tab Archivist

A planned Chrome and Firefox extension that helps turn 1,200 open tabs into a manageable 150—without losing the pages you want to revisit.

Tab Archivist will archive tabs you are no longer using, close them to free browser resources, and let you find and restore them later.

## Project status

Initial project setup. The extension has not been implemented yet.

## Planned workflow

1. Review tabs that have been inactive for a chosen period.
2. Select tabs to archive, protecting pinned tabs and any tabs you exclude.
3. Save the archive successfully before closing the selected tabs.
4. Search the archive and restore individual pages or groups when needed.

The goal is to reduce active-tab clutter and resource use while keeping archived pages easy to recover. The number of remaining tabs should be a user preference, not a forced limit.

## Design priorities

- **Local storage by default:** browsing history and archived URLs stay on the device unless an optional feature explicitly says otherwise.
- **User control:** preview what will close, configure exclusions, and support manual archiving before introducing automatic rules.
- **Recoverability:** searchable archives, export/import, and clear feedback if saving an archive fails.
- **Large tab collections:** design and test for hundreds or thousands of tabs.
- **Chrome and Firefox:** investigate shared WebExtensions code and document browser-specific differences.

An archive initially means saving page URLs and tab metadata, not downloading complete offline copies of websites. Restoring a URL cannot guarantee recovery of unsaved forms, authentication state, or every page's prior in-memory state. Resource savings will depend on the pages and browser behavior.
