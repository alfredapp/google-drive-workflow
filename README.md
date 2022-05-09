# <img src='Workflow/icon.png' width='45' align='center' alt='icon'> Google Drive Alfred Workflow

List File Stream contents from Google Drive

<a href='https://github.com/alfredapp/google-drive-workflow/releases/latest/download/Google.Drive.alfredworkflow'>⤓ Download Workflow</a>

## About

<!-- BEGIN ABOUT -->

An interim Workflow to bridge the gap until (if) Google Drive fixes the situation of files not being indexable by Spotlight (and thus Alfred).

Call `gd` and type to filter the contents of your Google Drive. `gdf` limits the search to folders.

![](https://user-images.githubusercontent.com/1699443/167266488-61a6f874-4f6c-41fb-a2f4-2c359ed429a0.png)

![](https://user-images.githubusercontent.com/1699443/167266492-26ab7d8c-536c-4c0a-ab3f-4639f3d24d54.png)

↵ opens the path; ⌥↵ reveals it in the Finder; ⇧↵ searches for it on Google Drive’s website.

You’ll be asked to build the cache on your first run. A notification will show when it’s ready. The more files you have, the longer the wait. A macOS launchd agent will be loaded to do it daily and on boot.

To rebuild the cache on demand, run `:gdrebuildcache`.

The File Actions make it straightforward to copy and move files to a Google Drive folder.

![](https://user-images.githubusercontent.com/1699443/167266470-cca9430b-4255-46b8-a772-d4253e5a01f2.png)

The Workflow Environment Variables have defaults which will work for most. You only have to mess with them if you have an atypical setup.

* `auto_refresh`: Enable (`1`) or disable (`0`) automatic cache rebuilding.
* `google_drive_path`: The location of Google Drive on your file system. Can take multiple paths separated by commas.
* `ignore_list`: A comma-separated list of case-sensitive keywords to ignore. If any appears in a path, it will not be saved to your cache. Wildcard characters are interpreted.
* `result_limit`: How many entries to show in Alfred.

`!gddiagnostic` inspects the current Workflow configuration. It is to be run when asking for help.

<!-- END ABOUT -->

<a href='https://github.com/alfredapp/google-drive-workflow/releases/latest/download/Google.Drive.alfredworkflow'>⤓ Download Workflow</a>
