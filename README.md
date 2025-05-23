# AutoTF Documentation

## Info

This repo contains the documentation for the AutoTF systems as implemented and is still an active **Work-In-Progress**.

Be aware that the documentation might not reflect the actual code in every corner.

The documentation might lag behind a bit, because the safety and functionality of actively running systems is priorizied.


### **All info given in this repository are without warranty. AutoTF and individiuals representing AutoTF are not liable for any damanges occuring due to the contents unless specified otherwise in a contract.**


## LFS
Large files are hosted on the AutoTF Gitea instance at [lfs.autotf.de](https://lfs.autotf.de/admin/AutoTf-Documentation)

## Active repositories

Active repositories of AutoTF, that contain code that is used in prod are:

### Utility:
* [AutoTf.Logging](https://github.com/AutoTF-Rail/AutoTf.Logging): Logger used in all main AutoTF repo's.
* [AutoTf.YubiKeyInteractor](https://github.com/AutoTF-Rail/AutoTf.YubiKeyInteractor): Interactor to register yubikey's on the central server.
* [AutoTf.MotorCalibration](https://github.com/AutoTF-Rail/AutoTf.MotorCalibration): CLI Tool to calibrate and test motors.
* [Machine-Setup](https://github.com/AutoTF-Rail/Machine-Setup): Commands for a central bridge installation(To be moved to docs repo.)
* [AutoTf.Manager](https://github.com/AutoTF-Rail/AutoTf.Manager): Desktop app to manage the central server and trains.
* [AutoTf.GpsTest](https://github.com/AutoTF-Rail/AutoTf.GpsTest): A very simple console app to get the latitude and longitude as well as speed from a Gps device. (Code is partially used in Central Bridge)
* [AutoTf.FahrplanParser](https://github.com/AutoTF-Rail/AutoTf.FahrplanParser): A console app/package that parses images of a fahrplan into code to be used in automation.
* [AutoTf.Localisation](https://github.com/AutoTF-Rail/AutoTf.Localisation): CLI Demo to localise a train based on train display outputs + Hektometer recognition infront of the train. (Works with [AutoTf.FahrplanParser](https://github.com/AutoTF-Rail/AutoTf.FahrplanParser))
* [CentralBridgeInstall](https://github.com/AutoTF-Rail/CentralBridgeInstall/): Contains scripts used in the install script generated in [AutoTf.Manager](https://github.com/AutoTF-Rail/AutoTf.Manager).
* [AutoTf.AuthentikDashboard](https://github.com/AutoTF-Rail/AutoTf.AuthentikDashboard): API for interactions with the Authentik API for external users. (Includes somewhat working Avalonia WASM frontend).
* [AutoTf.AdminPanel](https://github.com/AutoTF-Rail/AutoTf.AdminPanel): API and Frontend for interactions with cloudflare, docker, plesk, and authentik to create new EVU servers easier.

### Central Code:
* [AutoTf.CentralBridge](https://github.com/AutoTF-Rail/AutoTf.CentralBridge): Backend that runs on the raspberry PI's on a train, that act as a central brain.
* [AutoTf.TabletOS](https://github.com/AutoTF-Rail/AutoTf.TabletOS): Avalonia OS that runs on a tablet to configure and control a central bridge/train.
* [Central Server](https://github.com/AutoTF-Rail/Central-Server): Dockerized central server to remote manage trains.
* [AutoTf.Aic](https://github.com/AutoTF-Rail/AutoTf.Aic): Backend that runs on the AIC (Jetson orin nano super) on a train to handle video streams to detect objects etc.



Please keep in mind that some repositories might not be public yet due to their active development.

## API documentation

Links to the api documentations can be found in [/swagger](https://github.com/AutoTF-Rail/AutoTf-Documentation/tree/main/swagger)

## Drawn Documentation

Documentation is made using Draw.IO and saved in [DrawIODOC](https://github.com/AutoTF-Rail/AutoTf-Documentation/tree/main/DrawIODOC/)

Exports can be found in

### Testing Roadmap:

![Test roadmap](https://raw.githubusercontent.com/AutoTF-Rail/AutoTf-Documentation/main/DrawIODOC/Export/TestRoadmap.png)

### Train setup diagram:

![Train Setup](https://raw.githubusercontent.com/AutoTF-Rail/AutoTf-Documentation/main/DrawIODOC/Export/TrainSetup.png)


### AI Control diagram:

![Train Setup](https://raw.githubusercontent.com/AutoTF-Rail/AutoTf-Documentation/main/DrawIODOC/Export/AI_Control.png)

### Open API diagram:

![OpenApi](https://raw.githubusercontent.com/AutoTF-Rail/AutoTf-Documentation/main/DrawIODOC/Export/OpenApi.png)

### Infrastructure diagram:

![Infrastructure](https://raw.githubusercontent.com/AutoTF-Rail/AutoTf-Documentation/main/DrawIODOC/Export/Infrastructure.png)



## 3D models

The molds for motors, and other prototyping is done in blender, and all models can be found in [Models](https://github.com/AutoTF-Rail/AutoTf-Documentation/tree/main/Models/).

Rendered screenshots can also be found in the Models folder.

There will always be a printable example version in the [ExampleLever](https://github.com/AutoTF-Rail/AutoTf-Documentation/tree/main/Models/Export/Print/ExampleLever/) folder.




## Licenses

While some repositories are listed under the Apache 2.0 license, main parts like the [CentralBridge](https://github.com/AutoTF-Rail/AutoTf.CentralBridge) are listed under the [GPL](https://www.gnu.org/licenses/gpl-3.0.txt) due to the usage of software/packages of third party listed as well under the GPL license.

For a list of used packages please refer to the individiual repository.


## Contributions

Would you like to contribute to this project, or noticed something wrong?

Feel free to contact us at [opensource@autotf.de](mailto:opensource@autotf.de)
