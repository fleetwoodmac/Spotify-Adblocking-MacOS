# Spotify Adblocking on MacOS

## Notes

A short discussion created **purely for educational purposes.**

## In a browser

1. Download Firefox or a Chromium based browser such as [ungoogled chromium](https://github.com/Eloston/ungoogled-chromium#automated-or-maintained-builds) or [Brave](https://github.com/brave/brave-browser)
2. Install [uBlock Origin](https://github.com/gorhill/uBlock) (chrome store)
3. Log into to Spotify's webplayer (open.spotify.com)
4. Enjoy


## As a "native app"

There is no equivalent to BlocktheSpot or similar on MacOS currently. If you want a "Native App" for Spotify with adblocking, the best way to achieve this is by using a Progressive Web App. **Brave can be used for this strictly due to its ease of creation**. Alternatives are out there, but most are single site browser creating apps that use Electron, but do not support extensions yet. Coherence X does not work properly for Spotify even though it does support extensions.

1. Download [Brave](https://github.com/brave/brave-browser)
2. Install [uBlock Origin](https://github.com/gorhill/uBlock) (chrome store)
3. Log into to Spotify's webplayer (open.spotify.com)
4. Click the burger icon (three horizontal lines) on the right side and click "Install Spotify" (above 'More Tools'). Click Install. _Below is an example shown for YouTube._
![test](https://user-images.githubusercontent.com/69140036/148520268-5513bfe5-1565-4359-aa5a-19680187e1b6.png)

5. Note that Web Apps are stored at /Users/YOUR_USERNAME/Applications/Brave Browser Apps

6. There should now be a window open with the Spotify webplayer and a Spotify icon in the Dock. Below is how the YouTube app would look like (with extensions installed shown).

![test2](https://user-images.githubusercontent.com/69140036/148522056-de505e5c-bee2-4a2e-bb9c-16697af205f6.png)

7. Pin the app to your dock for easy access if you wish. Below is an example with the created YouTube app.

![test3](https://user-images.githubusercontent.com/69140036/148522764-592f82bb-7099-4d82-8f01-2dca8f8376ed.png)

### Annoyances with this method

- Every time the Spotify app is started, Brave will also start, as the PWA depends on brave to be running. You can close any Brave windows that come up and just leave the Spotify window open while you play music.
- To uninstall any PWA you create with Brave click the burger icon in the PWA and click uninstall. Below is an example with the YouTube app.
![test4](https://user-images.githubusercontent.com/69140036/148523348-c27aa824-9439-40e3-94b2-cd1c79393f2a.png)

### Solutions to Annoyances

1. You can use the provided [Alfred Workflow](spotify_workflow.alfredworkflow) if you have Alfred and a Powerpack license. Just download it and double click to import it into Alfred. The usage is described in the 'about' section of the workflow but essentially 
   - the keyword **lspot** launches the Spotify PWA and closes the Brave window that opens up upon launch
   - the keywork **kspot** kills the Spotify PWA by killing the Brave application

2. If you don't have Alfred you can use Automator (default application that is included with every macOS install) to create an application that launches Spotify and closes the Brave window, and a hotkey combo/macro or second application that closes Spotify by killing Brave. Below is an example program that launches the Spotify PWA and gets rid of the Brave window.

![test5](https://user-images.githubusercontent.com/69140036/148635333-7a939dc8-698a-4d85-a337-c11554aac7ec.png)

Here is another example program to close Spotify by killing Brave

![test6](https://user-images.githubusercontent.com/69140036/148635513-6c78ee01-16bb-4ba1-b02a-d2732aed53df.png)


