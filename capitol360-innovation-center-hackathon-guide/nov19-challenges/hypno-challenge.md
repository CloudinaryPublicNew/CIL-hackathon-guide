# HYPNO Challenge

We believe the future of music is highly visual — a future where music is seen, not just heard. 

Our culture is increasingly powered by cameras and content, so how can we help artists \(and fans\) leverage these tools to make music more visual? How can cameras expand the studios where music is made? How can cameras evolve with social platforms where music is shared?

In this challenge, Hypno invites the developer community to its instant camera API, which mixes photos and videos with music and special effects in real-time. Our technology makes it easy for artists to shoot and share mini music videos, for example, and for fans to participate and contribute videos of their own. We're excited to see how the developer community uses Hypno to empower the next generation of artists... and shape the future of music.

\*\*\*\*

**Prizes**

The winning team will be awarded $1500 cash at Capitol Royale.

All developers who integrate our API into any of the challenges will receive a limited-edition reflective Hypno sweaty — and a VIP invite to Hypno Happy Hour.

\*\*\*\*

**Thought Starters**

Check out the \[Hypno Cam iOS app\]\([https://apps.apple.com/us/app/hypno-cam/id1249059769](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fapps.apple.com%2Fus%2Fapp%2Fhypno-cam%2Fid1249059769&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692203855&sdata=XXfOscAx7K3kRrVMASS8HqGfwXZULU7Fd1hqYAKpkEE%3D&reserved=0)\) in the App Store to see our real-time video processing API in action.

Here are some ideas for apps that could be built using the Hypno API:

\*Challenge 1:\*

Artists without big teams find it challenging to produce social videos that promote their music.

\*Solution:\*

Develop an app that makes it easy for artists to make quick, artist-branded videos without any editing or post-production \(think Ableton, but for video\).

\*Challenge 2:\*

Social music videos are an important tool to help spread music. Most artists don’t have a way to enable their fans to make content with their tracks.

\*Solution:\*

Develop an app that connects artists and fans who want to make and share social music videos. 

\*Challenge 3:\* 

Dance challenge videos are a fun way to go viral. Wouldn’t they be more fun with friends?

\*Solution:\*

Develop an app where you can directly challenge your friends to make a dance video using the song of your choice. After everyone submits their video, each person in your group will vote on the winner. A leaderboard keeps track of who’s winning amongst your friends and other friend groups around the world.



**Documentation**

The Hypno API is used to programmatically sequence and process video. The input to the API is video and other media assets, plus a script that defines how these are remixed to generate the output video.

A core component of the Hypno Platform is the \`libhypno\` iOS/MacOS software library. In addition to providing the library itself, we're providing two convenient ways to leverage it: an iOS framework \(with sample Xcode project\) and a cloud API.

!\[hypno diagram\]\([https://d2ddoduugvun08.cloudfront.net/items/1s1V0z3b281C1235382h/Messages%20Image\(2594241386\).png?X-CloudApp-Visitor-Id=1657970](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fd2ddoduugvun08.cloudfront.net%2Fitems%2F1s1V0z3b281C1235382h%2FMessages%2520Image%282594241386%29.png%3FX-CloudApp-Visitor-Id%3D1657970&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692203855&sdata=37BaiH2Vh7YdXJxs0Sm%2Bykvm%2Baam11jOU9Ghq%2FvRAfU%3D&reserved=0)\)

Hypno scripts are written in javascript and we provide an IDE called Nyx for authoring and previewing these scripts.

**Nyx**

\[Download Nyx \(MacOS only\)\]\([https://cl.ly/1abe5c0e1adb/download/Nyx.zip](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcl.ly%2F1abe5c0e1adb%2Fdownload%2FNyx.zip&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692213850&sdata=TIHy3sK0tn1x6OsnLWSVSSnBQSafQ6uqWi8VOBFzZiU%3D&reserved=0)\) and extract to Applications \(or some directory other than Downloads\); right click and press Open \(recommended for initial launch\).

\[Tutorial scripts\]\([https://github.com/HYPERHYPER/nyx-tutorials/tree/master/api-v2](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FHYPERHYPER%2Fnyx-tutorials%2Ftree%2Fmaster%2Fapi-v2&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692213850&sdata=3%2F%2F%2FErT0CKLMxdQ0zTlCaDs%2FLi2rKawdLBUOpHOKvb4%3D&reserved=0)\) covering the basics, plus some more interesting examples. Clone the repository and double click on the .nyxproj files to open tutorials. Stick to the newer api-v2 scripts.

\[Nyx / Hypno script API documentation\]\([https://hackathon.hypno.com/hypno/doc/modules/\_hypno\_.hypno.html](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fhackathon.hypno.com%2Fhypno%2Fdoc%2Fmodules%2F_hypno_.hypno.html&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692223840&sdata=VuPx4J0z4tEf5c1rWtWpqpAw%2F83%2FiqdCikOqVcdo1Zc%3D&reserved=0)\)

**Hypno.framework and Sample Xcode Project**

\`Hypno.framework\` is the iOS framework for \`libhypno\` that can be added to any iOS Xcode project. You can \[download it here\]\([https://hackathon.hypno.com/tbd](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fhackathon.hypno.com%2Ftbd&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692223840&sdata=wE2yvJJ7E%2FzXq2lvtCCAKI0w8EN42ggVB%2FW2a5TJPTc%3D&reserved=0)\).

You can also \[download a sample Xcode project\]\([https://hackathon.hypno.com/tbd](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fhackathon.hypno.com%2Ftbd&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692233836&sdata=irf%2B39O0QLMlurAdblG5Qum6Jzp3gO0wIz2z4oLs4fc%3D&reserved=0)\) to get up and running quickly with \`Hypno.framework\` with a working demo app you can build via github. We recommend starting with this if you're building an iOS app for this challenge.

**Hypno Cloud API**

The Hypno Cloud API gives developers a way to leverage the power of the Hypno API from any online application. You won't get the instant playback capability provided by the iOS library, but the same scripts can be used for both and will generate the same output.

\*\*\`POST /packages\`\*\*

Create new package. A package is a zip file with a hypno script and supporting assets, usually created with Nyx.

Example:

\`curl -F "[package=@MyScript.zip](mailto:package=@MyScript.zip)" -v [http://tbd.hypno.com:5000/packages\`](https://eur02.safelinks.protection.outlook.com/?url=http%3A%2F%2Ftbd.hypno.com%3A5000%2Fpackages&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692233836&sdata=cq0fP5BvgXSpt0xkkb4mkXF1I0kTTj87U6DMfqKo48c%3D&reserved=0)

This will return a package id that can be used for subsequent renders using that package.

\*\*\`POST /jobs\`\*\*

Create new job with a specified package.

Example:

\`curl -F "[camera=@default-002.mp4](mailto:camera=@default-002.mp4)" -v [http://tbd.hypno.com:5000/jobs?packageId=5ce8889e08d52fc337350233\`](https://eur02.safelinks.protection.outlook.com/?url=http%3A%2F%2Ftbd.hypno.com%3A5000%2Fjobs%3FpackageId%3D5ce8889e08d52fc337350233&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692243836&sdata=Ryofki4K8c8GiITzpNMkL99SDBbBi1HJrFoljvJdzP0%3D&reserved=0)

This will return a job id that can be used for downloading complete renders using that package.

\*\*\`GET /jobs/{id}/file\`\*\*

Downloads the finished video file.

\`[http://tbd.hypno.com:5000/jobs/5ce88c6008d52fc3d2050413/file\`](https://eur02.safelinks.protection.outlook.com/?url=http%3A%2F%2Ftbd.hypno.com%3A5000%2Fjobs%2F5ce88c6008d52fc3d2050413%2Ffile&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692243836&sdata=Pl5YeRm3Zk6jyBvu1gnARVC%2Fm7fO6Au2tmQKz0%2BVsMk%3D&reserved=0)

\#\#\# Libhypno

If you want to use the \`libhypno\` library directly, \[you can download it here\]\([https://hackathon.hypno.com/hypno/libhypno.tar.gz](https://eur02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fhackathon.hypno.com%2Fhypno%2Flibhypno.tar.gz&data=02%7C01%7CChingChing.Chen%40umusic.com%7C3f1c7404966b4ac9dee208d765eb8e6a%7Cbbcb6b2f8c7c4e2486e46c36fed00b78%7C1%7C0%7C637089934692253824&sdata=gTOeZgvTOUToYr3JpvjswLFFOlQalvYi%2Btb9H8vf0%2Bo%3D&reserved=0)\).

**Building** 

1. \`Under Build Settings\`/\`Apple Clang - Language - C++\` set \`C++ Language Dialect\` to GNU++17 \(libhypno makes use of c++17 features\).

2. \`Under Build Settings\`/\`Search Paths\` add an entry in \`Header Search Paths\` to \`path/to/libhypno folder\` example: \`$\(PROJECT\_DIR\)/vendor\` if you have a folder in your project directory called vendor with a libhypno folder inside it.

3. \`Under Build Phases\`/\`Link Binary With Libraries\` add \`+\` or drag and drop \`libhypno.a\` static library from your \`libhypno\` folder.

4. \`Under Build Phases\`/\`Link Binary With Libraries\` add \`AVFoundation.framework\`, \`CoreMedia.framework\`, and \`CoreServices.framework\`.

**Using**

1. Change your App Delegate file's extension too \`.mm\` \(libhypno makes use of c++\).

2. \`\#import &lt;libhypno/hypno.h&gt;\` inside your App Delegate file.

3. Inside your \`application:didFinishLaunchingWithOptions:\`method add a call to initialize the library \`hypno::Platform::initialize\(\);\`

4. Inside your \`applicationWillTerminate:\` method add a call to shutdown the library \`hypno::Platform::shutdown\(\);\`

5. Declare a property \`@property \(nonatomic, assign\) std::shared\_ptr&lt;hypno::Video&gt; video;\`

6. \`@synthesize video;\`

7. Create your first hypno \`video = hypno::Video::create \({ "path/to/JavaScript file", { path/to/main video file } }\);\`

