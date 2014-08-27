## About
Create xml file and send it to UMS to create/update content for particular subnetwork/profile.

## Install
* ant
* curl

## Getting Started
- Currently only *intcar.content.tpl.xml* with content of INTCAR NG exists
- Copy _settings.properties to settings.properties
- In settings.properties: change uid, pwd, subnetwork, profile to appropriate values
- optional: Open intcar.content.tpl.xml and comment in *update_if_exists* tag for particular content if it should be replaced
- Run *ant*
  * intcar.content.xml will be created and send to UMS
  * Log file *ums-output.log* will be created
- Check UMS Backend

If tag *update_if_exists* is used, UMS searches for content  by insert_content.name tag.


## Debug
To debug run *ant -debug*.

