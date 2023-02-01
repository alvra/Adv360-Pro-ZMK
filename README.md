# ADV360-PRO-ZMK

## Customize firmware

1. Modify `adv360.keymap1` or `macros.dtsi`.

## Build firmware in GitHub Actions

1. Push a commit to trigger the build action.
2. Download the artifact.

## Build firmware locally in a container

Either Podman or Docker is required, Podman is preferred if both are present.\
Make is also required

1. Execute `make`.
2. Check the `firmware` directory for the latest firmware build.

The built docker container and compiled firmware files can be deleted with `make clean`.

## Flash firmware

1. Connect the left module via USB.
2. Mount the left module for update: `Mod` + `①`.
3. Install the left module firmware by copying the `left.uf2` file to the mounted drive.
4. Wait for the installation to complete.
5. Do the same thing for the right module using: `Mod` + `③`.

## Other support

Further support resources can be found on Kinesis.com
https://kinesis-ergo.com/support/kb360pro/#firmware-updates
https://kinesis-ergo.com/support/kb360pro/#manuals
