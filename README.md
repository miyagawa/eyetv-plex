## EyeTV - Plex renamer

This tiny Ruby script scans "EyeTV Archive" folder for new recordings, and makes a symlink in the Plex TV folder with Plex's default scanner friendly filename, such as:

    Show Name/2013/Show Name - 2013-01-02 - Episode Title.m4v

TV show titles and subtitles are parsed from EyeTV's own metadata. You're recommended to scan the created symlink folder with "Plex Series Scanner" and "Personal Media Shows" metadata agent for TV Shows.

By default, the script will look for `~/Documents/EyeTV Archive` for EyeTV recordings and creates a symbolic links in `~/Movies/TV Recordings` folder. You can change them with `EYETV_ARCHIVE` and `PLEX_FOLDER` environment variables.

It is required that you configure EyeTV to export the recordings in the same directory for iOS access. I set to the iPad 720p format which plays nicely with Plex.

You can run this script periodically via crontab, or triggerd from `ExportDone` event [using EyeTV AppleScript integration](http://support.elgato.com/index.php?_m=knowledgebase&_a=viewarticle&kbarticleid=2727) (which I've personally never have managed to work).

## Author

Tatsuhiko Miyagawa

## License

MIT



