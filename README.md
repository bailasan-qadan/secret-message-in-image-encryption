# Block-Based LSB Steganography

This project implements a secure and robust method for hiding messages in images using the **Least Significant Bit (LSB)** technique combined with **block-based distribution**.

## 📌 Features

- **Block-Based Channel Embedding:** Divides the image into blocks and embeds data in rotating color channels (Red, Green, Blue) to minimize detectability.
- **Selective Channel Encoding:** Each pixel's channel is used independently to obscure message patterns.
- **Robust Against Detection:** Designed to resist statistical and visual steganalysis techniques.
- **Lossless Output:** Uses lossless image formats to preserve quality while embedding.

## 🔍 How It Works

1. The input image is divided into blocks (e.g., 4 pixels per block).
2. Each block embeds a bit of the secret message into a specific color channel (G, R, B in rotation).
3. Channels are rotated per block to avoid patterns and increase obfuscation.
4. The message is distributed across multiple passes if needed, minimizing alterations in any single channel.
