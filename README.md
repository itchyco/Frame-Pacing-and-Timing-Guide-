# Frame-Pacing-and-Timing-Guide-
An explanation of how frame pacing and timing can hinder the stability of your machine, no matter the performance power it has and its computing ability.

# What is Frame Pacing and Timing?

    Definition: It measures how evenly spaced the delivery of consecutive frames is, typically tracked in milliseconds.
    The Math: At a steady 30 frames per second (FPS), your system should deliver a new frame every 33.33ms | 30 FPS = 33.33ms per frame (1000 ÷ 30).
              At a steady 60 frames per second (FPS), your system should deliver a new frame every 16.67ms | 60 FPS = 16.67ms per frame (1000 ÷ 60).
    The Problem: If your graphics card outputs frames unevenly, such as one frame taking 7ms and the next taking 22ms, the game will stutter and feel 
              choppy, even if the average frame rate stays high.

# Examples of Bad Frame Pacing and Timing
<img width="461" height="191" alt="Screenshot 2026-08-27 224259" src="https://github.com/user-attachments/assets/9dd008d1-d602-4ef3-86f5-6a110d5d7b2c" />

# Examples of Good Frame Pacing and Timing
<img width="461" height="191" alt="Screenshot 2026-08-27 215137" src="https://github.com/user-attachments/assets/fdc28eaa-1313-4765-94f3-8053a6ceb592" />

Why is that bad? And how can we counter this issue?
Frame rate is just a count of how many frames show up each second. If those frames don't land in the same even intervals, Bad pacing means frames arrive unevenly even when the average FPS looks fine or high, and that unevenness is what shows up as stutter or judder. Stutter or judder is one of the main causes of your game feeling choppy and uneven. Most people would complain their game is at 100+ (FPS) but feels like it's at 30-40 (FPS) while holding those high frame rates. All that goes back to how each frame is sent and arrives. 

To combat this issue, you want to apply a frame limiter or V-Sync. 


# What tools to use? 
MSI Afterburner + RTSS | https://www.msi.com/Landing/afterburner (Free).
<img width="561" height="547" alt="image" src="https://github.com/user-attachments/assets/56260c05-ba51-4d7a-a496-2a86e176ba85" />


FramePacer | https://store.steampowered.com/app/4874400/framepacer/ (Paid). 
<img width="915" height="336" alt="Screenshot 2026-08-27 230356" src="https://github.com/user-attachments/assets/6d9a7267-998f-48ac-9e9a-94af53e2665c" />
