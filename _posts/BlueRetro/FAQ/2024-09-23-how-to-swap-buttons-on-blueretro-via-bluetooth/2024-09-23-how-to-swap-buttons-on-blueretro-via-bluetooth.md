---
layout: post
title: How to Swap Buttons on BlueRetro via Bluetooth
subtitle: Swap R2 and X for Pressure Sensitivity
author: Ripto
categories: [BlueRetro]
banner: 
  image: https://repository-images.githubusercontent.com/198868981/98d05272-da79-4387-97af-7aaa665b2ff9
  opacity: 0.5
image: https://repository-images.githubusercontent.com/198868981/98d05272-da79-4387-97af-7aaa665b2ff9
tags: BlueRetro FAQ Tutorial
---

#### 1. **Understanding BlueRetro and Button Remapping**
6	   - **BlueRetro** allows you to connect modern Bluetooth controllers (e.g., DualShock 3/4) to your PS2 and offers customizable button mappings, which is perfect if you want to swap the **R2 and X** buttons to take advantage of **R2's pressure sensitivity**.
7	   - BlueRetro runs on the **ESP32** and hosts a **web interface** that can be accessed via Bluetooth for configuration.
8	
9	#### 2. **Accessing the BlueRetro Web Interface via Bluetooth**:
10	   - Ensure that your **ESP32** running BlueRetro is connected to the PS2 and powered on.
11	   - On your Bluetooth-enabled device (laptop, phone, etc.), connect to the **BlueRetro ESP32** via **Bluetooth**.
12	   - After connecting, open a web browser and type:  
13	     **http://blueretro.io**
14	   - This will bring up the BlueRetro web interface where you can configure controller settings.
15	
16	#### 3. **Navigating to Controller Configuration**:
17	   - Once in the **BlueRetro web interface**, go to the section called **Controller Mapping** or **Player Configuration**. Here, you will see a mapping table showing which buttons are assigned to which inputs on your PS2.
18	   - For more information on this, refer to the **BlueRetro Wiki** at:  
19	     **https://blueretro.io/wiki**
20	
21	#### 4. **Swapping R2 and X for Pressure Sensitivity**:
22	   - **Locate the X Button (Cross)**: 
23	     - Find the **X button (cross)** in the mapping interface. By default, this will be mapped to the **X button** on your controller. You need to change this mapping to **R2**.
24	   - **Change R2 Mapping**:
25	     - Next, find **R2** in the mapping interface and change it to **X**. 
26	     - This will make **R2** function as the **X button**, allowing you to use its **pressure-sensitive** feature for tasks normally assigned to **X** (like acceleration or certain in-game actions).
27	
28	#### 5. **Saving the Changes**:
29	   - After you’ve swapped **R2 and X**, click the **Save Configuration** button in the web interface to apply these changes.
30	   - BlueRetro will store this configuration, so you won’t need to redo the mapping each time you use the PS2.
31	
32	#### 6. **Testing the Configuration**:
33	   - Now that you’ve saved the button mappings, boot up a game that uses pressure sensitivity (e.g., a racing game where **X** is used for acceleration). Pressing **R2** should now function like **X** but with the benefit of pressure sensitivity.
34	
35	#### 7. **Further Button Remapping or Adjustments**:
36	   - If you want to remap more buttons or fine-tune your setup, you can do so easily through the same **web interface**. BlueRetro supports remapping most buttons on modern controllers to match the PS2’s layout.
37	
38	### Resources for BlueRetro and Button Remapping:
39	- **BlueRetro GitHub** (Project repository and latest firmware updates):  
40	  **https://github.com/darthcloud/BlueRetro**
41	  
42	- **BlueRetro Wiki** (Comprehensive guide on setup, remapping, and troubleshooting):  
43	  **https://blueretro.io/wiki**
44	
45	- **BlueRetro FAQ** (Frequently asked questions, including button mapping details):  
46	  **https://blueretro.io/wiki/#/faq**
47	
48	By following these steps, you'll have successfully swapped **R2 and X** to ensure that you can take full advantage of **R2’s pressure sensitivity** for games that benefit from it. Let me know if you encounter any issues or need further clarification!
49	
50	To clarify, when I mentioned **"if compatible"** regarding multiple profiles and game-specific remapping, I was referring to features that might depend on the version of the **BlueRetro firmware** you're using. Let's break down what is compatible and what isn’t based on the current state of **BlueRetro** functionality:
51	
52	### BlueRetro Compatibility for Button Remapping and Profiles:
53	
54	1. **Global Button Remapping (Always Compatible)**:
55	   - **Every version of BlueRetro** supports **global button remapping**. Once you remap buttons like **R2 and X**, this remap will apply to **all connected controllers** and **all games** by default.
56	   - This means if you swap **R2 and X**, it will stay swapped for every game and controller until you change the mapping again.
57	
58	2. **Game-Specific Profiles (Limited Support)**:
59	   - **Profile-based remapping**—where you can save different button layouts for different games or situations—depends on the **firmware version** you are using.
60	   - As of the latest updates (September 2023), BlueRetro supports **multiple profiles**, but not all configurations may allow this feature in full detail yet.
61	
62	   ### Current BlueRetro Firmware Features:
63	   - **Global Remap**: Always supported.
64	   - **Multiple Profiles**: Supported in newer firmware, but still evolving. You can save and switch profiles for different controller setups or specific games. However, profile management may be limited depending on the setup of your **ESP32** and the specific build you're using.
65	   - **Controller-Specific Remapping**: BlueRetro does not yet offer a fully automated system for switching remaps based on individual games, but you can manually change profiles through the web interface.
66	
67	### Compatibility Check:
68	- If you're using an **updated firmware** version (recent 2023 builds), you likely have access to **multiple profiles** and can configure button mappings for different setups manually.
69	- Older or custom builds of BlueRetro may not yet support **profile management**, and in these cases, only **global remapping** is available.
70	  
71	For more specific compatibility, you can check your firmware version and compare it to the **latest BlueRetro releases** on their **GitHub** page:  
72	**https://github.com/darthcloud/BlueRetro/releases**
73	
74	You can also refer to the detailed **Wiki** for updated profile-related features:  
75	**https://blueretro.io/wiki**
76	
77	---
78	
79	### What Is Compatible:
80	- **Global button remapping** works on **all versions**.
81	- **Multiple profiles** or game-specific remapping may be available in recent versions, but it is not an automatic feature based on the game you're playing.