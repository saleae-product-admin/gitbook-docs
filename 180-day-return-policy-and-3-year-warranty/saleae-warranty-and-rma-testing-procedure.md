---
description: Saleae Warranty & RMA Testing Procedure
---

# Process a Warranty

### Troubleshooting Steps

If you believe your Logic hardware is broken, please perform the troubleshooting steps below so we can verify the source of the problem.

1. Test with the Latest Beta Software. Link: [Latest Beta Release](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/logic-software/latest-beta-release)
   * If you are running the standalone version of the Saleae software, you will need to manually install the drivers. To do that, follow these instructions: [Driver Install](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/logic-software/the-driver-wont-install)
2. Remove any USB hubs, laptop docking stations, and extension cables. Also, remove all other USB devices from your PC. Then, test the device directly on the PC, and on all other USB ports. Logic Pro 8 and Pro 16 require USB 3.0 ports.
3. Test Logic on a second PC.
   * If the second PC also fails to connect, then it is likely a hardware issue. If so, stop here and submit a [Warranty Request](https://goo.gl/forms/1NEjPF4g4eXeJnbf2). Otherwise, if it fails on one PC and works on another PC, then it is likely a PC issue. In this case, continue with the steps below.
4. Test with another USB cable
   * If another USB cable works, then your original USB cable may be faulty. If so, stop here and [Contact Support](https://support.saleae.com/hc/en-us/requests/new) for help. Otherwise, continue with the steps below.
5. Test if the VID and PID are correct. Instructions: [The Device's USB VID and PID Failed](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/troubleshooting/the-devices-usb-vid-and-pid-failed)
   * If the VID and PID are incorrect, then the hardware may be faulty. Stop here and submit an [Warranty Request](https://goo.gl/forms/1NEjPF4g4eXeJnbf2).
6. If you are troubleshooting Logic Pro 8 or Pro 16, ensure the latest USB 3.0 Host Controller is installed. Update the driver, if possible, and run the tests again. Link: [Latest USB 3.0 Host Controller Drivers](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/logic-software/latest-usb-3.0-host-controller-drivers)
   * The windows driver update check will NOT update USB 3.0 host controller drivers. These are not included in the Windows update driver database and must be manually updated.

### PC Detection Test

If the above steps did not resolve the issue, we need to determine if the PC can detect the Logic device:

1. Before connecting Logic to the PC, ensure the Saleae Software is **not running**.
2. Connect the device to the PC using the provided USB cable.
3. Check if the operating system \(OS\) detects the device:
   * **Windows:** Open device manager. Expand the section "Universal Serial Bus Controllers" and check for "Saleae Logic X USB Logic Analyzer" where "X" is the specific product version \(4, 8, Pro 8, etc.\). If "unidentified device" appears, then the OS did not detect it properly. If "Westbridge" appears, then there is a problem with the Saleae driver and you should follow the instructions here: [Driver Install](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/logic-software/the-driver-wont-install)
   * **Linux:** Run lsusb. Check for any device name containing "Saleae" or a VID of "0x21A9" or "0x0925". A complete list of VID and PID pairs can be found here: [The Device's USB VID and PID Failed](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/troubleshooting/the-devices-usb-vid-and-pid-failed)
   * **OSX:** Open "System Report" by opening the Apple menu and selecting "About this Mac," and then select "System Report...". Then select USB under Hardware and check for "Westbridge" in the treeview.
4. If the PC detects the Logic device properly, open the Saleae software. If the Saleae software reports \[Disconnected\] at the top, then the hardware is likely OK and this may be a software issue. Proceed to the troubleshooting steps here: [Troubleshooting the Software Connection to the Device](https://saleae.gitbook.io/docs/~/edit/drafts/-LJtrnKeYdvZQmbbuVU1/troubleshooting/troubleshooting-device-connection-2-software-connection-to-the-device)

### PC Fails to Detect Logic

If all tests above have failed, please submit a [Warranty Request](https://goo.gl/forms/1NEjPF4g4eXeJnbf2).

