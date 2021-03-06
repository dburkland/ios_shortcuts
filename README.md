README
=========

The Tesla legacy shortcuts were created based on the excellent examples shared by u/jn1cks of reddit.com in this post: https://www.reddit.com/r/teslamotors/comments/ahe5be/i_created_a_siri_shortcut_that_wakes_up_my_tesla/. 

In order to import the shortcuts, you will first need to allow the import of untrusted shortcuts. This can be done by completing the steps documented [here](https://9to5mac.com/2019/08/14/allow-untrusted-shortcuts-ios-13/). You can then click on the link next to "Download Latest Legacy Tesla Shortcuts" to download & install the shortcut downloader. With the shortcut downloader installed please execute it via the Shortcuts app to download each of the shortcuts. Once each shortcut has been imported into the Shortcuts app on your device, you will then need to execute the "Generate Tesla Token" shortcut. This results in the creation of an authentication token that is used to communicate with your car. Once that is complete you can then execute any of the other Tesla shortcuts.

Tesla Legacy iOS Shortcut Inventory:

* [Download Latest Legacy Tesla Shortcuts](https://www.icloud.com/shortcuts/95ce55d2e76749ad941248dffa15c376)
  * Allows you to download each of the published Tesla legacy shortcuts, right from the Shortcuts app.
  * NOTE: Anytime a new version of the Tesla legacy shortcuts is released you simply need to re-run this shortcut and re-download the appropriate shortcut(s) replacing the existing copies.

* Generate Tesla Token
  * Generates an authorization token from the captured Tesla.com credentials
  * NOTE: This shortcut needs to be executed at least every 45 days since the tokens automatically expire.
  * RECOMMENDATION: Set a reminder in your favorite calendaring or task app with the "workflow://run-workflow?name=Generate_Tesla_Token" link in the notes section.

* Actuate Frunk
  * Wakes the vehicle (if needed) and actuates the frunk

* Actuate Trunk
  * Wakes the vehicle (if needed) and actuates the trunk

* Turn On HVAC Normal
  * Wakes the vehicle (if needed), turns on the HVAC system, and sets the temperature to 67 degrees Fahrenheit

* Turn On HVAC Max
  * Wakes the vehicle (if needed), turns on the HVAC system, sets the temperature to 82 degrees Fahrenheit, and turns on the driver's seat warmer

* Turn Off HVAC
  * Wakes the vehicle (if needed) and turns off the HVAC system

* Lock Doors
  * Wakes the vehicle (if needed) and locks the doors

* Unlock Doors
  * Wakes the vehicle (if needed) and unlocks the doors

* Turn On Sentry
  * Wakes the vehicle (if needed) and turns on Sentry Mode

* Turn Off Sentry
  * Wakes the vehicle (if needed) and turns off Sentry Mode

* Vent Windows
  * Wakes the vehicle (if needed) and vents the windows

* Close Windows
  * Wakes the vehicle (if needed) and closes the windows

* Set Charge Limit
  * Wakes the vehicle (if needed) and sets the charge limit to the user-selected percentage.

* Open Charge Port Door
  * Wakes the vehicle (if needed) and opens the charge port door

* Close Charge Port Door
  * Wakes the vehicle (if needed) and closes the charge port door

* Start Charging
  * Wakes the vehicle (if needed) and starts charging

* Stop Charging
  * Wakes the vehicle (if needed) and stops charging

* Honk Horn
  * Wakes the vehicle (if needed) and honks the horn

* Flash Lights
  * Wakes the vehicle (if needed) and flashes the lights
  
### FAQs

* What can you do if you receive error messages like this one: ![](https://pbs.twimg.com/media/EHQXnncXYAEvPbZ?format=jpg&name=medium)
  * Delete the "Generate Tesla Token" shortcut and re-import it.
  * Execute the re-imported "Generate Tesla Token" shortcut, this time making sure to select "Allow" when prompted.
  * Re-run the Tesla shortcut that you originally tried to execute.
* How can I call these shortcuts using "Hey Siri"?
  * The name of the shortcut is automatically setup as the voice command phrase that Siri recognizes. 
  * If you would prefer another shortcut voice command phrase, you can simply rename the shortcut (after it is imported) in the Shortcuts app to whatever you like.
  * Once the shortcut is named appropriately, simply say "Hey Siri <Name of Shortcut>".
  * NOTE: Please keep in mind that the shortcut name must be unique from other shortcuts in your library. As an example, I tried to rename **Turn on HVAC Normal** to **Turn on Heat**, but that command is associated with HomeKit so it doesn't work. **Turn Heat On** however works perfectly fine.
* How secure are these shortcuts?
  * The authentication token that is generated by the "Generate Tesla Token" shortcut is stored in your personal iCloud Drive. The shortcut is only visible to apps or services that have access to your iCloud drive meaning folks cannot publicly access this data by default. 
  * Each of the shortcuts leverage TLS when communicating with Tesla just like the official Tesla app
  * I do not log or record any usage data, nor do I log or record any of the generated Tesla API tokens.

