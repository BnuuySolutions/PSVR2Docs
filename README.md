# PlayStation VR2 Docs
Reverse-engineered documentation for PlayStation VR2.

# "Report" Format
The PlayStation VR2 uses its own "report" format using USB transfer control calls, with the following structure:
- Report ID (UInt16)
- Sub-Command (UInt16)
- Data Length (UInt32)
- Data Buffer (504 bytes)

**NOTE:** Although most interfaces use the "report" format, a few also use bulk USB reads (e.g. Gaze), potentially with its own format.

# Interfaces
- Interface 0 (Control)
- Interface 1 (Audio)
- Interface 3 (SLAM Tracking) - CaesarUsbThreadSlamTracking
- Interface 4 (Data)
- Interface 5 (Gaze) - CaesarUsbThreadGaze (implemented by PlayStation VR2 Toolkit)
- Interface 6 (Image) - CaesarUsbThreadImage
- [Interface 7 (IMU/Status)](imu-status-interface.md) - CaesarUsbThreadImuStatus
- Interface 8 (LED Detector) - CaesarUsbThreadLeddet
- Interface 9 (Relocalizer) - CaesarUsbThreadRelocPre
- Interface 10 (Generated Data) - CaesarUsbThreadGenData
- Interface 11 (SLAM Trace)
- Interface 12 (Log) - CaesarUsbThreadLog
