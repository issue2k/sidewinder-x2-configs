# sidewinder-x2-configs
My artillery sidewinder x2 configs

## Build and flash marlin firmware

### build

- Check out https://github.com/markrossington/sidewinder-x2-marlin
- Replace config files with the ones placed in marlin/
- Update marlin version commit in scripts/settings.py:

```marlin_version = "1c119e9fa69773a98af43d538b5b94359a44323b"  # Use latest 2.1.x```

- run python3 scripts/marlin_build.py

### flash

```sudo dfu-util -a 0 -s 0x8000000:leave -D output/firmware.bin```
