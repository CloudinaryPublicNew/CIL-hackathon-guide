# Hypno Challenge

We believe the future of music is highly visual — a future where music is seen, not just heard.

Our culture is increasingly powered by cameras and content, so how can we help artists \(and fans\) leverage these tools to make music more visual? How can cameras expand the studios where music is made? How can cameras evolve with social platforms where music is shared?

In this challenge, Hypno invites the developer community to its [instant camera API](https://instant.hypno.com/), which mixes photos and videos with music and special effects in real-time. Our technology makes it easy for artists to shoot and share mini music videos, for example, and for fans to participate and contribute videos of their own. We're excited to see how the developer community uses Hypno to empower the next generation of artists... and shape the future of music.

## Prizes

The winning team will be awarded $1500 cash at Capitol Royale.

All developers who integrate our API into any of the challenges will receive a limited-edition reflective Hypno long sleeve tee  — and a VIP invite to Hypno Happy Hour.

## Thought Starters

Check out the [Hypno Cam iOS app](https://apps.apple.com/us/app/hypno-cam/id1249059769) in the App Store to see our real-time video processing API in action.

Here are some ideas for apps that could be built using the Hypno API:

_Challenge 1:_ Artists without big teams find it challenging to produce social videos that promote their music.

_Solution:_ Develop an app that makes it easy for artists to make quick, artist-branded videos without any editing or post-production \(think Ableton, but for video\).

_Challenge 2:_ Social music videos are an important tool to help spread music. Most artists don’t have a way to enable their fans to make content with their tracks.

_Solution:_ Develop an app that connects artists and fans who want to make and share social music videos.

_Challenge 3:_ Dance challenge videos are a fun way to go viral. Wouldn’t they be more fun with friends?

_Solution:_ Develop an app where you can directly challenge your friends to make a dance video using the song of your choice. After everyone submits their video, each person in your group will vote on the winner. A leaderboard keeps track of who’s winning amongst your friends and other friend groups around the world.

## Developer Documentation

The Hypno API is used to programmatically sequence and process video. The input to the API is video and other media assets, plus a script that defines how these are remixed to generate the output video.

We're providing two convenient ways to leverage the Hypno Platform: an iOS static library called `libhypno` \(with sample Xcode project\) and the Hypno Cloud API.

![](../../.gitbook/assets/messages-image-19917885%20%281%29.jpeg)

Hypno scripts are written in javascript and we provide an IDE called Nyx for authoring and previewing these scripts.

### Nyx IDE

[Download Nyx \(MacOS only\)](https://pro.hypno.com/r/nyx-hackathon) and extract to Applications \(or some directory other than Downloads\); right click and press Open \(recommended for initial launch\).

Two short [tutorial videos](https://instant.hypno.com/tutorials) to get acquainted with the Nyx UI. 

[Tutorial scripts](https://github.com/HYPERHYPER/nyx-tutorials/tree/master/api-v2) covering the basics of writing Hypno scripts, plus some more interesting examples. Clone or download the repository and double click on the .nyxproj files to open tutorials. Stick to the newer api-v2 scripts.

[Nyx / Hypno script API documentation](https://hackathon.hypno.com/hypno/doc/modules/_hypno_.hypno.html)

### Hypno Static Library and Example Xcode Project

We're providing a sample Xcode project to get up and running quickly with `libhypno` in a working demo app that can be built with Xcode. We recommend starting with this if you're building an iOS app for this challenge. If you want to use the cloud API instead, skip this section.

1. Download the libhypno [iOS Example Project](http://pro.hypno.com/r/hackathon-sample-project) and extract the archive anywhere on your system.  
2. If you haven’t already done so, [download libhypno](http://pro.hypno.com/r/hackathon-libhypno) and extract the contents of the archive into /path/to/HYPNOApp \(iOS Example Project\)/vendor.  
3. Open `HYPNOApp.xcodeproj` with Xcode.  
4. Plug in your iOS device and build/run.

Alternately, if you want to add the `libhypno` static library to an existing Xcode project, [download it](http://pro.hypno.com/r/hackathon-libhypno) and follow these instructions:

#### Building

1. `Under Build Settings`/`Apple Clang - Language - C++` set `C++ Language Dialect` to GNU++17 \(libhypno makes use of c++17 features\).
2. `Under Build Settings`/`Search Paths` add an entry in `Header Search Paths` to `path/to/libhypno folder` example: `$(PROJECT_DIR)/vendor` if you have a folder in your project directory called vendor with a libhypno folder inside it.
3. `Under Build Phases`/`Link Binary With Libraries` add `+` or drag and drop `libhypno.a` static library from your `libhypno` folder.
4. `Under Build Phases`/`Link Binary With Libraries` add `AVFoundation.framework`, `CoreMedia.framework`, and `CoreServices.framework`.

#### Using

1. Change your App Delegate file's extension too `.mm` \(libhypno makes use of c++\).
2. `#import <libhypno/hypno.h>` inside your App Delegate file.
3. Inside your `application:didFinishLaunchingWithOptions:`method add a call to initialize the library `hypno::Platform::initialize();`
4. Inside your `applicationWillTerminate:` method add a call to shutdown the library `hypno::Platform::shutdown();`
5. Declare a property `@property (nonatomic, assign) std::shared_ptr<hypno::Video> video;`
6. `@synthesize video;`
7. Create your first hypno `video = hypno::Video::create ({ "path/to/JavaScript file", { path/to/main video file } });`

### Hypno Cloud API

The Hypno Cloud API gives developers a way to leverage the power of the Hypno API from any online application. You won't get the instant playback capability provided by the iOS library, but the same scripts can be used for both and will generate the same output.

**`POST /packages`**

Create new package. A package is a zip file with a hypno script and supporting assets, usually created with Nyx.

Example: `curl -F "package=@MyScript.zip" -v https://cloud.hypno.com/packages`

This will return a package id that can be used for subsequent renders using that package.

**`POST /jobs`**

Create new job with a specified package.

Example: `curl -F "camera=@default-002.mp4" -v https://cloud.hypno.com/jobs?packageId=5ce8889e08d52fc337350233`

This will return a job id that can be used for downloading complete renders using that package.

**`GET /jobs/{id}/file`**

Downloads the finished video file.

`https://cloud.hypno.com/media/5ce88c6008d52fc3d2050413`



