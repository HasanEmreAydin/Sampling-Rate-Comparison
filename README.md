# Sampling-Rate-Comparison

# Signal Sampling Analysis

This MATLAB code demonstrates the effect of different sampling rates on a sine wave signal by comparing a high sampling rate (8000 Hz) with a low sampling rate (4000 Hz). The objective is to observe aliasing in the signal sampled at a lower rate.

## Code Explanation

### Parameters
- `fs_high` - High sampling rate (8000 Hz).
- `fs_low` - Low sampling rate (4000 Hz).
- `f_signal` - Frequency of the sine wave (3000 Hz).
- `t_high` - Time vector for the high sampling rate.
- `t_low` - Time vector for the low sampling rate.

### Signal Generation
The code generates a sine wave signal at a frequency of 3000 Hz. It samples this signal at two different rates:
- High sampling rate: 8000 Hz (no aliasing)
- Low sampling rate: 4000 Hz (expected aliasing)

### Plotting
The results are plotted to visualize the effect of sampling rates on signal representation:
1. **Sampling at 8000 Hz** (blue): Displays the sampled signal without aliasing.
2. **Sampling at 4000 Hz** (red): Displays the sampled signal with aliasing, as 4000 Hz is close to the Nyquist rate, which results in loss of information in the signal.

## Usage
1. Run the code in MATLAB to generate the plots.
2. Observe the difference between the two subplots to understand how aliasing affects signal sampling.

## Interpretation
- **No Aliasing (8000 Hz)**: The high sampling rate captures the sine wave accurately, maintaining its original shape.
- **Aliasing (4000 Hz)**: The low sampling rate causes the sampled signal to deviate from the original sine wave, resulting in aliasing.
