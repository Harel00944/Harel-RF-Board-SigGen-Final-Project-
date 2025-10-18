# Harel-RF-Board-SigGen-Final-Project-
RF Front-End Board for 430 MHz–4400MHz Signal Generator. Includes ADF4351 PLL , SKY13322 RF switch , PE43711 digital attenuator, GVA-63+ broadband amplifier. Designed for controlling  via MCU SPI control of the MCU Board( Part1 of the final Project)
This board is the second stage of the final project — an RF front-end board based on the ADF4351 PLL (Analog Device)
It can generate RF signals up to 4.4 GHz, either routed through the RF Front-End chain or directly output for testing purposes.

 Overview:

The board integrates several RF functional blocks designed for controlled amplitude and signal routing across the frequency range.
Power is supplied and filtered through multiple LDO regulators (TPS73633) to provide clean domains for each RF section ( PLL, Attenuator, Amplifier).

 Main Functional Blocks:

ADF4351 (Analog Devices) — Wideband PLL with integrated VCO, frequency range up to 4.4 GHz.

PE43711B (pSemi) — 7-bit digital step attenuator with 0.25 dB / 0.5 dB step resolution, controlled via GPIO from the MCU Board.

GVA-63+ (Mini-Circuits) — Wideband RF amplifier providing approximately 18–21 dB of gain across the band.

Filter Bank (Mini-Circuits ) — Selectable filters for harmonic suppression and signal conditioning.

RF Switches  — SP4T  RF switches used for routing between the filters in the filter bank , test output, and main signal path.

 Features

Output Frequency: 400 MHz – 4400 MHz

Output Power Range: (depending on configuration and gain stage). The board is designed to generate strong continuous-wave (CW) signals for testing purposes and to serve as a local oscillator (LO) source for RF mixers in  lab
Supports both direct RF  output and front-end chain output

Clean, low-noise power rails with separate regulation for PLL, VCO, and amplifier

SMA RF output for measurement and testing


Powered from the main MCU controller board via 5 V 

Controlled via SPI and GPIO from the STM32F405 MCU board

Main connector: J2 – IPL1-114-01-L-D-K (28-pin dual-row header)

<img width="1735" height="674" alt="image" src="https://github.com/user-attachments/assets/4563f24b-f571-47cd-accc-e6943eab3e51" />
<img width="1202" height="460" alt="image" src="https://github.com/user-attachments/assets/8c71c199-6dc2-464a-b2cc-a354825dadd8" />


