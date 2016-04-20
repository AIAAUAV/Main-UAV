Main UAV
====================

Main program run onboard the UAV Raspberry Pi running Windows 10 IoT.

Spec
---------------------

* Receive live telemetry from PixHawk
* Connect to cloud backend
* Log telemetry from PixHawk, CV and all other onboard devices/sensors
* Send live/logged telemetry to cloud backend
* Recieve flight instructions from cloud backend
* Make connection with base station through TBD radio device
* Recieve kill switch instruction through TBD radio device
* Send basically telemetry through TBD radio device

Notes
--------------------

Currently undecided as to whether the CV software will run on dedicated hardware or not. The telemetry logged to the cloud will be complete telemetry, compared to the subset sent to the base station over radio
