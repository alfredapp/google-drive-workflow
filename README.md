# <img src='Workflow/icon.png' width='45' align='center' alt='icon'> Google Drive Alfred Workflow

List File Stream contents from Google Drive

## Instructions

An interim Workflow to bridge the gap until (if) Google Drives fixes the situation of files not being indexable by Spotlight (and thus Alfred).

Call `gd` and type to filter the contents of your Google Drive. `gdf` limits the search to folders.

![](https://i.imgur.com/nBleTsJ.png)

![](https://i.imgur.com/5hNOPzs.png)

↵ opens the path; ⌥↵ reveals it in the Finder; ⇧↵ searches for it on Google Drive’s website.

You’ll be asked to build the cache on your first run. A notification will show when it’s ready. The more files you have, the longer the wait. A macOS launchd agent will be loaded to do it daily and on boot.

To rebuild the cache on demand, run `:gdrebuildcache`.

The Workflow Environment Variables have defaults which will work for most. You only have to mess with them if you have an atypical setup.

* `auto_refresh`: Enable (`1`) or disable (`0`) automatic cache rebuilding.
* `google_drive_path`: The location of Google Drive on your file system. Can take multiple paths separated by commas.
* `ignore_list`: A comma-separated list of case-sensitive keywords to ignore. If any appears in a path, it will not be saved to your cache. Wildcard characters are interpreted.
* `result_limit`: How many entries to show in Alfred.

`!gddiagnostic` inspects the current Workflow configuration. It is to be run when asking for help.

## Download

[Get the latest release.](https://github.com/alfredapp/google-drive-workflow/releases/latest/download/Google.Drive.alfredworkflow)

## License

3-Clause BSD
