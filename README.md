# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.

## APPARATUS REQUIRED

PC installed with SCILAB

## PROGRAM 

clc;

clear;

clf;

xn = [1,2,3,4,4,3,2,1];

N = length(xn);

n = 0:N-1;

Xk = fft(xn);

disp("FFT output:");

disp(Xk);

K = 0:N-1;

magnitude = abs(Xk);

phase = atan(imag(Xk), real(Xk));

y = ifft(Xk);

subplot(2,2,1);

plot2d3(n, xn);

xtitle("Input Sequence", "n", "x(n)");

subplot(2,2,2);

plot2d3(K, magnitude);

xtitle("Magnitude Spectrum", "k", "|X(k)|");

subplot(2,2,3);

plot2d3(K, phase);

xtitle("Phase Spectrum", "k", "Phase (radians)");

subplot(2,2,4);

plot2d3(n, real(y));

xtitle("Inverse FFT Output", "n", "x(n)");

### CALCULATIONS:

<img width="1125" height="1500" alt="6bf44ed7-0fdb-43a7-8248-0bcfa3b937ae" src="https://github.com/user-attachments/assets/72c2b08b-a5eb-4468-adb5-0368c620f877" />
<img width="1125" height="1500" alt="959b0ae4-7759-4658-b7be-783b22459be1" src="https://github.com/user-attachments/assets/7899ad73-22fb-45cb-a40f-f570c438ac4d" />
<img width="1125" height="1500" alt="82cbf9c3-ec96-4c25-8e43-6192c574ac22" src="https://github.com/user-attachments/assets/5e73eb12-929e-4c6a-a626-126f18888647" />
<img width="1125" height="1500" alt="61ea0894-fcdf-4e36-9b72-22eae786f724" src="https://github.com/user-attachments/assets/1dd011b4-472e-43e1-b2e6-02856adc0887" />


### SAMPLE OUTPUT:
<img width="1125" height="1500" alt="24bc75a8-02f4-42e0-8f5b-9320c6922b5c" src="https://github.com/user-attachments/assets/9a6e672d-849b-4c0f-a2d6-2afc6066562f" />


## RESULT:

Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.


