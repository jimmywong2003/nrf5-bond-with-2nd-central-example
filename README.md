# nrf5-multiple-bond-example

In this example, I use the example ble_app_hrs to show how to bond with 2nd host and then replace the existing bonding record.

When the nRF52 is bonded with Host A, nRF52 would use the advertising with whitelist for reconnection.  

## Procedure

* Press button 1 to erase all the bonding
* Press button 2 to advertising without whitelist with 30 seconds (wait for 2nd host bonding request)

## Requirement

* NRF52832 DK 
* SDK 14.2 / S132v5.1
* IDE: Segger Embedded Studio
