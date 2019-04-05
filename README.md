# How to bond with another central B during the device is connecting with exist central A.

This example code is to show how to bond with another host B if the device is connected to host A.  It would enable the dual peripheral role.


### BLE configuration on the link

```
// <o> NRF_SDH_BLE_PERIPHERAL_LINK_COUNT - Maximum number of peripheral links. 
#ifndef NRF_SDH_BLE_PERIPHERAL_LINK_COUNT
#define NRF_SDH_BLE_PERIPHERAL_LINK_COUNT 2
#endif

// <o> NRF_SDH_BLE_CENTRAL_LINK_COUNT - Maximum number of central links. 
#ifndef NRF_SDH_BLE_CENTRAL_LINK_COUNT
#define NRF_SDH_BLE_CENTRAL_LINK_COUNT 0
#endif

// <o> NRF_SDH_BLE_TOTAL_LINK_COUNT - Maximum number of total concurrent connections using the default configuration. 
#ifndef NRF_SDH_BLE_TOTAL_LINK_COUNT
#define NRF_SDH_BLE_TOTAL_LINK_COUNT 2
#endif
```

## Instruction

* Press button 1 to erase all the bonding
* Press button 2 to advertising without whitelist with 30 seconds (wait for 2nd host bonding request)

# Requirements
------------
- nRF5 SDK version 14.2.0
- Softdevice S132v5.1.0
- nRF52832 DK 
- Segger Embedded Studio IDE (SES) Project

# Note

The project may need modifications to work with later versions or other boards. 

To compile it, clone the repository in the /nRF5_SDK_14.2.0/examples/ directory.
