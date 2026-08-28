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

To combat this issue, you want to apply a frame limiter or V-Sync. Applying in-game limiters doesn't fully give you smooth or even frame pacing; most game limiters fail at doing their jobs. The only way to achieve that perfect frame timing is to use 3rd-party tools such as RTSS (Rivatuner Statistics Server) and FramePacer (available on Steam). Both apps work very well at maintaining consistent frame timing, which you can see in the examples above.   

# The different types of limiters with RTSS: 
1) Async (Asynchronous).
* How it works: The default setting. It paces frames by buffering a single frame to ensure an exceptionally flat, uniform frametime graph.
* Pros: Delivers maximum visual smoothness and consistent frame delivery.
* Cons: Adds a minor one-frame buffer delay, slightly increasing input latency compared to uncapped or reflex-managed rates.
2) Front Edge Sync.
* How it works: Aligns frame generation intervals to the start (the front edge) of the display's vertical blanking (VBlank) refresh cycle. 
* Pros: Offers flexibility in presentation timing; useful for reducing micro-stutters or when combined with hybrid scanline sync.
* Cons: Can introduce minor input lag variations or tearing if not matched precisely to display refresh parameters.
3) Back Edge Sync.
* How it works: Synchronizes frame output to the trailing end (the back edge) of the refresh cycle interval.
* Pros: Helps manage tearing issues better than async in specific setups and works hand-in-hand with specialized scanline sync configurations.
* Cons: Generally exhibits higher overall input latency, making it less optimal for fast-paced competitive action.
# Other types of limiters
4) NVIDIA Reflex.
* How it works: Utilizes NVIDIA Reflex integration within RTSS to interface directly with the frame queue instead of enforcing a traditional software-side buffer.
* Pros: Bypasses the 1-frame delay of Async mode to dramatically lower system latency while keeping frametimes stable.
* Cons: Requires an NVIDIA graphics card and compatible API/game framework hooks to function properly.
5) AMD
  
# What tools to use? 
MSI Afterburner + RTSS | https://www.msi.com/Landing/afterburner (Free).
<img width="561" height="547" alt="image" src="https://github.com/user-attachments/assets/56260c05-ba51-4d7a-a496-2a86e176ba85" />


FramePacer | https://store.steampowered.com/app/4874400/framepacer/ (Paid). 
<img width="915" height="336" alt="Screenshot 2026-08-27 230356" src="https://github.com/user-attachments/assets/6d9a7267-998f-48ac-9e9a-94af53e2665c" />
