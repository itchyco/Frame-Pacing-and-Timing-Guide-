# Frame-Pacing-and-Timing-Guide-
A explination into how frame pacing and timing can hinder the stability of your machine, no matter the performance power it has and computing ability.

# What is Frame Pacing?

    Definition: It measures how evenly spaced the delivery of consecutive frames is, typically tracked in milliseconds.
    The Math: At a steady 30 frames per second (FPS), your system should deliver a new frame every 33.33ms | 30 FPS = 33.33ms per frame (1000 ÷ 30).
              At a steady 60 frames per second (FPS), your system should deliver a new frame every 16.67ms | 60 FPS = 16.67ms per frame (1000 ÷ 60).
    The Problem: If your graphics card outputs frames unevenly—such as one frame taking 5ms and the next taking 30ms—the game will stutter and feel choppy, even if the average frame rate stays high.
