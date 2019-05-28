# Release History

* 20190429, V0.9.15
    * Updated to homeduino@0.0.70 which bundles rfcontroljs and otat-repl. This version
      should solve issues with stray characters in input causing node.js to error
      with "Illegal Token" exception
    * Minor changes
    
* 20190426, V0.9.14
    * defunct - do not install
      
* 20190425, V0.9.13
    * Updated to homeduino@0.0.68 which includes updated rfcontroljs@0.0.59 and
      updated vhduino binary
    * Updated rfcontroljs version contains various fixes for shutter protocols and
      new switch protocols for Masterplug UK.
    
* 20190415, V0.9.12
    * Added xUpLabel, xDownLabel, xStoppedLabel extensions to HomeduinoRFShutter, issue #70
    * Only listen to "on" event on switch discovery to prevent invalid device 
      types, thanks @Wiebe Nieuwenhuis
    * Validity check on temperature and/or humidity to prevent invalid devices on 
      discovery, thanks @Wiebe Nieuwenhuis
    * Added battery indicator support for HomeduinoRFContactSensor
    * Added option "inverted" for HomeduinoRFContactSensor, thanks @Bernd Strebel
    * Added HomeduinoRFShutter rollingTime attribute to support moving shutter 
      by percentage, thanks @Michael Kotten
    * Updated to homeduino@0.0.67 which includes migration to serialport@6 for
      supporting newer Node.js version