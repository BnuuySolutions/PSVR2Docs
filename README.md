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
- Interface 2 (Audio)
- Interface 3 (SLAM Tracking)
- Interface 4 (Data)
- Interface 5 (Gaze)
- Interface 6 (Image)
- [Interface 7 (IMU/Status)](imu-status-interface.md)
- Interface 8 (LED Detector)
- Interface 9 (Relocalizer)
- Interface 10 (Generated Data)
- Interface 11 (SLAM Trace)
- Interface 12 (Log)
