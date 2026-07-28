# ECG Signal Conditioning and Analog Design using LTspice

## Overview

This project presents the design and simulation of an Electrocardiogram (ECG) signal conditioning circuit using LTspice. The objective is to acquire a low-amplitude ECG signal, amplify it, suppress unwanted noise, and produce a clean output suitable for analog-to-digital conversion or further digital signal processing.

The design models a typical biomedical analog front-end used in ECG monitoring systems and wearable medical devices.

---

## Objectives

- Amplify low-amplitude ECG signals
- Remove baseline drift
- Eliminate 50/60 Hz power-line interference
- Reduce high-frequency noise
- Produce a clean analog ECG waveform for ADC input

---

## System Architecture

```
ECG Electrodes
      │
      ▼
Instrumentation Amplifier
      │
      ▼
Band-Pass Filter
      │
      ▼
50/60 Hz Notch Filter
      │
      ▼
Post Amplifier
      │
      ▼
Conditioned ECG Output
```

---

## Features

- Instrumentation Amplifier
- High Common-Mode Rejection (CMRR)
- Band-Pass Filtering
- 50/60 Hz Notch Filter
- Signal Amplification
- Noise Suppression
- LTspice Simulation
- AC Analysis
- Transient Analysis
- Frequency Response Analysis

---

## Tools Used

- LTspice
- Analog Circuit Design
- Operational Amplifiers
- Passive Components

---

## Circuit Blocks

### 1. Instrumentation Amplifier

Amplifies the differential ECG signal while rejecting common-mode noise.

### 2. Band-Pass Filter

Removes:

- Baseline drift
- High-frequency interference

Typical ECG bandwidth:

```
0.5 Hz – 150 Hz
```

---

### 3. Notch Filter

Removes power-line interference at:

- 50 Hz
or
- 60 Hz

depending on the electrical standard.

---

### 4. Post Amplifier

Provides additional gain to produce a signal level suitable for measurement and digitization.

---

## Simulation Performed

- Operating Point Analysis
- AC Sweep
- Transient Analysis
- Frequency Response
- Gain Analysis
- Noise Suppression Verification

---

## Results

The designed analog front-end successfully:

- Amplifies low-level ECG signals
- Rejects common-mode interference
- Suppresses power-line noise
- Preserves the ECG waveform within the desired bandwidth
- Produces a conditioned analog output suitable for ADC interfacing

---

## Applications

- ECG Monitoring Systems
- Biomedical Instrumentation
- Patient Monitoring Devices
- Wearable Health Devices
- Medical Electronics
- Analog Front-End Design
