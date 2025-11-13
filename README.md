**Light-O-Rama Audio Packager**

Turn any song you legally own into a complete Light-O-Rama timing package.

What This Toolkit Does:

• Download high quality audio from a YouTube link.

• Convert any MP3 or WAV into a clean mono WAV at 44.1 kHz.

• Detect beats automatically and build timing labels.

• Generate a SuperStar timing grid.

• Package everything into an import ready folder with no extra steps.

• Works on Windows and macOS with simple double click launchers.

Who This Is For:

• Holiday lighting hobbyists.

• Light-O-Rama users who prefer simple tools.

• Volunteers helping with shows.

• Anyone who wants beat grids without learning audio software.

## ⚖️ Before You Start

Only process audio you own or have explicit permission to use. You are responsible for how you use this toolkit.


<details> <summary><strong>See the full legal references</strong></summary>


YouTube Terms of Service: https://www.youtube.com/static?template=terms

Digital Millennium Copyright Act (DMCA): https://www.copyright.gov/legislation/dmca.pdf

Local and international copyright laws

</details>

---

**Step-by-step instructions:**

---

Step 1: Download the Toolkit:

Click the green Code button on GitHub

Choose “Download ZIP”

Unzip it somewhere easy to find (Desktop recommended)

If you are comfortable with Terminal or PowerShell, please skip to **Advanced: Manual Setup**

---

Step 2: Running the Toolkit:

**macOS (Auto Setup)**

Right click Run_LOR.command → Open

Approve the macOS “from the internet” warning (standard warning, this software is not malicious)

First run creates the virtual environment

Select your MP3 or WAV

Output appears on your Desktop

---

**Windows (Auto Setup)**

Right click Run_LOR.bat → Run as Administrator

First run creates a virtual environment and installs everything

The script launches the packager

Choose your MP3 or WAV file

A **folder** named like this appears on your Desktop:

song_LOR_Package

---

Step 3: Import Into Light-O-Rama:

Sequencer (S6)

**Place your Light-O-Rama Audio Packager:**

**macOS: ~/Documents/Light-O-Rama/Audio**

**Windows: Documents\Light-O-Rama\Audio**

**(This is a must to continue, you can also manually place the file into the Audio file associated with the Light-O-Rama folder)**

---

Open Sequencer

File → New → Musical Sequence

Choose the _LOR.wav file

locate Timings: Timings → Import Timings

Choose your _LOR_Timings.txt file

Start sequencing

---

**SuperStar (if owned)**

Open SuperStar

File → Import Timings

Choose the _LOR_SuperstarGrid.xml file

Start sequencing

---

**Advanced: Manual Setup**

---

**Mac Terminal:**

python3 -m venv venv

source venv/bin/activate

pip install -r requirements.txt

python lor_packager.py inputfile.mp3

---

**Windows PowerShell:**

python -m venv venv

.\venv\Scripts\activate

pip install -r requirements.txt

python lor_packager.py inputfile.mp3

---

**Troubleshooting:**

Python not recognized: Install Python 3.10 or newer

macOS blocked the command: System Settings → Privacy and Security → Allow Anyway

No folder appears: Ensure the MP3 or WAV is valid

Beats look wrong: Try a higher quality source or a file with clearer percussion

---

**Author & License:**

Created by John Thomas DuCrest Lock (FX Industries • SYMBEYOND Project)

---

MIT License — free to use, modify, and distribute responsibly.

---

“I can’t see the breeze, yet I can see the leaves flutter.” — SYMBEYOND

---

Have an idea or found an issue? Open a GitHub issue with your OS, Python version, and LOR version.
