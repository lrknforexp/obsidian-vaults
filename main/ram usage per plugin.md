Checking the ram usage and its not going crazy for now since I am not using any plugins but I am going to take note of what each ram bumps it up to 
idle no plugins, theme, and CSS: 335-340
1. Calendar when first activated increases too 400 then decreased to 346-360
2. Editing toolbar when first activated bumps up to ~417 then goes down to 360-375
3. Data-view bumped up to 457 when first activated then goes down to 410-420  decrease is 390
4. Harper bums it up to 840 megabytes and doesn't decrease at all but instead keeps increasing total increase right now is ~1000+ disabling it decreases to 800mb and after resetting the application it goes down to ~497+
5. Iconic bumps it up to peak ~510+ goes down to ~450+
6. Image converter ram stays at solid ~416+ might increase a bit to 420-421
7. Self note opening the settings tab increases it to ~460+
8. Copilot peaked ~500-510+ MB but decreased down to ~460+ might go to 470+
9. Image in editor peaked 526 megabytes decreased down to 488+ goes up to 490+
10. Manual sorting spiked up to 546 but that's because i had the settings tab open which increases ram drops down to ~500 megabytes with all the extensions mentioned earlier, open excluding Harper since I am testing plugins and Harper explodes my ram lmao
11. Enabled Harper to test it out and it increased to 1 gigabyte of ram usage with all the extensions mentioned in an earlier statement open
12. Disabled Harper and its still at 1 gigabyte of ram usage I don't think Harper is using the ram but something else
13. Multi-column-Markdown still at 1 gigabyte of ram usage something has to be wrong
14. I am going to disable all the plugins to see what’s wrong.
15. Disabled them all still at 1 gigabyte relaunching brings it back down 
16. I am going to enable them all and then relaunch to check ram usage with them all on and disable and reset one at a time to see which makes a drastic change.
17. Enabling them all increased it to 1.4 almost 1.5 gigabytes
18. Relaunched and it dropped down to 1 gigabyte instead of 1.4-1.5
19. Disabled ytranscript and relaunched and its still 1 gigabyte
20. Disabled typewriter mode and relaunched the app and its still 1 gigabyte
21. disabled stylesettings for css and still 1 gigabyte
22. smart typography still 1 gigabyte
23. outliner went down to 700 then went back up to 900
24. Omnisearch 800 goes up to 900
25. notebook navigator somehow increased to 950 then went down to 790-800
26. multi-column-markdown 700 mb increased to 800 after clicking onto the app
27. **Harper is your biggest RAM offender**, but it's more nuanced than that. Let me break it down:
**The RAM culprits ranked:**

28. **Harper** — the most dramatic single-plugin impact. Goes from baseline to 840MB+ and _keeps climbing_ rather than settling. That "keeps increasing" behavior is a memory leak, not high usage. Even after disabling it, RAM doesn't fully recover until a full relaunch.
29. **Copilot** — also a heavy hitter. It takes **870ms to load** (by far the longest startup time — longer than all other plugins _combined_ almost), and contributes meaningfully to your baseline RAM. AI plugins are inherently heavy since they're managing model connections, caching, etc.
30. **The compounding problem** — your 1GB floor after enabling everything and relaunching once suggests something isn't fully releasing memory on disable. The fact that disabling plugins one by one still kept you at 1GB until a _fresh_ relaunch with fewer plugins confirms this. Obsidian (Electron) doesn't always garbage collect aggressively.

**What the startup data confirms:** Copilot at 870ms + Harper at 369ms + Notebook Navigator at 304ms = those three alone account for **~58% of your community plugin load time**.

**My recommendations:**

- **Harper** — disable permanently or only enable when actively writing. It has a clear memory leak (RAM grows and doesn't release). Check if there's a newer version or report it to the dev.
- **Copilot** — if you're not using AI assistance constantly, consider only enabling it when needed
- **Notebook Navigator** — worth testing without it since it showed a weird RAM _increase_ during your stepwise testing (step 25), which is suspicious
- **Always relaunch after disabling** — mid-session disabling doesn't free memory in Electron apps; only a clean boot reflects true usage

Your real baseline with all plugins except Harper is probably around **700-800MB**, which is honestly normal for Obsidian with 17 active plugins, 11 tabs, and a 240-file vault.


1. Obsidian start-up time breakdown

Obsidian version: 1.12.7
Installer version: 1.12.7
Operating system: Windows 11 Pro 10.0.26100

- Total startup time: 5,004 milliseconds
- Initialization: 783 milliseconds
- Vault (240 files): 253 milliseconds
- Workspace (11 tabs, 7 deferred): 1,058 milliseconds
- Core plugins: 267 milliseconds
- Community plugins (17 active): 2,643 milliseconds
  - Copilot (3.2.7): 870 milliseconds
  - Harper (2.0.0): 369 milliseconds
  - Notebook Navigator (2.6.2): 304 milliseconds
  - Omnisearch (1.28.2): 115 milliseconds
  - Iconic (1.1.8): 97 milliseconds
  - Image Converter (1.4.3): 89 milliseconds
  - Multi-Column Markdown (0.9.1): 83 milliseconds
  - Dataview (0.5.68): 76 milliseconds
  - Editing Toolbar (4.0.7): 74 milliseconds
  - Typewriter Mode (1.3.1): 65 milliseconds
  - Image in Editor (2.2.6): 32 milliseconds
  - Manual Sorting (3.2.4): 31 milliseconds
  - Style Settings (1.0.9): 29 milliseconds
  - Calendar (1.5.10): 25 milliseconds
  - Outliner (4.10.0): 24 milliseconds
  - YTranscript (1.3.1): 17 milliseconds
  - Smart Typography (1.0.18): 6 milliseconds




ram usage check 2.0 by turning them on and then disabling before activating another plugin
1. calender 230 idle 250+ while typing
2. copilot increased to 290 steady+
3. dataview 327+
4. editing toolbar 327+
5. harper peaked 800 when first turned on went down to 698+
6. iconic 250+
7. image converter 310+
8. image in editor 275+
9. manual sorting 250+
10. multi column markdown 300+
11. notebook navigator 340+
12. omnisearch 258+
13. outliner 246+
14. smart typography  220+
15. style settings 215+
16. typewriter mode 261+
17. ytranscript 228+