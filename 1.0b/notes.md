# HKI update 1.0b

## Changes:
- fixed issue on the frontpage where clicking on the lights would not take you to the lights view
- fixed comments on how to remove the third person on the frontpage
- fixed 3 dots in the footer, they are now hidden
- removed secrets from `global_config.yaml` (when left unchanged lovelace would not load)
- bumped version to 1.0b

## How to update?
Changed files are sorted through their respective lovelace folders. Only the files listed here have changed!

### Method 1:
if you haven't changed any code in the following files you can simply copy/paste and overwrite the old one, files listed here are sorted in the same structure as the full setup to make copy/pasting easy

### Method 2:
if you did make changes? please do the following changes in the following files:
- in `lovelace/views/00.frontpage.yaml` change the path `/lovelace/light` to `lovelace/lights` on `line 74`.
- in `lovelace/views/00.frontpage.yaml` change line 44 to have the correct description (line 44 to 49). This is a comment, you do not need to do this if you know how to edit lovelace yourself.
- in `lovelace/views/menu.yaml` change the version number to 1.0b (not required, but certainly helps if you ask me for support if I know which version you are running)
- copy/paste the `lovelace/views/about.yaml` view and overwrite your old one
- copy/paste `lovelace/custom_header/custom_header.yaml` file and overwrite your old one
