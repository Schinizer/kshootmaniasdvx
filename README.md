# SDVX Charts for KShootMania #

SDVX Song packages meant for use in KShootMania. 

These charts follows the offical sdvx charts closely to emulate the original experience.

## How to setup for playing ##
1. Empty out the directory of "kshootmania\songs"
2. Clone the repository directly into "kshootmania\songs"
3. **`Optional`** Revert your directory to its original state (This repository is configured to ignore all other songs)
4. Start KShootMania
5. Enjoy.

The repository is configured this way for easy editing and playing the charts.

### Video Walkthrough ###
[![Screenshot](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/VideoWalkthrough.png)](https://www.youtube.com/watch?v=3Sh1gX-e9JE)

# Contributing to this project #

There are incomplete charts located in `\incompleteChart` folder.  
They are configured exactly like the `songs` folder of KShootMania.  
In `\incompleteChart\<song name>`, you will find the `.ksm` charts.  
They are fully mapped and in need of a little work to be playable.  

`If you cannot find the diffculty you are looking for, I'm sad to say I don't have the chart yet :(`

## Processing the charts##
1. Fork this repository & create a new branch
2. Look for the song you want to process in `\incompleteChart` folder
3. Cut & paste the whole folder into to `\sdvx`
4. [Processing the songs](https://github.com/Schinizer/kshootmaniasdvx#download-&-processing-the-songs)
5. [Processing the jacket](https://github.com/Schinizer/kshootmaniasdvx#processing-song-jackets)
6. [Processing the Song preview]()
7. [Processing the Spinning/Gravity effects]()
8. [Chart Proofing]()
9. [Play Test]()
10. Once everything is in order, make a pull request when you are ready
 
## Download & Processing the songs ##
Songs are downloaded from Youtube and processed. The objective here is to preserve the quality for the best experience.

### Step by step guide ###
1. Navigate to [SDVX譜面保管所](http://www.sdvx.be/) and find the song you are processing
2. Download the FX tracks and No FX tracks from the links (Youtube)  
![Reference](http://schinizer.github.io/kshootmaniasdvx/githubTutorials/SongDownload.png)  
If you do not have a downloader, you can try using [Clip Converter](http://www.clipconverter.cc/) or [4k Video Downloader](https://www.4kdownload.com/products/product-videodownloader).  
To prevent more re-encoding, download the sound as `.aac` or `.m4a` and process them.  
`Disclaimer: I am not afflicated with either products. Feel free to use them as you like`
3. Trim the tracks, offseting them if required and save them into `.ogg` format
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

# Project Status & Milestones #
- [x] Extract data from [SDVX 譜面播放器](http://sdvx-sheet.github.io/) and convert them into `.ksh` charts
- [x] Populate extracted data with meta data
- [ ] `In Progress` Process extracted `.ksh` charts
- [ ] SDVX Song requests | Process remaining SDVX songs
