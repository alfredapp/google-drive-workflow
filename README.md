# Alfred Workflow for Google Drive

List File Stream contents from Google Drive

## Instructions

An interim Workflow to bridge the gap until (if) Google Drives fixes the situation of files not being indexable by Spotlight (and thus Alfred).

Before your first use, run `:gdlaunchd` and wait for the notification. The more files you have, the longer the wait. It can take several minutes to finish building the cache. A macOS launchd agent will be loaded to do it daily (running `:gdlaunchd` again removes it).

To rebuild the cache on demand, do `:gdrebuildcache`.

When done, call `gd` and type to filter the contents of your Google Drive. `gdf` limits the search to directories.

The Workflow Environment Variables have defaults which will work for most. You only have to mess with them if you have an atypical setup.

* `google_drive_path`: The location of Google Drive on your file system. Can take multiple paths separated by commas.
* `ignore_list`: A comma-separated list of keywords to ignore. If any appears in a path, it will not be saved to your cache.
* `result_limit`: How many entries to show in Alfred.

## Download

[Get the latest release.](https://github.com/alfredapp/google-drive-workflow/releases/latest/download/Google.Drive.alfredworkflow)

## License

To be determined
