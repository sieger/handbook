# Why you want to get the lowest latency #
- AFPS is one of the game types you want to have fastest reaction time, as just in couple of seconds everything can change, you can loose map control,  you can loose one of the main items, and even you might loose the game. So having even a slightest advantage will give you an edge.

- Forget games, why would you want a computer has a delay?

- Also optimized hardware / software will give you consistent feeling. Its like having a stable ping, if you sometimes have 10 ping, sometimes 70, you will loose it, your rails will not connect, you will always need to adjust your aim, but if you always have 30 ping, it will be consistant and better. 

- I am not and will never be a tweaker, do not ask, I just love to learn and try these little things that are matter.

So here, I will try to give you some information and some sources, sources from my friends to get you started to the journey. And I will try not to comment on anything I havent tried / tested, so feel free to ask further questions.

**Why latency matters, can you even feel it?**

When people say you cannot feel couple of ms, it is like smaller than a second, you show them this.  And this is only a video, you will feel a lot better. https://www.youtube.com/watch?t=80&v=vOvQCPLkPt4 

Here is a study by nvidia about the corrolation between latency and aim : https://www.nvidia.com/en-us/geforce/news/reflex-low-latency-platform/#why-does-system-latency-matter

**CPU**
- If you are going to play games, **intel** is the way. Try to get best intel possible with non disabled core. For example 10850k is failed 10900k, 10700k is really failed 10900k and 2 of its cores are disabled which will cause latency as well.
- If you are rendering / modelling stuff, then you buy the highest core number possible, which will be AMD these days. But this is not our focus, so I will not talk about it again.
- Uncore = Core.
- Disable all power saving features
- Flat llc for lowest delay - aim for smallest delta.
- Try not to leave anything auto
- Always check temperatures, try to test cpu stability with bootable linpack, 1-4 hours should be enough and your max cpu temp should be 80 degrees.
- Check temps in game, should be max 60, after that intel hinders the performance
- You can get Artic Freezer 420/360 as a good cpu fan
- Learn delidding and use liquid metal instead of thermal paste. It will give you 6-18 degrees difference which is huge!

**MOBO**
- Most poeple just get the cheapest motherboard they can get, no, get the best motherboard you can get. Most probably you will want to use 2 dimm motherboard, they have much stronger VRMs, you can check it from https://docs.google.com/spreadsheets/d/16YJm4L1-ohpL8s-4rLDDDCBZvi97ZYwkc44s7LS5-2Q/here. You should try to get the most PCB layer possible. Examples can be Asus Apex and EVGA Dark series. EVGA has the best quality pieces and really good OC capacity, but it has spread spectrum forced which will give you jitter. We are trying to get at least and option from EVGa to disable it at least in z590 board, but we will see. If we can do that, it would be one of the best motherboard available.
- Try to use grub to change hidden values.
- Use zipties and fans over VRM, Ram, PCH. 
- Try to use liquid coollers because air fans will be too big for you to put more fans over the important parts of the motherboard, besides 360aios will give better results.


**RAM**

Ram is my main topic I guess, because I really like how it works, how it behaves and everything.
- Try not to get RGB, some of the top rams will have rgb because of marketting stuff, but still you can almost always find an alternative.
- Try to get good bin b-die so that you can daily 1.5-1.6 easily, if you remove the heatsinks and put a fan on ram, you can go around 1.7-1.8V.
- Try to get a2 layout as its latency is the lowest. **A0** - 27.6, **A**1 - 19.73, **A2** - 13.13, **A3** - 13.67
- Try to get dual rank if your motherboard is good enough, which will be 2x16 rams right now. They are going to give you around 14% better results than single ranks with all other things same.
- For dual rank: **3600 14-15-15 1.45v**, **3200 14-14-14 1.3**5 are the ones I have tested and performed really well.
- For single rank: The one I can suggest most is **gskill 3600 15-15-15 1.35V**, It has really great OC potential, right now I am using this kit 4100-15-15 cr1
- Use cr1
- Max tREFI
- Min tRFC
- tRC/tRCD/tRAS/tRP is a lot more important than tCL
- try to lower iols to 3-5, and they should be max 1 point different than other one. 
- tRTP = tWR, this is not for latency but the stability and mouse feeling.
- remove your spreaders 
  - https://streamable.com/lmczh0 - strip front side 
  - https://streamable.com/vo9l2z - strip back side 
- After every single ram value change please test it, because it might now give error in a long time, but if there is a correction it will reduce the performance. Also if you change a value, but the tests are not that effected then it means there is a problem.
- Only test with intel memory latency checker. mlc. simple command can be `mlc --loaded_latency -t10`. and run it as admin.
- Testing for only 1 day will not be enough, try OCCT sse 1 night, OCCT avx 1 night, Anta55 1 night, then if you have Karhu 1 night, then you can say it is fine.
	
**Mouse**
- https://www.youtube.com/watch?t=540&v=gOQNRvJbpmk& try to get most pooling rate possible
- Yes you can feel the difference between 1000hz and 8000hz. It is not beyong human eye capabilities. If you think it is, go and try. Same peope argued people cannot feel the difference between 120hz and 240hz, they even argued 60hz vs 120hz. There will always be these people.
- Avoid wireless because of the interference. EMF, 4G, 5G, also wired has lower input latency.
- Try to use 1600 dpi. The idea is to use highest dpi without smoothing, it will have better latency and smoother mouse movement.
    
**Monitor**
- Because buying please check its input latency tests and try to get the most hz, lowest latency monitor. https://www.rtings.com/monitor/tools/table
- Try to limit fps in game, and check for the feeling, some games benefit from fps limit some dont. For example CSGO is worse with fps locked. Quake champions give worse latency with FPS locked.
    
**OS**
- Use Windows 7, even stock Win7 is a lot better than optimized windows 10.
- Install it as MBR
- Use Ntlite to debloat defender + bitlocker + superfetch
- If you really need windows 10, try to make dual boot.

**Mini Games**
- https://donttap.github.io/donttap/
- https://dphdmn.github.io/ballsheet/
- https://qqwref.github.io/schulte/
- https://schulte-table.com/
- http://www.aimbooster.com/

**Programs**
- Overclock your mice: https://github.com/LordOfMice/hidusbf
- MLC: https://cdn.discordapp.com/attachments/784503582716198912/784507138608201748/mlc.zip
- MouseTester: https://cdn.discordapp.com/attachments/784503582716198912/784507149535281182/Mouse_Polling_Test.zip
- Linlack Xtreme: https://www.techpowerup.com/download/linpack-xtreme/
- Ram testing with extreme@anta777 config: https://cdn.discordapp.com/attachments/653171331256549386/742827513218334861/TM5_extremeanta777.zip
- OCCT: https://www.ocbase.com/
- Karhu Ram test: https://www.karhusoftware.com/ramtest/
- Ntlite: https://www.ntlite.com/

**Best to read and follow!**
- https://twitter.com/siegerQL my twitter
- https://github.com/sieger/handbook this handbook
- https://i.imgur.com/pFxxbt9.png why Ram is important
- https://github.com/NVIDIA/Reflex-Latency-Analyzer-Mouse-Database/blob/main/NVIDIA%20RLA%20Mice%20Database%20-%20Github.csv - Nvidia click latency database
- https://www.pdl.cmu.edu/PDL-FTP/NVM/chargecache_low-latency-dram_hpca16.pdf leakage problem doubles every 10Degrees
- https://forums.blurbusters.com/viewforum.php?f=10&sid=fee291b005b0500ccd746e1783d13f0a Blurbusters
- https://kingfaris.co.uk/ram Importanjce of Ram oc by Kingfaris
- https://www.calypto.us/ One of the best guides to get lowest latency by Calypto
- https://docs.google.com/document/d/14ma-_Os3rNzio85yBemD-YSpF_1z75mZJz1UdzmW8GE/edit Overclock your GPU right way by Cancerogeno
- https://github.com/djdallmann/GamingPCSetup Mostly windows 10 focused, OS optimization by timecard
- https://github.com/BoringBoredom/PC-Optimization-Hub Great all around source for you to read by Bored
- https://github.com/integralfx/MemTestHelper/blob/master/DDR4%20OC%20Guide.md Detailed and really easy step by step Ram OC guide by Integralfx

**Some Proof**

Tweaked/oced bios vs default xmp one

![fps](/images/fps.PNG)
![base](/images/mice.png) ![tweaked](/images/micetweaked.png)
