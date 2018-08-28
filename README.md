This is a switch-'port' of the webassembly-vm vmir (https://github.com/andoma/vmir)

The only changes that I had to make to get it to run on the switch was to change an open-flag which isn't present on the switch and get rid of the assumption that opening "/dev/stdout" will get a file-descriptor to stdout.

Right now this just executes the `test.wasm` file at the root of the sdcard and then prints some stats.