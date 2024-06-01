# unraid_pause_docker_parity_check
Script that checks if unraid is running a parity check and pauses containers if yes.

## Logic:
```
if parity check = yes
then pause defined docker containers
```
```
if parity check = no
then check if container is paused and resume (Can disable if you want to restart manually)
```

## Considerations:
-Does not consider if parity check is paused
-A paused parity will trigger the script
-no logic in place to account for if you paused the container manually, it will unpause any paused container on the list

V0.9
Initial Commit
