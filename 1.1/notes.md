# HKI update 1.1

# Changes:
- fixed issue on the frontpage where clicking on the lights would not take you to the lights view

## How to update?
Changed files are sorted through their respective lovelace folders. Only the files listed here have changed!

### Method 1:
if you haven't changed any code in the following files you can simply copy/paste and overwrite the old one.

### Method 2:
if you did make changes? please do the following changes in the following files:
- in `lovelace/views/00.frontpage.yaml` change the path `/lovelace/light` to `lovelace/lights` on line 74.
