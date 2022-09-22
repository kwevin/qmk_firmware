# Keychron K8 Pro

![Keychron K8 Pro](https://cdn.shopify.com/s/files/1/0059/0630/1017/t/5/assets/keychronk8proqmkviawirelessmechanicalkeyboardformacwindowsosaprofilepbtkeycapspcbscrewinstabilizerwithhotswappablegaterongpromechanicalswitchcompatiblewithmxcherrypandakailhwithrgbbacklightaluminumframe-1645094681965.jpg)

A customizable 87 keys TKL keyboard.

* Keyboard Maintainer: [Keychron](https://github.com/keychron)
* Hardware Supported: Keychron K8 Pro
* Hardware Availability: [Keychron K8 Pro QMK/VIA Wireless Mechanical Keyboard](https://www.keychron.com/products/keychron-k8-pro-qmk-via-wireless-mechanical-keyboard)

Make example for this keyboard (after setting up your build environment):

    make keychron/k8_pro/ansi/rgb:default

Flashing example for this keyboard:

    make keychron/k8_pro/ansi/rgb:default:flash

**Reset Key**: Connect the USB cable, toggle mode switch to "Off", hold down the *Esc* key or reset button underneath space bar, then toggle then switch to "Cable".

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).


# Full install instruction for (Windows)

Clone repository and navigate to bluetooth_playground branch

Install [QMK MSYS](https://msys.qmk.fm)
Install [QMK Toolbox](https://github.com/qmk/qmk_toolbox)

Open QMK MSYS
Navigate to cloned directory

    qmk setup
    qmk compile
    qmk clean -a
    make git-submodule
    make keychron/k8_pro/ansi/rgb:via
    
It should output a file in the current directory
Open QMK Toolbox
Follow instruction to enter DFU mode in [update Firmware](https://www.keychron.com/blogs/archived/k8-pro-factory-reset-and-firmware-flash)
flash the newly compiled file instead

Load the K8-Pro-Ansi-wMatrix.json for via

Done
