# IMU/Status Interface
This interface is usually used for receiving IMU data and getting/setting the overall state of the HMD.

# Reports

## (Set) Report ID 2 (DFU Mode)
Sub-Command: `Unknown`

Data: `Unknown (UInt32)`

Description: TODO.

## (Set) Report ID 5 (Power Off)
Sub-Command:
- 1 (Power Off)
- 2 (Reboot?)

Data: `None`

Description: Powers off or reboots the HMD. It is unknown what sub-command #2 does, as it seems to do the same thing as power off.
