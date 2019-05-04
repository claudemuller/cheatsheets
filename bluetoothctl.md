1. list - Generates a list of available controllers. You can pair a controller and a device while working from another controller, but on a home system you may have only one controller. However, you need the controller's MAC address to run other commands. If it is no longer visible on screen, run list again. You might be able to simplify the process by turning off all controllers except the one to pair.
2. show - Gathers information about available controllers, including their names and current state. This information can be useful for distinguishing one controller from the other.
3. select <CONTROLLER-MAC-ADDRESS> - Selects the controller to pair. Once you select the controller, all controller-related commands will apply to it for three minutes or until you select a new controller.
4. power on - Enables the selected controller. If you are pairing the controller on which bluetoothctl is running, this step is unnecessary.
5. agent on - Turns on Bluetooth support. If you use a USB adapter, it is on as long as it is plugged in.
6. default agent - Sets the current agent to the default.
7. discoverable on - Makes the controller visible to other devices. As a security precaution, run discoverable off after pairing.
8. scan on - Receives a list of detected devices (Figure 3). If a device you expect is not visible, check that it is turned on, ready to pair, and within range. Already paired devices will not be listed.
9. pairable on - Readies the controller for pairing. Remember that you have three minutes after running this command to pair.
10. devices - Lists available devices. You want the MAC address, not the name, to use with other commands.
11. info <DEVICE-MAC-ADDRESS> - Displays information about a particular device (Figure 4). This command is most often useful in identifying the correct device.
12. connect <DEVICE-MAC-ADDRESS> - Readies the device for pairing.
13. pair <DEVICE-MAC-ADDRESS> - Pairs the device with the default controller.
14. trust <DEVICE-MAC-ADDRESS> - Sets the device to re-pair automatically when it is turned on, which eliminates the need to pair all over again.
15. discoverable off
