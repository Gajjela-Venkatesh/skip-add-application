Auto Ad Skipper
Auto Ad Skipper is a lightweight Python automation tool that detects and clicks the "Skip Ad" button automatically during video playback (e.g., YouTube ads).
It uses PyAutoGUI for screen recognition and image-based automation, providing a simple hands-free solution for ad skipping.

🚀 Project Overview
This script continuously scans your screen for a predefined “Skip Ad” button image (skip_button.png).
When detected, it automatically clicks the button — allowing uninterrupted viewing without manual input.

✨ Key Features
🖱️ Automated Ad Skipping — Detects and clicks the “Skip Ad” button automatically.

🧩 Image Recognition — Uses PyAutoGUI to find button patterns with adjustable confidence levels.

♻️ Looping Detection — Continuously scans every few seconds for new ads.

⚙️ Lightweight and Customizable — Modify detection frequency or image templates easily.

🧰 Technology Stack
Component	Technology
Language	Python 3.8+
Library	PyAutoGUI
Screenshot Handling	Pillow (for image processing)
🛠️ Installation and Setup
1. Clone the Repository
bash
git clone https://github.com/<your-username>/auto-ad-skipper.git
cd auto-ad-skipper
2. Create and Activate Virtual Environment
Windows

bash
python -m venv venv
.\venv\Scripts\activate
macOS/Linux

bash
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies
bash
pip install pyautogui pillow
4. Add the Skip Button Image
Save a clear screenshot of the “Skip Ad” button from your screen as:

text
skip_button.png
5. Run the Script
bash
python auto_ad_skipper.py
⚙️ Configuration
You can adjust detection parameters inside the script:

python
time.sleep(2)  # detection interval
confidence=0.7  # match confidence level
💡 How It Works
Takes periodic screenshots of your screen.

Searches for the skip_button.png pattern using image matching.

Moves the cursor to the center of the detected image.

Performs a click to skip the ad automatically.

⚠️ Notes
Works best when the screen resolution and “Skip Ad” button match the reference image.

May not work on minimized or background browser windows.

Use responsibly; for personal convenience only.

📄 License
This project is licensed under the MIT License.
Feel free to modify and share with proper attribution.

