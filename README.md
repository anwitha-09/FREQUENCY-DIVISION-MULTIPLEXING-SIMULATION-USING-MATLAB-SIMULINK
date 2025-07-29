# Frequency Division Multiplexing Simulation Using MATLAB Simulink

This project demonstrates a secure analog communication system using MATLAB Simulink R2024b. It combines signal-level encryption with Frequency Division Multiplexing (FDM) to enable simultaneous transmission of multiple analog signals with simple, effective encryption.

## Features

- Pseudo-random phase modulation for analog signal encryption
- DSB-SC modulation using separate carrier frequencies
- Multiplexing via signal summation for FDM
- Coherent demodulation and decryption at the receiver
- Signal recovery with lowpass filtering
- Modular and clearly labeled Simulink design

## Tools Used

- MATLAB R2024b  
- Simulink  
- PN Sequence Generator  
- Scope blocks for visual verification  
- MATLAB (for optional plotting)

## System Workflow

### 1. Signal Generation
Two analog sine waves are generated with distinct frequencies.

### 2. Encryption
Each signal is encrypted by modulating its carrier phase using a pseudo-random binary sequence scaled by π.

### 3. Modulation and FDM
Encrypted signals are modulated using DSB-SC and combined into a composite FDM signal.

### 4. Demultiplexing and Decryption
The composite signal is split and demodulated using synchronized carriers and PN sequences to decrypt each stream.

### 5. Signal Recovery
Lowpass filters are applied to each decrypted signal to recover the original waveforms, displayed using Scopes.

## Simulation Output Graphs

### Message Signals
- [Message Signal 1](GraphOutputs/m1.jpeg)
- [Message Signal 2](GraphOutputs/m2.jpeg)

### Carrier Signal
- [Carrier Signal](GraphOutputs/carrier.jpeg)

### Pseudo-Random Encryption Setup
- [PN Sequence](GraphOutputs/PNsequence.jpeg)
- [Pulse Encryptor](GraphOutputs/pulse%20encryptor.jpeg)

### Encrypted and Modulated Signals
- [Modulated Signal 1](GraphOutputs/modulated.jpeg)
- [Modulated Signal 2](GraphOutputs/modulated_2.jpeg)

### Multiplexed Signal
- [FDM Composite Signal](GraphOutputs/multiplexed.jpeg)

### Demultiplexing and Decryption
- [Demodulated Signal 1](GraphOutputs/demod.jpeg)
- [Demodulated Signal 2](GraphOutputs/demod_2.jpeg)
- [Decrypted Signal 1](GraphOutputs/demultiplexed.jpeg)
- [Decrypted Signal 2](GraphOutputs/demultiplexed_2.jpeg)

