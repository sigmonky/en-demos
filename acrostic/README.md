# Acrostic
This is a tiny web app that hides secret messages in playlists. The is online at [Acrostic Playlist Maker](http://static.echonest.com/demo/acrostic/acrostic.html).  

The app doesn't make any direct calls to The Echo Nest API. Instead it uses precrawled songs sets organized by genre. Each set is about 1000 songs in size. Frequency of the first letter in each song (which is used to create the Acrostic) matches [English letter frequency](http://en.wikipedia.org/wiki/Letter_frequency). To add a new genre crawl the song set with the build_precache.py python script like so:

    % python build_precache.py 'alternative rock'
   
add the output to the 'js' directory and add the genre name to the list of predefinedGenre found in the fetchGenres() method in acrostic.html/var/folders/_s/7bq8ytj94234xv01jh4p_5fw0000gn/T/com.skitch.skitch/Acrostic_Playlist_Maker.png