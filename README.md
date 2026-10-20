# LG TV Remote

A one-page web remote for an LG webOS TV. Open it on an iPhone that's on the same WiFi as the TV.

**Live page:** https://utdred.github.io/lg-remote-app/

## Setup (once)
1. Open the page in Safari and enter the TV's IP address (TV: Settings → Network → Wi‑Fi → Advanced settings).
2. Tap the TV's secure address link the page shows, then accept Safari's certificate warning (the TV uses a self-signed certificate).
3. Tap **Connect** and accept the prompt on the TV.
4. Share → **Add to Home Screen**.

## Notes
- Talks to the TV directly over your local network (`wss://<tv-ip>:3001`); nothing goes through a server.
- It can turn the TV off but not on (web pages can't send Wake-on-LAN).
- The pairing manifest comes from the open-source [lgtv2](https://github.com/hobbyquaker/lgtv2) library.
