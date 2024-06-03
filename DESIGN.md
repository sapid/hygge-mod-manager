# Goals:

- Warn when large changes are about to occur (e.g. change more than 30% by size)
- Run some executable afterward (e.g. a launcher)
- Pre-configure from text file

### Manager mode:
- Choose a storage provider
- Store authentication
- Choose a root directory
- Write a changelog
- Mark folders for sync
- - Pre-configured selections
- Mark files as config files 
- - Clients should grab if they don't exist; otherwise don't grab.
- - Sync if does not exist upstream. Otherwise, ignore changes.
- Save a hygge config file with upstream info
### Client mode:
- Choose an upstream location
- - Credentials if necessary
- Mark files as personally-managed (config)
- Display a changelog if changes occurred

# ToDo:
- Explain the name "hygge"
- Bundle rclone


# Backlog goals:
- Stash config changes
- - v1: Store a local copy of configs (e.g. move to `.backup`) then grab fresh upstream configs
- - v2: Show a diff between them and re-add any personal changes
- - v3: Support upstream config upgrades


# Dev goals:
These are just for my own education.

I'd like to use PyQt if possible, and I'd like to try out PyTest-qt for [ci/cd.](https://ilmanzo.github.io/post/testing_pyside_gui_applications/) Or, even better, [PySide6.QtTest](https://doc.qt.io/qtforpython-6/PySide6/QtTest/index.html)

