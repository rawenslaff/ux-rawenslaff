# Adobe Premiere Pro's UI Scaling (*or lack thereof*)

I have been using Adobe Premiere Pro as my primary video editing software for a little over seven years, ranging from personal projects to professional work. As is common with most video editing software, its user interface (UI) includes a timeline, a program monitor (where users can preview their footage), and a variety of tools and effects that can be applied to clips in the timeline.

*(image of premiere layout)*

The timeline serves as the main workspace, allowing users to arrange and trim video and audio clips, apply effects, and adjust properties like color and volume. Everything is organized chronologically from left-to-right, while vertical layers determine the visibility of video clips (i.e., if several clips are stacked on top of one another, only the top clip is visible). This is analogous to traditional film editing, where physical film was cut and rearranged to create a finished movie. This demonstrates Jakob Nielsen's **Matching Between the System and the Real World** heuristic, which suggests that interfaces should follow real-world conventions so that users can relate to a familiar, real world counterpart.

*(film physically being cut) https://www.youtube.com/watch?v=lB933a1CF1Y*

Early last year, I was commissioned to edit a performance-style music video for a local artist. This type of project typically involves one audio layer (the song), and several video layers (different takes of the artist performing the song), all synchronized to that audio layer. 

I began synchronizing the footage to the song, and each take required placement on a new layer, so as not to overwrite a previous take. However, I quickly found myself running out of vertical space in the timeline. I could add as many layers as I wanted, but I needed to scroll up and down within the timeline panel if I wanted to see everything. This meant that there were always layers that were hidden, which interferes with Nielsen's **Recognition Rather than Recall** heuristic. Elements and relevant information should always be visible within the UI so users do not have to remember them. Because I couldn't see all my layers at once, I had to repeatedly navigate the timeline to locate certain takes, making the editing process less efficient.

Premiere Pro *does* provide some flexibility through the ability to vertically (and horizontally) zoom in and out of the timeline. However, I still managed to reach the limit of how far I could zoom out in the timeline while needing more room.

*(zooming in and out of timeline)*

My typical approach to an interface that feels too zoomed in is the *ctrl + minus* shortcut, as this is a common **convention** used to zoom out in browsers like Google Chrome or Mozilla Firefox, as well as in several apps, such as Spotify or Discord. However, this shortcut only zoomed out within the timeline, which was the action I had just done and not what I intended to do. That is to say, the **mental model** of using *ctrl + minus* to zoom out the UI that I had developed from prior application usage conflicted with Adobe's **conceptual model** of only zooming out within in the timeline panel. 

Ultimately, I determined that there is no native option within Premiere Pro to scale the UI.

Premiere Pro does have a menu found in the top of the UI, called Workspaces, which consists of over a dozen preset UI layouts, each targeting a specific stage of the post-production process (e.g., editing, color grading, audio), as well as any custom layouts the user creates. This appears to be Adobe's method of combatting the limited screen space available, but I found this to be a usability issue primarily because it lacks **efficiency**.

Having everything that I might need to interact with visible on my screen is efficient; everything has a dedicated space and is quickly available via cursor movement. Switching between workspaces, on the other hand, is **not efficient** for two main reasons:

1) Switching to another workspace involves several clicks or the pressing of a hotkey. This increases the number of steps needed to achieve my goal; one of the metrics used to evaluate efficiency.
2) Clicks/hotkeys aside, switching to another workspace itself can take several seconds to load. This is especially noticeable on larger project files. This increases the amount of time needed to achieve my goal; another metric used to evaluate efficiency. Additionally, taking several seconds to indicate to the user that their action was successful is an example of poor **feedback**. While a few seconds may not seem like a lot, it is magnitudes slower than the instant feedback the user expects, never mind the fact that users may need to perform the action several times.

This brings me back to my original issue: my inability to scale down the UI. A feature like this is not foreign to video editing software either. Another popular software, DaVinci Resolve, has UI scaling built in, as seen in the animation below:

*davinci animation: https://www.youtube.com/watch?v=PJyL8HW4k2c*

Even more frustrating is the fact that this issue is not even foreign to Adobe software. Adobe Illustrator, another program tailored for media editing/production, has a UI scaling feature similar to that of Resolve, yet it is absent from Premiere Pro.

*illustrator ui scaling option*

I eventually found a workaround to my problem, though it was not cheap nor quick. The UI scale of Premiere Pro is dependent on monitor resolution and operating system scaling. Since Windows 11 does not allow users to reduce the operating system scaling below 100% (what it was already set to), my remaining option was to increase my monitor resolution. So, I purchased a higher resolution monitor (*2560x1440 as opposed to 1920x1080*), which mostly solved my issue, as I now had much more space in the UI and could therefore see all of the layers in my timeline. Though this negatively contributed to my **satisfaction** with the software, as I frustratingly found myself needing to purchase additional hardware to compensate for what ultimately should have been a software limitation (that Adobe has already addressed elsewhere, might I add).

*animation from 1080p to 1440p*

Despite the limitations involved in the UI scaling, Premiere Pro was still **effective** in allowing me to accomplish my overall goal of editing the music video, as all the tools I needed to utilize were available to me. The process was just unnecessarily time-consuming and tedious due to the inefficiencies mentioned previously.

Though all of this could have been easily (and cheaply) avoided by adding a way to scale Premiere Pro's UI independently of monitor resolution and operating system scale. Something as simple as a slider like the one featured in Illustrator would have been more than adequate. This would positively contribute to both **User Control and Freedom**, as users would have the freedom to adjust the UI as they please, as well as **Flexibility and Efficiency of Use**, as the interface would accommodate different workflows, rather than forcing users to work around the limitations of switching between several workspaces. 

