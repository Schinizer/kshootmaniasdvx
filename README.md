# SDVX Charts for KShootMania #

SDVX Song packages meant for use in KShootMania. 

These charts follows the offical sdvx charts closely to emulate the original experience.  

## SDVX and SDVX II Song packages ##
They are completed and playable. Due to github not able to support repository above 1GB in size, SDVX and SDVX II songs are removed from the repo and archived. The song packs can be found [here](https://github.com/Schinizer/kshootmaniasdvx/releases). 

## SDVX III Song packages ##
### How to setup for playing ###
1. Empty out the directory of "kshootmania\songs"
2. Clone the repository directly into "kshootmania\songs"
3. **`Optional`** Revert your directory to its original state (This repository is configured to ignore all other songs)
4. Start KShootMania
5. Enjoy.

The repository is configured this way for easy editing and playing the charts.

### Video Walkthrough ###
[![Screenshot](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/VideoWalkthrough.png)](https://www.youtube.com/watch?v=3Sh1gX-e9JE)

# Contributing to this project (Under Edit)#

This project has completed all SDVX and SDVX II charts. They have been archived and released.  
This repo will now only accept SDVX III charts.

## Processing the charts##
1. Fork this repository & create a new branch
2. Navigate to [KShootMania SDVX Song Status](https://docs.google.com/spreadsheets/d/1n0aO0TCHKOUCGxCDqg5vcdtosVNoQBc1Ty2WdSQHXtM) to check for collaborator status
3. Look for the song you want to process in the spreadsheet
    - Set the relevant cell to "In Progress" if you are working on it
    - To prevent conflicts, work only on songs that are not marked "In Progress"
4. Navigate to `\incompleteChart` and find the song folder you are working on
5. Cut & paste the whole folder into to `\sdvx`
6. [Processing the songs](https://github.com/Schinizer/kshootmaniasdvx#download--processing-the-songs)
7. [Processing the jacket](https://github.com/Schinizer/kshootmaniasdvx#processing-song-jackets)
8. [Processing the Song preview](https://github.com/Schinizer/kshootmaniasdvx#processing-song-previews)
9. [Chart Proofing](https://github.com/Schinizer/kshootmaniasdvx#chart-proofing)
10. [Processing Lane effects](https://github.com/Schinizer/kshootmaniasdvx#processing-lane-effects)
11. [Play Test](https://github.com/Schinizer/kshootmaniasdvx#play-test)
12. Once everything is in order, save the chart and commit your changes to your fork. 
13. Feel free to process other songs. (Repeat from step 4)
14. When you are ready, make a pull request!
 
## Download & Processing the songs ##
Songs are downloaded from Youtube and processed. The objective here is to preserve the quality for the best experience.

### Step by step guide ###
1. Navigate to [SDVX譜面保管所](http://www.sdvx.be/) and find the song you are processing
2. Download the FX tracks and No FX tracks from the links (Youtube)  
![Reference](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/SongDownload.png)  
If you do not have a downloader, you can try using [Clip Converter](http://www.clipconverter.cc/) or [4k Video Downloader](https://www.4kdownload.com/products/product-videodownloader).  
To prevent more re-encoding, download the sound as `.aac` or `.m4a`, then process them.  
`Disclaimer: I am not afflicated with either products. Feel free to use them as you like`
3. Trim the tracks, offseting them if required and save them into `.ogg` format (Repo only takes `.ogg`)
4. Rename the FX track `<diffculty>.ogg`
  * Novice charts `nov.ogg`
  * Advanced charts `adv.ogg`
  * Exhaust charts `exh.ogg`
  * Infninite charts `inf.ogg`
  * Gravity charts `grv.ogg`
5. Rename the No FX track `nofx.ogg`
6. Place the tracks into `\sdvx\<song you are processing>`  
7. And its done. (Charts are mapped to the song filenames too)

## Processing song jackets ##
Finding song jackets is mostly a google image searching task, there isn't a real method to get them.  

Here are some places you can find images for a start:  

[Remy Wiki](https://remywiki.com/SOUND_VOLTEX_Information) | [Google Image Search](https://images.google.com/) | [SDVX.be](http://www.sdvx.be/)
:------------: | :-------------: | :-------------:
[![RemyWikiJacket](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/RemyWikiJacket.png)](https://remywiki.com/SOUND_VOLTEX_Information) | [![GoogleImageJacket](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/GoogleImageSearch.png)](https://images.google.com/) | [![SDVX.beJacket](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/SdvxBe.png)](http://www.sdvx.be/)
Click the image for high res version | `Search by Image` works well | Use this if you can't find high res jackets  
Not always available | Not always available | Always available  

### Guidelines ###
  - Check if there is existing jacket (I've put some in)
  - Always use the highest res version you can find.  
  - Take note that this repository accepts only `.png` and `.jpg` files.
  - **For convenience, all charts are mapped to `jacket.png`**
    - Convenient if your jacket is `.png` and all difficulty share the same art. (Just name the jacket `jacket.png`)
  - If the song has different jackets for different difficulty, name them appropriately.
    - Novice Chart `nov_jacket.<extension>`
    - Advanced Chart `adv_jacket.<extension>`
    - Exhaust Chart `exh_jacket.<extension>`
    - Infinite Chart `inf_jacket.<extension>`
    - Gravity Chart `grv_jacket.<extension>`
    - **You will have to edit the meta of the relevant chart to accomodate this**

## Processing Song previews ##
Find the song's chorus timing and add it to song preview.  
It is not necessary to have 1:1 song preview with SDVX. Find what works well and use it.  

### Tips for song preview timing ###
![CursorTip](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/Cursor.gif)

## Chart proofing ##
The charts are directly extracted from [SDVX 譜面播放器](http://sdvx-sheet.github.io/) and they are prone to minor errors. You will need to correct the minor errors.  

Simply navigate to [SDVX譜面保管所](http://www.sdvx.be/) and find your chart for reference.

### Common errors ###
Red laser is quite prone to errors, so keep a look out.  
![LaserError](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/LaserError.png)  
`Tip: Use selection tool to select laser segment & ctrl + ← → to shift laser endings`  

BT & FX note errors are rare but may happen, keep a look out for them too.  

All the charts are trimmed to their first measure, so there might be padding errors like this.
![PaddingError](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/PaddingError.png)  
You can either offset the track or just shift the notes to fix this.  
`Tip: Use ctrl + a to select all notes, then ↑ ↓ keys to shift them`  

### Gravity Charts ###
![GravityChart](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/GravityChart.png)  
K-Shoot MANIA does not support laser notes going beyond their lanes at the moment.  
You will have to intepret the pattern and make it playable in KSM.  
The objective is to emulate the original track.  

## Processing Lane Effects ##
There are multiple lane effects in a SDVX track. Unfortunately, to find out what lane effects a track contains, you will need to find gameplay videos of it. From there, you will need to plot out the effects referencing from the video.

Here are some good youtube channels for reference  

김광민 | LIRINSKY | PmD Terra  
:----------: | :-----------: | :----------: 
[![김광민](https://yt3.ggpht.com/-EaeNq__geTk/AAAAAAAAAAI/AAAAAAAAAAA/smob9qOjfEc/s900-c-k-no/photo.jpg)](https://www.youtube.com/channel/UCbb00aZbCf5_WDMSxXYQSVQ) | [![LIRINSKY](https://yt3.ggpht.com/-G9CsF3hZSdM/AAAAAAAAAAI/AAAAAAAAAAA/amfTSRooj4I/s900-c-k-no/photo.jpg)](https://www.youtube.com/user/lirinsky) | [![PmDTerra](https://yt3.ggpht.com/-Te8JewC4tVw/AAAAAAAAAAI/AAAAAAAAAAA/EXotiRWc7xw/s900-c-k-no/photo.jpg)](https://www.youtube.com/channel/UCh1i3ODEGeslRpIL50v7JtA)  

Here is a breakdown of what needs to be done:  
- [x] ~~BPM Change~~
- [ ] [Lane Spin](http://gfycat.com/RepentantFortunateItaliangreyhound)
- [ ] [Lane Tilt](http://gfycat.com/WellmadeExhaustedCarp)
- [ ] [Lane Zoom](http://gfycat.com/CircularBountifulBarasinga)

## Play test ##
Please start K-Shoot Mania and navigate to the song you have created.  
Here is a simple check list to look out for:  
- Jacket check (If it doesn't load, please check your files)
- Meta check (Artist, Effector, illustrator, Level, Diffculty)
- Song Preview (Is the song preview correct?)
- FX Track check (Play the song and try missing & hitting laser or long FX notes)
  - If FX track is distorted / glitchy, your `nofx.ogg` and `<diffculty>.ogg` are not synced.
- Lane Effect check (Check if they are working as intended)

# Project Status & Milestones #
- [x] Extract data from [SDVX 譜面播放器](http://sdvx-sheet.github.io/) and convert them into `.ksh` charts
- [x] Populate extracted data with meta data
- [x] Process extracted `.ksh` charts
- [x] Create remainder SDVX songs charts with meta data
- [x] SDVX Song requests | Plot remaining SDVX songs
- [ ] `In Progress` SDVX III Songs

# Special Thanks for contribution #
- Kyanern  
- Dessard  
- xheres  
- Subreezy  
- ChickenNotHD  
