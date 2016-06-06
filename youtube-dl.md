#Mucking Around with YouTube-dl

The following command:
* downloads a playlist
* creates a folder based on the institution identifier, collection number, and playlist name
* downloads best quality video/audio files and names them according to institution identifier, collection number, playlist order, and title
* cleans up file names
* write the video description to a text file (file named according to same convention)
* write full metadata to a json file (file named according to same convention)
* write annotations to an XML file (file named according to same convention)
* download thumbnails (file named according to same convention)

   youtube-dl -o 'pstsc_[collection number]_%(playlist)s/pstsc_[collection number]_%(playlist_index)s_%(title)s.%(ext)s' [URL] --restrict-filenames --write-description --write-info-json --write-annotations --yes-playlist --write-all-thumbnails

