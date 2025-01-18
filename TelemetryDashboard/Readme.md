## MAVLink Dashboard

This is a display only tool to help visualizing incoming MAVLink telemetry data.

This is not a GCS! It should be used in addition to a GCS.

Focus is on flexibility and user customization.


### Getting Started

1. Install pymavlink>=2.4.42
1. Run WebTools
1. Run SITL
    ```
    ./Tools/autotest/sim_vehicle.py -v Plane -L Kaga --console --map
    ```
1. In the MAVProxy console, add a websocket output:
    ```
    output add wsserver:0.0.0.0:5863
    ```
1. Connect