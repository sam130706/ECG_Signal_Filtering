# ECG Signal Filtering using FIR and IIR (Butterworth) Filters

## Description
This project focuses on ECG (Electrocardiogram) signal processing by simulating real-world noise and applying filtering techniques to recover a cleaner signal. It also compares the performance of FIR and IIR (Butterworth) bandpass filters.

## Features
- Uses real ECG data (MIT-BIH dataset)
- Simulates realistic noise:
  - Baseline drift
  - Powerline interference (50 Hz)
  - Gaussian noise
- Supports multiple noise levels (low, moderate, high)
- Applies:
  - FIR Bandpass Filter (0.5–40 Hz)
  - IIR Butterworth Bandpass Filter
- Visual comparison of filtering results

## Technologies Used
- Python  
- Libraries: `wfdb`, `numpy`, `matplotlib`, `scipy`, `seaborn`

## Working Principle
ECG signals are often affected by noise from body movement, electrical interference, and sensors.

In this project:
1. Clean ECG signals are loaded from a dataset.
2. Noise is artificially added to simulate real-world conditions.
3. Filters are applied to remove unwanted frequencies.
4. The outputs are compared to analyze filter performance.

## How It Works
1. Load ECG signal using WFDB.
2. Extract a 10-second segment.
3. Add noise (baseline drift, 50 Hz interference, random noise).
4. Apply FIR bandpass filter.
5. Apply Butterworth (IIR) bandpass filter.
6. Plot and compare results.

## FIR vs IIR (Butterworth) Comparison

| Feature | FIR Filter | IIR (Butterworth) Filter |
|--------|------------|--------------------------|
| Stability | Always stable | Generally stable |
| Speed | Slower | Faster |
| Complexity | Higher | Lower |
| Output | Preserves waveform shape well | Produces smoother output |


## Key Concepts 
- **FIR Filter**: A stable filter that maintains signal shape accurately.
- **IIR Filter**: A faster filter that uses feedback for efficient processing.
- **Bandpass Filter**: Allows only useful ECG frequencies (0.5–40 Hz) and removes noise.

## Key Learnings
- Understood how noise affects ECG signals  
- Learned the difference between FIR and IIR filters  
- Explored practical signal filtering techniques  
- Visualized signal improvement after filtering  

## Future Improvements
- Add frequency domain analysis (FFT)
- Compare filter performance numerically
- Real-time ECG signal processing
- Integration with IoT-based systems

