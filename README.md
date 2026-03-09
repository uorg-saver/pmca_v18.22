# pmca_v18.22

### Mirror links for PMCA v18.22

- These are the mirror links for this awesome [projects](https://github.com/ma1co/Sony-PMCA-RE).
- Fortunately, they works for my Sony a6400 in August 2023.
- You can also see [this](https://youtu.be/BJhheKXs39A) video for visual steps by steps guide.
Hope it helps.

---

### For those who have an A7III / ILCE-7M3 / A7M3 and struggled to unlock the video recording limit on firmware 4.01 (https://github.com/ma1co/Sony-PMCA-RE/issues/526#issuecomment-2726482113):

1. Download the older [Zadig 2.7](https://github.com/pbatard/libwdi/releases/download/v1.4.1/zadig-2.7.exe). This is **essential**, as it installs the libusb-win32 driver with version 1.2.6.0
2. Use the pmca-gui v18-22-ga82f5ba.exe file, NOT the v18 in the releases on this repo, as the one on this repo will not offer you the service mode tweaking, which is required for the A7III.
3. Once the camera is put into service mode, you will see a device in Zadig called "Sony USB device". If not already done, you also need install the libusb-win32 v1.2.6.0 driver here too.
4. If at any point you have used another version of zadig, it is likely you have a newer version of libusb installed like 1.4.0.0, which is incompatible. You need to connect the camera, and uninstall and delete the newer driver, then reboot. Connect the camera again and check that the newer driver has been removed. Then reinstall the 1.2.6.0 driver.
5. If at any point you need to force the camera to enter (and STAY) in service mode, so you can uninstall/install drivers for the Sony USB device, you can use the command prompt version of PMCA with command "pmca-console.exe serviceshell" to enter service mode.
