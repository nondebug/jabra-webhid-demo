# WebHID demo for the Jabra Evolve 40 USB headset

A demo that connects to a Jabra USB headset. The demo is designed to work with a Jabra Evolve 40 but may work with other Jabra headsets that share the same reports.

[WebHID API specification](https://wicg.github.io/webhid/index.html)

[Jabra HID usb.org specification](https://developer.jabra.com/site/global/sdks/web/documentation/index.gsp)

Jabra Evolve 40 is a stereo headset with a separate control unit. The control unit has 5 buttons which send HID input reports when pressed. The headset and the control unit have LEDs that can be turned on and off with HID output reports.

[Jabra Evolve 40 product page](https://www.jabra.com/business/office-headsets/jabra-evolve/jabra-evolve-40)

## Browser requirements

WebHID is available in Chrome 78+ behind a flag. To use WebHID, navigate to chrome://flags in a browser window and enable "Experimental Web Platform Features", then restart Chrome.

## Usage

* Plug the Jabra headset into a USB port.
* Open the [demo page](https://nondebug.github.io/jabra-webhid-demo/) and click the Connect button.
* In the device chooser dialog, select "GN Netcom A/S Jabra EVOLVE LINK" and click Connect.
* Check that a "Connected to device" message is displayed.

After connecting to the headset, try clicking the "Pick Up" button to send an output report. This will cause LEDs to light up on the headset and control unit. The headset should respond with HID input reports. You can also press buttons on the control unit to cause the headset to send HID input reports.
