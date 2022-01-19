# <img src='Workflow/icon.png' width='45' align='center' alt='icon'> Google Drive Alfred Workflow

List File Stream contents from Google Drive

## Instructions

An interim Workflow to bridge the gap until (if) Google Drives fixes the situation of files not being indexable by Spotlight (and thus Alfred).

Before your first use, run `:gdlaunchd` and wait for the notification. The more files you have, the longer the wait. It can take several minutes to finish building the cache. A macOS launchd agent will be loaded to do it daily (running `:gdlaunchd` again removes it).

![](https://i.imgur.com/oLz8iB3.png)

To rebuild the cache on demand, do `:gdrebuildcache`.

When done, call `gd` and type to filter the contents of your Google Drive. `gdf` limits the search to directories. Use ↵ to open the path, ⌥↵ to reveal it in the Finder, or ⇧↵ to search it in the web browser.

![](https://i.imgur.com/yuv4rEy.png)

![](https://i.imgur.com/5hNOPzs.png)

The Workflow Environment Variables have defaults which will work for most. You only have to mess with them if you have an atypical setup.

* `google_drive_path`: The location of Google Drive on your file system. Can take multiple paths separated by commas.
* `ignore_list`: A comma-separated list of case-sensitive keywords to ignore. If any appears in a path, it will not be saved to your cache. Wildcard characters are interpreted.
* `result_limit`: How many entries to show in Alfred.

`!gddiagnostic` inspects the current Workflow configuration. It is to be run when asking for help.

## Download

[Get the latest release.](https://github.com/alfredapp/google-drive-workflow/releases/latest/download/Google.Drive.alfredworkflow)

## License

3-Clause BSD
