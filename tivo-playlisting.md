# TiVo Playlisting

**TiVo Playlisting Console**

We're providing an interactive Playlisting Prototype and select assets from our music metadata catalog, to provide interactive experiences around:

* Track, Release, Album, Artist objective and subjective metadata
* Tones, Themes, Moods, and Similar Artists
* Artist & UMG album artwork

[https://discovery-demo.digitalsmiths.net/console/populations/tivo-music/carousels](https://discovery-demo.digitalsmiths.net/console/populations/tivo-music/carousels)

User: CapitalHackathon

Password: CapitalDec2018

For example, here's an API request for the 'Christmas' playlist you'll see in the playlisting console \(note the 'MW' ID is our album ID you can use with our Rovi Cloud Services API to retrieve album imagery and other associated information\) - 

[https://discovery-demo.digitalsmiths.net/sd/tivo-music/carousels/christmas](https://discovery-demo.digitalsmiths.net/sd/tivo-music/carousels/christmas) 

The prototype includes the following ‘Filters’ : Artist/Album Tones & Themes, Original Release Year, Song Popularity, Artist, Song Genre. All imagery and factual metadata is provided by TiVo Music Metadata.  Use the following cheat sheets for a complete listing of genre/subgenre/mood/theme metadata.

**Cheat Sheet** - Master Genre/Subgenre/Style List

Use the below link and choose File&gt;Download As&gt;CSV to import a CSV into your SQL/Mongo DB for a master list of all TiVo Music genres, subgenres, and styles - this can come in handy to create a genre/subgenre/style map or discovery experience.

​[https://docs.google.com/spreadsheets/d/1PgrGIifacbLokkh7mZgjU2JIi1zUGdVA0HMx4wlJIGs/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1PgrGIifacbLokkh7mZgjU2JIi1zUGdVA0HMx4wlJIGs/edit?usp=sharing)​

**Cheat Sheet** - Master Moods List

​[https://docs.google.com/spreadsheets/d/1K\_o6rKLHZ5zTkGbxLRw9ERXzpX3SfnKQSjKIKKaQHtM/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1K_o6rKLHZ5zTkGbxLRw9ERXzpX3SfnKQSjKIKKaQHtM/edit?usp=sharing)​

**Cheat Sheet** - Master Themes List

​[https://docs.google.com/spreadsheets/d/1OMA091NxeAFpOUAfPBU6AoP4iixNg3y1lDFK\_u9G2gk/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1OMA091NxeAFpOUAfPBU6AoP4iixNg3y1lDFK_u9G2gk/edit?usp=sharing)​

**Automated Playlists \(create a playlist based on artist, album themes, moods, tones, etc\)**

Click the “+” in the top left of the screen to create anew carousel

1. Provide an alphanumeric path name which will be part of the URL to

   call this carousel’s API. This can simply be the Name of the carousel

   with no spaces or special characters

2. Select the type “Automated”
3. Provide the name for your carousel. This will be the label for it when it is

   displayed. Click OK.

4. Click the “+” next to the “Any of the following are true...” message in

   the yellow strip

5. Select the “Filter” from drop-down
6. Select an available filter
7. Select the “Type” you want to use from the drop-down
8. Click in the “Values” field to see what options are available to you to

   select. As you start typing, the values will be searched against and limit the results. Select the value\(s\) you want.

9. View the Live Preview in the right pane. Use the arrows in the bottom of the pane to scroll through results.

10. Click the “+” on the right side of the dark gray strip of the center pane. This will add an additional filter. Both filters must be satisfied for the results to make it to the Live Preview pane. Additional filters can continue to be added as needed.

11. Click the “X” next to one of the filters. This will delete a filter.

12. Click the “+” next to the “Any of the following are true...” in the center pane. This has created a new set of filters. If any of the set of filters between the dark gray strips are satisfied, then they will be present in the Live Preview.

13. Hover over the sliders on the right pane to understand what each means. Try to slide a few of them over and note how the results in the Live Preview change order.

14. Click the disk icon on the top right of the screen to save it. You’vecreated an Automated Carousel.

**Removing Playlists**

1. Click the trash can icon at the top of the left pane to enter delete

   mode.

2. Click the “X” next to each carousel you just created.
3. Click the trash can icon at the top of the left pane again to come out

   of delete mode.

**Downloading Playlists**

1. Click the drop down, “Toggle Info” icon at the top of the center pane to enter delete mode.
2. Click on the pathway“sd/tivo-music/carousels/...”

3. With a JSON or XML web browser plug-in, you will be able to download and view the TiVo music metadata for each playlist

**UI Screen Testing**

1. Select Screens from the left navigation pane
2. Click the “+” in the top left of the to create a new screen
   1. Provide an alpha numeric path name which will be part of the URL to call this screen’s API. This can simply be the Name of thescreen with no spaces or special characters
   2. Provide the name for your carousel. This will be the label for it when it is displayed.
   3. Enter a default number of rows of carousels you want to return on your screen.
   4. Enter a default number of items you want to return in each carousel on your screen. Click OK.
   5. Drag a carousel from the lower left pane into the middle screen pane.
   6. Drag several more carousels into the middle screen pane. Note the listing of content in the Live Preview.
   7. Drag a carousel from the middle screen pane to a different position to update the ordering of carousels on the screen. Note the change in the Live Preview.
   8. Click the disk icon on the top middle of the screen to save it.  You’ve created a Screen.

3. Click the trash can icon at the top of the left pane to enter delete mode.

1. Click the “X” next to each screen you just created.
2. Click the trash can icon at the top of the left pane again to

   come out of delete mode.



