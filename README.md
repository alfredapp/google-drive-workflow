# Alfred Workflow for Google Drive

List File Stream contents from Google Drive

## Instructions

An interim Workflow to bridge the gap until (if) Google Drives fixes the situation of files not being indexable by Spotlight (and thus Alfred).

Call `gd` and type to list and filter the contents of your Google Drive.

Before your first use, you will have to either run `:gdrebuildcache` or `:gdlaunchd`. The former builds a cache of your files on demand; the latter uses a macOS launchd agent to rebuild it every day (run `:gdlaunchd` again to uninstall it).

The Workflow Environment Variables have defaults which will work for most people. You will only have to mess with them if you have an atypical setup.

* `google_drive_path`: The location of Google Drive on your file system.
* `ignore_list`: A comma-separated list of keywords to ignore. If any appears in a path, it will not be saved to your cache.
* `result_limit`: How many entries to show in Alfred.

## Download

Find the Workflow under `Assets` [in the latest release](https://github.com/vitorgalvao/alfred-google-drive/releases/latest).

## License
