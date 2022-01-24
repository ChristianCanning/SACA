# Students Against Cruelty to Animals (SACA) Website

This website is built with the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes).

---

## Calendar

I have a [herokuapp server](https://saca-calendar.herokuapp.com/) which pulls the latest events from the SACA GroupMe and stores it as an ics feed.
The SACA website then embeds a Google Calendar that pulls the ics feed from the herokuapp website to display it. 
To get around Google's slow update time on pulling ics feeds (limited to about once or twice per day), I am running [GAS-ICS-Sync](https://github.com/derekantrican/GAS-ICS-Sync) through [Google Apps Script](https://developers.google.com/apps-script) on the Google account which stores the calendar. This script
forces the Google Calendar to repull the ics feed every minute.