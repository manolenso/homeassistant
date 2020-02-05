## Homekit Infused v 1.1

The last few bugs are leaving HKI now and the RC tag is gone, thanks again for testing and see you soon!

#### Changes:
- Added several options for frontpage buttons/badges, fixed the 'C' that was shown on other sensors.
- Added a lock option to the thermostat buttons (this was a Feature Request)
- Added a new button template for use on the frontpage (see comments in `/global_config/views/frontpage_view.yaml` for examples)
- Edited thermostat button template and autofill climate template for use with locks
- All frontpage buttons now default to a simple button (if you want the badge please set that in the `/global_config/views/frontpage_view.yaml`file)
- Moved the `homekit_infused` folder to `packages/homekit_infused`. Some users had trouble setting up the HKI package with existing packages
- Removed duplicate keys from the HKI configuration.yaml file
- Shortened template code in HKI configuration.yaml

#### How to update?
You can ONLY update to this version if you come from the 1.0RC version (you will NOT be able to update from alpha/beta directly to this version)
Copy/Paste all the files from the [update](https://github.com/jimz011/homeassistant/tree/updates/1.0RC%20to%201.1) folder to the root of your setup.
Copy your `/homekit_infused/hki_groups.yaml` file to `/packages/homekit_infused/`, it will ask you to overwrite the old file, click yes.
In your `configuration.yaml` file edit the following lines and change it to:
```
homeassistant:
  packages: !include_dir_named packages/
```
Delete the old `/homekit_infused/` folder from the root of your setup as you no longer need that.

WARNING: the global_config files for both the climate_view and frontpage_view will be overwritten. If you have already configured those files please only copy the changes (use a decent code editor like VScode to compare the changes, usually this will be one or two lines at most!)

That's it folks, Enjoy!
