RAKTA Energy Management System

Real-time energy management system using AI for residential and commercial buildings.

## Badges

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Python](https://img.shields.io/badge/python-3.10+-green)
![License](https://img.shields.io/badge/license-MIT-green)

## Features

- ⚡ Real-time energy monitoring
- 🤖 LSTM-based load forecasting
- 💰 8-20% energy savings
- 🍃 Carbon footprint tracking
- 📱 Lightweight, runs on Raspberry Pi

## Requirements

| Hardware | Minimum Spec |
|----------|--------------|
| Raspberry Pi | 4 or 5 (4GB RAM) |
| SD Card | 16GB+ |
| Sensor | Current transformer |
| OS | Raspberry Pi OS 64-bit |

## Quick Installation

### Step 1: Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/rakta-ems.git
cd rakta-ems
Step 2: Run installer
bash
chmod +x install.sh
sudo bash install.sh
Step 3: Start the system
bash
source ~/rakta_env/bin/activate
cd rakta_core
python3 main.py
Project Structure
text
rakta-ems/
│
├── rakta_core/           # Main source code
│   ├── main.py           # Entry point
│   ├── ml/               # Machine learning models
│   ├── control/          # Control algorithms
│   ├── sensors/          # Hardware interfaces
│   └── utils/            # Utility functions
│
├── models/               # Saved trained models
├── deploy/               # Docker & deployment files
├── install.sh            # One-command installer
├── requirements.txt      # Python dependencies
└── README.md             # This file
Usage Example
After starting the system, you will see output like:

text
2025-01-15 10:30:00 - rakta.main - INFO - RAKTA Production System started
2025-01-15 10:30:30 - rakta.main - INFO - Power: 520.3W | Temp: 22.1C
2025-01-15 10:31:00 - rakta.main - INFO - Power: 510.8W | Temp: 22.0C | Savings: 1.8%
Configuration
Create a .env file for sensitive data:

bash
# .env file
ELECTRICITYMAPS_TOKEN=your_token_here
NORD_POOL_API_KEY=your_key_here
Testing
Run the test suite:

bash
python3 -m pytest tests/
Contributing
Fork the repository

Create a feature branch (git checkout -b feature/new-feature)

Commit changes (git commit -m 'Add new feature')

Push to branch (git push origin feature/new-feature)

Open a Pull Request

License
This project is licensed under the MIT License - see the LICENSE file for details.

Contact

Email: kavehbadri@gmail.com

GitHub: github.com/RAKTA-Co

Acknowledgments
Prof. Behnam Mohammadi Ivatloo (LUT University)

Dr. Zhengmao Li (Aalto University)

Business Finland for validation support
