## EyeTV - Plex renamer

This tiny Ruby script scans "EyeTV Archive" folder for new recordings, and makes a symlink in the Plex TV folder with Plex's default scanner friendly filename. TV show titles and subtitles are parsed from EyeTV's own metadata.

By default, it will look for `~/Documents/EyeTV Arhive` for EyeTV recordings and creates a symbolic links in `~/Movies/TV Recordings` folder. You can change them with `EYETV_ARCHIVE` and `PLEX_FOLDER` environment variables.

It is required that you configure EyeTV to export the recordings in the same directory for iOS access. I set to the iPad 720p format which plays nicely with Plex.

You can run this script periodically via crontab, or triggerd from `ExportDone` event [using EyeTV AppleScript integration](http://support.elgato.com/index.php?_m=knowledgebase&_a=viewarticle&kbarticleid=2727)

## Author

Tatsuhiko Miyagawa

## License

MIT



