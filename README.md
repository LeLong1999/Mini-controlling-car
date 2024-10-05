# MINI CONTROLLING CAR

This projec target on some critical feature below:

* Let user control the car from long distance

* Sharing realtime GNSS information and low quality video with user

* Supporting Software download though OTA.

Contains 3 basic ECUs:

> CHASIS: Responsible for receving driven signal and controlling car.

> Telematic Unit (TCU): Responsible for reading UBLOX for GNSS. Communicating with module SIM to get ethernet/wifi (Software download, Image trasnferring)

> GATEWAY: Responsible for communicating with LORA (Controlling command) This ECU controlling critical power management of both chasis and TCU. This one will be the gateway between chasis and TCU.

General communication will be used as CAN. SPI will be used at low layer of each ECU