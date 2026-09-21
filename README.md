ReaScripts-for-Reaper_current
Scripts to facilitate the workflow and tasks in Reaper.
(AliXiA project overseer, some coding, and very grateful) README v 1.0
Current Scripts in repo and descriptions. These scripts were created with the aid of some fine people I know who chose to take no credit only ask as I do that if you copy any of the code in here for your own projects to release then your project under the same licensing (or the portion containing our code) that we have chosen to use, GNU GPLv3. Thank you! I hope these scripts can help others as much as they have helped my workflow. Having ADHD is a bitch, so without these scripts I would loose focus doing the mundane and repetitive tasks some do. This allows me in turn to hyperfocus on what I love, music!  

1.**SESSION SETUP AND STEM INGESTION Lua SCRIPT v. 2.8** (previous versions are archived);
This script will create a new session by setting up the following tracks; Master (Presudo master keeps reference track routing   directly to Reaper master thus keeping your mix separated and ensures reference is not being processed). Reference Track,         Loopback, Drum Folder ( - child tracks include - Kick, White Noise for Kick, Snare, White Noise for Snare, Hi Hat, Tops,          Shakers, Perc 1 and Perc 2) routing for kick to trigger bass sub for sidechain is configured. Bass Folder that has the            following; Bass Main (where audio resides at - with JSFX 3 way splitter and routing to SUB, MID LOWS, and MID HIGHS)
SUB (with routing from kick to trigger sidechain and ReaComp), MID LOWS, and MID HIGHS. Keys Folder (Synth Pad, Synth Bass,       Synth   Melodic, Synth Lead, Piano Misc). Vocals Folder (Female 1 and 2, Male 1 and 2, Backing). FX Folder (FX1, FX2 and FX3).
  
     - Master bus with metering plugins**
     - FX sends/returns (reverb, delay)
     - Gain staging auto-integration
     - Better track organization
     - Improved error handling & logging
     - Sidechain routing refinements

  Stem ingestion - Still working on this feature. Script return no errors but not grabbing stems to ingest into tracks by           keywords.

2. **Diatonic Transposer v 1.8**
   Simple Transposing script enter the source root and source more and target root and target mode. Supports Major, minor, and        modes.
3. **Digital Fingerprinting v 1.3**
    Generates a hash that can be used to ensure file integrity has been kept while collaborating or sending them over networks.       Generate simply a hash and send it witht he file as a text file so receiving end can verify that file is intact.
4. **Mastering Floating Workflow Toolbar v 1.5**
   Multi-Function GUI for Import, cleanup and mastering prep.
5. **Pre-Mastering Mix Checker and Prep Utility v. 1.1**
   Enhanced with:
--   • Real-time peak & loudness metering
--   • Headroom analysis & recommendations
--   • Master bus FX detection
--   • Channel balance checking
--   • Export format validation
--   • Detailed pre-mastering checklist
--   • Integration hooks for mastering workflow
 6. **Mix Prep and Session Sanitizer v. 4.1**
 Enhanced with:
--   • Detailed logging & progress tracking
--   • Error handling & validation
--   • Folder track preservation
--   • Pre/post session verification
--   • Integration hooks for gain staging & transposition
--   • Customizable parameters
 7. **Stage gaining monitor for mixing v 1.5**
Displays:
    • Peak dBFS
    • Smoothed average level
    • Left / Right peak
    • Crest factor
    • Distance from -18 dBFS target
    • Visual dBFS meter
    • Gain-staging status

IMPORTANT:
REAPER's standard ReaScript API exposes real-time peak
meter information, but not a true post-FX RMS meter.

Therefore:
    PEAK       = actual REAPER track peak
    AVERAGE    = smoothed energy representation

The average is NOT falsely labeled RMS.

TARGET:
    -18 dBFS

No audio is altered.
No plugins are inserted.
No track settings are changed.

 8. **Studio Manager (Project, track, and time tracker) v. 2.7**

Features:
- Project metadata (client, track title, key/BPM, mix status, deliverables, revision notes, contact info)
- Track data (role, processing notes, routing, auto-detected media files)
- Quick note templates (timestamped)
- Time & billing log with start/stop timer
- Session summary (total hours, average session length)
- CSV export for invoicing
- Requires: ReaImGui extension


  


