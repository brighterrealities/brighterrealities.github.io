# What'sNew

> ## IMPORTANT! 
> Please delete and re-install your watch app for every build, particularly if you see sync issues (artwork missing etc). Many things have changed and the database needs to be built from scratch. Easiest way is via the watch app, find Wristrax, toggle off, wait a few seconds, toggle back on.   

---

## Version 1.0 (Build 16)

Unless there are any unexpected bugs (not that we have expected bugs…), this might be the RC as Apple finally updated my address so this could go get submitted now.  So please report any issue, no matter how small.

### Fixes:
1. Stale Plex user Avatar fix

### What’s new:
#### 1. Tracking of playlist changes
- Playlist Library view (2nd tab):
  - Pull down to refresh
  - Playlists with changes will have icon in library
- Sync View (3rd Tab): 
  - Download (1st segment): Added tracks from PL will be added to download queue
  - Select (2nd segment): PL will show that there is an update and will show added tracks if you expand PL line
  - Watch (3rd segment): sync now will add tracks
    - Removed tracks will be removed from watch immediately after PL refresh, no sync needed
    - Tracks only get removed if they have no relationship with downloaded albums

#### 2. Icons to flag library items as downloaded, selected, synced. 
- Artist will show grey icon if any release has a status (highest state wins). So if one album is download and one synced, artist will show grey watch icon)

#### 3. Updated view for Watch content
- same expandable pattern used everywhere else

#### 4. Watch App:
- Playing a track, play all or shuffle all now moves focus to play now screen as visual feedback
- Reduced crown sensitivity for volume control in play now screen by 50%

---

## Version 1.0 (Build 15)

This is kind of a big deal build. It contains a few things I had planned post-launch, but as Apple is not capable of changing my Dev account postal address for almost 2 weeks, I have extra time to invest. This is a bit risky because new fundmental stuff might pop up. But hopefully it is worth it.

### 0. Whats new (this!) 
- Now we have this in-app and without character limits!

### 1. Syncing had a complete overhaul! 

- You download albums/singles/EPs or Playlists from your Plex library to your phone
- From those, you select what you want to have on the watch
- You sync your watch

- If you want to remove something from the Watch, you de-select it. You can sync it again later. 
- You sync your watch.

- If you want to remove something from your phone and watch, you line-swipe to delete it. It removes it on phone and watch. (We can’t have tracks - only on watch, this would be too complex to manage for the shared database).

This means you can keep a large offline library on your phone and only sync a subset to your watch. Th sync tab is fully functional even when your Plex server is not reachable.

This was done in response to a handful of smaller requests (like “how can I remove playlists?” etc.) and I think this is a better way to manage this. 

### 2. The UI has changed to support the new flow. 
- The 1st tab in Sync is now called Download, the 2nd tab in Sync is now called Select. And now the sequence of tabs also makes sense. 

### 3. Now, you finally see all your releses.
- The app did not list singles or EPs in the library, this is now also fixed.
- Needed a different API endpoint that has different features and lacks track count.
- So now the track count is created from opening an album and cached. You win your missing releases. You lose upfront track counts. Seems fair.

### 4. Inverted green thingy no more
- The Watch app no longer shows an inverted green system crown indicator. I tried to correct the orientation and got nothing but app crashes. The volume bar is already a visual cue, so goodbye.

### 5. Bios
- I realised I am pulling artist bios from the API so I thought why not add it to the Artist Library view as a toggle.
- Nobody asked for it, but you might get bored and now you have something to read. 

### 6. We have codec badges everywhere now. 
- So you know if this is your lossless version or your MP3 128kbps version.

### 7. Deleted delete
- We had about 5 different delete buttons across the app. I deleted them. Now we have 2 trash icons for phone and watch in the Sync/Select screen.

## 8. Storage stats have a new home
- All under Sync:Select where you need it.
- Removed from all the other random places

---

## Version 1.0 (Build 14)

### Fixes:

1. Lazy NavigationLink for artist list (fixes app freeze with large artist lists - this is in addition to improving the server calls for the same scenario in build 13)
2. Filter out >10k track playlists (hides "All Music") - nobody needs to sync these to a watch and they cause issues

### New stuff:

1. Auto-navigate to Phone tab after downloads complete                                                         
2. “Shuffle All” button on Watch playlists and albums                                                           3. Double Tap pinch gesture for play/pause on Watch (needs WatchOS 11+, Series 9 and Ultra 2 onwards)
