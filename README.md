# TickTrackTock
a timegrapher app

# Manual
This app requires a bit of dexterity and understanding of how other timegrapher devices and apps generally work. This particular one relies on the excellent microphone which is already built-in to your iPhone. You need a relatively quiet place to do this. The iPhone best picks up the sound when it is dressed in a protector and you put the bottom side of the phone flush onto the dial of the watch. Once you press the **start button**, you should see the beats on the top display.

## Setting the Beats-per-Hour
You need to manually set the beat-per-hour for your watch. Typically it is 6x3600 = 21,600 for the mainstream watches, and sometimes 8x3600=28,800 for some better models. If you do not not know it, don't worry: as soon as you start you should be able to see the beats of the watch on your display and count exactly how many times it beats in a second - that is the width of the display - then multiply the number of ticks you see by 3600 to get the beats-per-hour number. 
My Seiko watch is 21,600 BPH, so I see six beats per second on my display:

<img width="300" alt="tick_track_tock_ticks" src="https://github.com/user-attachments/assets/9a10b904-1201-44bc-8c12-392ac1636815" />

## Reading the Rate
The lower display has the advance/retard line. You can pull it up or down with your finger and align it to zero at the left of the display, then read off the deviation of the watch per 24 hours on the right side, just like in other timegrapher devices and applications. Please see the screenshots to get an idea of what you are supposed to see.

## The Beat Error
The beat error is the asymmetry of the oscillation of the balance wheel with respect to the fork. Ideally it should be below 0.5ms, but anything below 1ms is good. The reading in this app is pretty reliable.

## Reading the Amplitude
This is much harder to get it right. I provide two readings, one manual and one automatic, and hopefully they will agree within ±10°. Make sure you are really in a place as quite as possible to get a clean sound. The amplitude reading will take up to a minute to settle down after you lay down the watch *horizontally* either face up or down and stand the phone on top - I am not sure if the measurement will ever work on the wrist and/or how to prop up the phone to the watch in the *vertical* position. The manual reading is accomplished in the **waveform** display. Tap the checkbox at top left and you will see the sound waveform display. The horizontal scale is 2ms per minor tick on the axis.

<img width="400" alt="tick_track_tock_waveform" src="https://github.com/user-attachments/assets/f71d36d1-2c1c-4288-ad8f-a896472312e5" />

Pull the vertical green line and align it to the exact start of the first sound, which Witschi calls the A sound:
<img width="200" alt="εικόνα" src="https://github.com/user-attachments/assets/3282ff39-3427-4c15-8618-042963368dd2" />

The reading on the last line of the screen will reflect the corresponding manual amplitude readout. 

## Verifying the Amplitude 
I have also figured out a way to get the ground truth about the amplitude using the camera on that same wonderful iPhone. If you have a transparent back or the watch is open, you can go to the Camera app on your phone and shoot a max-zoomed
**Slo-Mo* video of your balance wheel. A few seconds of this at 240 frame-per-second should be enough. You look at the video frame-by-frame and you can read off the actual true amplitude from there. **Beware:** since amplitude normally is greater than 180°, you can be fooled, so watch it carefully. If you do this and your automatic and manual readings are far from the true value, let me know by filing on [this page](https://github.com/kotika/TickTrackTock/issues), providing as much detail as possible.

## Settings
I provide the possibility to set the lift angle and beats-per-hour in the Setting page. It is opened with a tap on the standard *gear* symbol **⚙** at the bottom of the screen.
