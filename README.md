# NVidia-Run

This script runs the given command forcing it to use the NVidia GPU for graphics.

This helps with running X11/XWayland programs on dual GPU setups (e.g. Intel + Nvidia Optimus) with proprietary NVidia drivers.
Without the correct environment variables set, programs oftem fall back to integrated Intel GPUs.

Install:
```sh
chmod +x ./nvidia-run
sudo cp ./nvidia-run /usr/bin
```

Usage:
```sh
nvidia-run COMMAND
```

Example:
```sh
nvidia-run glxgears -info

nvidia-run java -jar some-minecraft-launcher.jar
```
