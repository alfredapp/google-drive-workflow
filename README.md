# <img src='Workflow/icon.png' width='45' align='center' alt='icon'> Google Drive Alfred Workflow

List File Stream contents from Google Drive

<a href='https://alfred.app/workflows/alfredapp/google-drive'>⤓ Install on the Alfred Gallery</a>

> On Alfred 4 use <a href='https://github.com/alfredapp/google-drive-workflow/releases/download/2022.12/Google.Drive.alfredworkflow'>alternative link</a>

## Usage

Search the contents of your Google Drive via the Search Keyword (default: `gd`) or Folder Search Keyword (default: `gdf`).

![Alfred search for gd](Workflow/images/about/gd.png)

![Alfred search for gd fran](Workflow/images/about/gdfran.png)

* <kbd>⏎</kbd>: Open.
* <kbd>⌥</kbd><kbd>⏎</kbd>: Reveal in Finder.
* <kbd>⇧</kbd><kbd>⏎</kbd>: Search on Google Drive’s website.

You’ll be asked to build the cache on your first run. A notification will show when it’s ready. The more files you have, the longer the wait. A macOS launchd agent will be loaded to do it daily and on boot. If necessary, an immediate cache rebuild can be forced with the `:gdrebuildcache` keyword.

The [Universal Actions](https://www.alfredapp.com/help/features/universal-actions/) make it straightforward to copy and move files to a Google Drive folder.

![File Actions for Google Drive copy and mode](Workflow/images/about/fileaction.png)

To report a problem, run `!gddiagnostic`.
