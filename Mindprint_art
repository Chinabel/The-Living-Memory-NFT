import pandas as pd
import matplotlib.pyplot as plt
import numpy as np

# Load EEG data
eeg_data = pd.read_csv("eeg_data.csv")

# Plotting the brainwave data
plt.figure(figsize=(12, 6))
plt.title("MindPrint - Brainwave Signature", fontsize=16)
plt.xlabel("Time")
plt.ylabel("Amplitude")

# Simulate different frequency bands if not labeled
colors = ['b', 'g', 'r', 'c', 'm']
for i, col in enumerate(eeg_data.columns[1:6]):
    plt.plot(eeg_data[col], color=colors[i], label=col)

plt.legend()
plt.tight_layout()
plt.savefig("mindprint_art.png")
plt.close()
