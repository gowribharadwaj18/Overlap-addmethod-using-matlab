# Overlap-Add Method Using MATLAB

## Overview  
This repository contains the MATLAB implementation of the **Overlap-Add (OLA) method**, a **Digital Signal Processing (DSP) technique** used for efficiently filtering **long signals** with a **Finite Impulse Response (FIR) filter**. By segmenting the input, processing smaller parts individually, and recombining the results, OLA reduces **computational complexity** compared to direct convolution.  

## Objective  
To implement and demonstrate the **Overlap-Add method** in MATLAB for **efficient signal filtering** while minimizing computational load.  

##  Methodology  
1️⃣ **Segmenting the Input Signal** – The signal is divided into **non-overlapping blocks**.  
2️⃣ **Zero-Padding** – Each segment is **zero-padded** to prevent **circular convolution**.  
3️⃣ **Convolution of Segments** – Each segment is **linearly convolved** with the FIR filter.  
4️⃣ **Overlap and Add** – The convolved segments are **overlapped and summed** to reconstruct the **output signal**.  

## 🔢 MATLAB Implementation  
The repository includes a **MATLAB script** that:  
1 Takes user input for **input sequence, filter, and segment length**.  
2 Performs **segmentation, zero-padding, and convolution**.  
3 Implements the **Overlap-Add method** to reconstruct the **filtered signal**.  
4 **Plots the input signals, filter, and final output**.  

## Sample Input & Output  

### **Input:**  
```matlab
x = [1 2 -1 2 3 -2 -3 -1 1 1 2 -1];  % Input Sequence  
h = [1 2];  % FIR Filter  
N = 4;  % Block Length  
```
## Output  

```ini
K = 4
N = 4
y = [1 4 3 0 7 4 -7 -7 -1 3 4 3 4 3 -2]
```
## Applications of the Overlap-Add Method  

. **Speech Processing** – Noise reduction, voice filtering  
. **Image Processing** – Filtering and restoring images  
. **Biomedical Signal Processing** – ECG/EEG noise removal  
. **Telecommunications** – Channel equalization, modulation  
. **Radar & Sonar** – Object detection and signal enhancement  
. **Data Compression** – Used in **MP3 & MPEG filtering**  
