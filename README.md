# armadillo1_navigation_upgrade
Additional config for armadillo1 navigation

## runing

* in order to use dynamic reconfiguration for move_base, use the following commands:

for the real robot use:
```bash
$ roslaunch armadillo2_navigation_upgrade armadillo1.launch lidar:=true amcl:=true have_map:=true map:="<paht_to_map>/<map_name.yaml>" move_base:=true
```

to navigate through doors, use:
```bash
$ rosrun dynamic_cfg move_base_pass_through_doors.py
```

for basics configuration, use:
```bash
$ rosrun dynamic_cfg move_base_basic.py
```
