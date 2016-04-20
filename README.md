Main UAV
====================

Main program run onboard the UAV Raspberry Pi running Windows 10 IoT.

Spec
---------------------

* Receive live telemetry from onboard PixHawk through MAVLink over UART interface
* Connect to [Cloud Backend](https://github.com/AUUAV/Cloud-Backend) through onboard 3G/4G usb stick
* Log telemetry from PixHawk, [Computer Vision](https://github.com/AUUAV/Computer-Vision) and all other onboard devices/sensors (possibly to external storage in case of pi failure?)
* Send live telemetry to [Cloud Backend](https://github.com/AUUAV/Cloud-Backend) or logged telemetry if connection was lost and found again
* Recieve flight instructions from [Cloud Backend](https://github.com/AUUAV/Cloud-Backend)
* Make connection with [Base Station](https://github.com/AUUAV/Base-Station) through TBD radio device
* Recieve kill switch instruction through TBD radio device
* Send basic telemetry through TBD radio device

Notes
--------------------

Currently undecided as to whether the [Computer Vision](https://github.com/AUUAV/Computer-Vision) software will run on dedicated hardware or not. The telemetry logged to the [Cloud](https://github.com/AUUAV/Cloud-Backend)  will be complete telemetry, compared to the subset sent to the base station over radio
