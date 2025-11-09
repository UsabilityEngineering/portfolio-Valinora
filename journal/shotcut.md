# Shotcut
## A Non-linear Video Editor

### Colin Jamison
### 09 November 2025


# Goals

My goal with this interaction of Shotcut was to edit two videos together, and trim some dead space.
This is a simple beginner level interaction that mirrors patterns you would find in more advanced usages.
It should be easy to import the individual clips, manage their relative positons on a timeline, and export the final project.

I have some previous experience with using non-linear editors (NLEs) previous, so I expect there should be enough similarities that I should not need any significant guidance.
Needing to search for help or an outside guide should probably be seen as a failure of **affordances**, or visual clues that indicate what actions are possible.

# Interaction

![First Open](/assets/first_open.png)

When you first open the program, you are presented with this screen.
I did not resize the window nor any of the panels, leaving everything at its default.
In the center of the screen, I'm drawn to the 'start' button, but I notice it is greyed out.
I also see a wall of text on the left, with instructions for interaction.

![Project Name](/assets/project_name.png)

Filling in the name of the project, the start button becomes interactable.

![Project Created](/assets/project_saved.png)

Which upon first appearance does not seem to have gotten me any closer to my goal of splicing two clips together.
The center of the program is now empty, though the text on the left is still there.
Looking at the toolbar, I see a button labeled 'Open File', which seems promising.

![First File Opened](/assets/video_open.png)

Clicking that 'Open File' button brought up a OS Native file selection dialog (not pictured), which allowed me to select my first clip.
When that file was selected, and I pressed confirm on the selection dialog, it brought me to the pictured state.
A preview of the clip shown in the middle, which started automatically playing.
The text on the left also disappeared.
I was initially stuck here for a minute.
Remembering that the text said to "drag n' drop", I tried dragging the image preview itself to the playlist area.

![Preview Dragged to Playlist](/assets/video_drag_to_playlist.png)

This actually worked! However, in looking for how to add a video to the playlist (which I've been assuming to act as a library of all clips I want to edit), I notice this button:

![Multi Import](/assets/multi_import.png)

This button brought up another OS native file selection dialog, allowing me to add multiple files at once.
Furthermore, all files imported this way were automatically added to the playlist view.

![Multi Import Results](/assets/multi_import_results.png)

From there, I tried dragging clips from the playlist down to the timeline area.

![Video to timeline](/assets/video_drag_to_timeline.png)

Which seems to have worked.
It also seems to have automatically added a new blank video track above the one created by the first video.

![Second Video to Timeline](/assets/second_video_drag_to_timeline.png)

And dragging the second video into this track creates a third blank one.


# Analysis

The "Open File" button is a clear positive **affordance**, its labeling and location communicate its function well. However, many other interactive elements lack visual distinction. For example, the preview window and playlist area do not initially appear draggable or interactive, even though dragging is a key part of the workflow. This weak visibility contributes to early confusion.

The discovery of the “multi-import” button exemplifies limited **discoverability** (how easily a user can uncover available functions without instruction). The presence of multiple valid import paths (dragging, opening, multi-importing) is powerful but hidden. Contextual tooltips or a short onboarding overlay explaining these would dramatically reduce friction. Once the user identifies the import logic, Shotcut becomes efficient and predictable.