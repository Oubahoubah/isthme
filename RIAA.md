# CamillaDSP to run phono correction
## RIAA biquad coefficients
From: https://www.musicdsp.org/en/latest/Filters/122-digital-riaa-equalization-filter-coefficients.html
- 44.1kHz:
a = [ 1.0000000000 -1.7007240000  0.7029381524 ]
b = [ 1.0000000000 -0.7218922000 -0.1860520545 ]
error ~0.23dB

- 48kHz:
a = [ 1.0000000000 -1.7327655000  0.7345534436 ]
b = [ 1.0000000000 -0.7555521000 -0.1646257113 ]
error ~0.14dB

- 88.2kHz:
a = [ 1.0000000000 -1.8554648000  0.8559721393 ]
b = [ 1.0000000000 -0.8479577000 -0.1127631993 ]
error 0.008dB

- 96kHz:
a = [ 1.0000000000 -1.8666083000  0.8670382873 ]
b = [ 1.0000000000 -0.8535331000 -0.1104595113 ]
error ~0.006dB
## CamillaDSP configuration
Integrate these coefficients to a Filter, type "Biquad Free". You won't find an a[0] in the interface, it should always be equal to one. 
