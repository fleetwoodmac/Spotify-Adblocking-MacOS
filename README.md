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

### Notes

- Every time the Spotify app is started, Brave will also start, as the PWA depends on brave to be running. You can close any Brave windows that come up and just leave the Spotify window open while you play music.
- To uninstall any PWA you create with Brave click the burger icon in the PWA and click uninstall. Below is an example with the YouTube app.
![test4](https://user-images.githubusercontent.com/69140036/148523348-c27aa824-9439-40e3-94b2-cd1c79393f2a.png)

