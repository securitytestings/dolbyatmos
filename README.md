# dolbyatmos
A way to obtain Dolby Atmos Decoding, via a non Dolby-Atmos certified amplifier.




## ⚠️ DO NOT

This project is intended for **educational and legal purposes only**. Please adhere to the following guidelines:

- **DO NOT** attempt to bypass licensing or DRM restrictions.  
- **DO NOT** use this project to reverse-engineer proprietary software.  
- **DO NOT** distribute copyrighted or patented content without proper authorization.  
- **DO NOT** rely on this project for commercial use unless you have all required licenses.  
- **DO NOT** modify this project in ways that violate applicable laws or third-party agreements.  

Failure to comply may result in **legal consequences**. Use responsibly.  




## 🛠️ Software Needed

To follow this project/tutorial, make sure you have the following software installed:

- **[Dolby Reference Player]([https://professional.dolby.com/product/media-processing-and-delivery/drp---dolby-reference-player/])** – for testing and playing Dolby Atmos content.  
- **[VB-Audio Matrix Coconut](https://vb-audio.com/Matrix/coconut.htm)** – for routing the audio signals of Dolby Atmos.  
- **[VB-Audio VB-Cable Virtual Audio Device](https://vb-audio.com/Cable/)** – to create a virtual audio device for routing Dolby Atmos. 

## Setup Instructions

### Step 1 – Install Required Software
Make sure all the software listed above is installed.

---

### Step 2 – Configure Audio Devices
1. Open your **Advanced Sound Settings**.  
2. For both **Cable In 16ch** and **Cable Output**, which can be found inside **Playback** and **Recording**, make sure these settings are selected for it:
   - Channels: 16  
   - Bit depth: 16-bit or 24-bit  
   - Sample rate: 44100 Hz  (If you are listening to DDP (Dolby Digital Plus) Tracks, encoded for online media. 48000 Hz for True-HD.
3. These settings are found in the **Advanced** tab of each audio device.

---

### Step 3 – Configure Dolby Reference Player
1. Open **Dolby Reference Player**.  
2. Navigate to **Output Configuration**:
   - Set your **speaker layout** to your preferred setup.  
   - Set the **audio output device** to **CABLE In 16ch**.  

---

### Step 4 – Assign Speaker Channels
1. Click the **three dots** next to "Output Configuration" to open the **Speaker Configuration** options.  
2. Assign numbers to each speaker output (e.g., L = 1, R = 2, etc.).  
3. Save and close the speaker configuration.

---

### Step 5 – Configure VB-Audio Matrix Coconut
1. Open **VB-Audio Matrix Coconut**.  
2. In **Windows Devices** (WIN32.IN), use **CTRL + Left Click** to select **CABLE Output** as the input device.  

---

### Step 6 – Add Your Amplifiers
1. Add your amplifier outputs inside **WIN1.OUT**, **WIN2.OUT**, **WIN3.OUT**, etc.  
2. Use **CTRL + Left Click** to assign each audio device.

---

### Step 7 – Open the Routing Grid
1. Press **CTRL + 4** to open the **routing grid**.  
2. This grid allows you to map the Cable Output channels to your amplifier outputs.

---

### Step 8 – Route Channels Correctly
1. You need to assign each channel from **Cable Output** (left side) to the correct **WINx.OUT channels**.  
2. Typical channel order:
   - L = 1  
   - R = 2  
   - Center = 3  
   - LFE = 4  
   - Remaining channels: route manually based on your setup.
3. To route a channel, simply press **CTRL + Click** on one of the black squares in the routing grid.  
4. Tip: Play a Dolby Atmos track in Dolby Reference Player, **mute all channels except the one you want to route**, then check the routing grid to see which channel is active. Repeat until all channels are correctly assigned.

---

### Step 9 – Play Dolby Atmos Content
Once routing is complete:
1. Add a **Dolby Atmos track** to Dolby Reference Player.  
2. Press **Play**.  
3. Your setup should now output Dolby Atmos correctly through your non-certified amplifier.
