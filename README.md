# ScrobblerBrainz
A MusicBee plug-in to scrobble tracks to ListenBrainz. Forked to further support ListenBrainz features such as MBID submitting.

# Restrictions
1. Works better than the last.fm scrobbler, even tracks shorter than 30 s. are scrobbled.
1. ~~No MBIDs in the scrobble. MusicBee doesn't expose them in the API.~~ **MBIDs are submitted using TagLib#**
1. No playcount sync.
1. ~~No "now listening".~~ **This version submits "now listening", with MBIDs!**
1. No liking of tracks.

# Notes
Not all MBID tags can be retrieved. TagLib# has updates to support multi-value tags easier on certain formats, but they haven't pushed out a new release yet. I'll see what I can do, but until then, AAC and ASF tags (iTunes and Windows Media, respectively) can only retrieve one artist MBID. This is fine, however, as ListenBrainz will complete the rest as long as the recording MBID is present.

# Download
https://github.com/Viktini/ScrobblerBrainz/releases/tag/v1.1.1-mbid_submit

# Usage
1. Get MusicBee https://getmusicbee.com/downloads/
1. Get MusicBrainz account https://musicbrainz.org/register?uri=%2F
1. Get ListenBrainz account https://listenbrainz.org/login/
1. Download the plugin to *Plugins* folder in your MusicBee instalation folder
1. Get your ListenBrainz user token https://listenbrainz.org/profile/
1. Start MusicBee and enable the plugin in *Edit->Edit preferences->Plugins*
1. Input your user token into the toolbox
1. Save the settings and you're good to go
