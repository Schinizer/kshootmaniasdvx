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
[![Screenshot](http://img.youtube.com/vi/3Sh1gX-e9JE/maxresdefault.jpg)](https://www.youtube.com/watch?v=3Sh1gX-e9JE)

# Contributing to this project #

There are incomplete charts located in `\incompleteChart` folder. 

They are fully mapped and in need of a little work to be playable.

## Processing the charts ##
1. Fork this repository
2. Look for the song you want to process in `\incompleteChart` folder
3. Cut & paste the whole folder into to `\sdvx`
4. [Processing the songs](https://github.com/Schinizer/kshootmaniasdvx#processing-the-songs)
5. [Processing the jacket]()
6. [Processing the Song preview]()
7. [Processing the Spinning/Gravity effects]()
8. [Play Test]()
9. Once everything is in order, make a pull request when you are ready
 
## Processing the songs ##
1. Navigate to [SDVX譜面保管所](http://www.sdvx.be/) and find the song you are processing
2. Download the FX tracks and No FX tracks from the links (Youtube)
3. Trim the tracks, offseting them if required and save them into .ogg format
4. Rename the FX track `<diffculty>.ogg`
  * Novice charts `nov.ogg`
  * Advanced charts `adv.ogg`
  * Exhaust charts `exh.ogg`
  * Infninite charts `inf.ogg`
  * Gravity charts `grv.ogg`
5. Rename the No FX track `nofx.ogg`
6. Place the tracks into `\sdvx\<song you are processing>`
