# Flight Guard AI

Flight Guard AI is a real-time cockpit voice analysis system designed to detect tone, assess flight risk, and generate contextual summaries from audio recordings. Built for offline operation, it uses a 4-bit dynamically quantized version of the Gemma 3n language model and is optimized for edge deployment.

This repository demonstrates the system using two real-world example flight audios:
- `Alitalia final.mp3`
- `8501_full audio.mov`

The notebook processes these audios by simulating real-time streaming in 15-second overlapping chunks. For each segment, it detects emotional tone (e.g. calm, urgent), assigns a risk level (LOW, MEDIUM, HIGH), and generates a short summary. Outputs include structured CSV/JSON files and a visual risk progression plot for dashboard integration.

No internet connection is required for inference, making this system ideal for secure, onboard aviation environments.
