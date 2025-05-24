# Bot Commands

Here is a list of all the commands you can use with the bot. Remember to start commands with `/` in Discord.

## Playback Control

*   `/join`
    *   Makes the bot join the voice channel you are currently in.

*   `/leave`
    *   Makes the bot leave its current voice channel.

*   `/play <query>`
    *   Plays a song or adds it to the queue. The `query` can be a song name to search on YouTube or a direct YouTube video URL.

*   `/pause`
    *   Pauses the song that is currently playing.

*   `/resume`
    *   Resumes playback if the music is paused.

*   `/skip`
    *   Skips the current song and plays the next one in the queue (if any).

*   `/stop`
    *   Stops the music completely, clears the entire queue, and the bot stops playing.

*   `/volume <level>`
    *   Changes the bot's playback volume. The `level` should be a number between 0 (silent) and 100 (loudest).

## Queue Management

*   `/queue`
    *   Shows the list of songs currently waiting in the queue, including the song that's playing now.

*   `/nowplaying`
    *   Displays detailed information about the song that is currently playing.

*   `/loop <mode>`
    *   Sets how songs should loop. Choose a `mode`:
        *   `Off`: No looping (default).
        *   `Loop Current Song`: Repeats the current song forever.
        *   `Loop Entire Queue`: When the queue ends, it starts again from the beginning.

*   `/shuffle`
    *   Randomly shuffles the order of the songs currently waiting in the queue (doesn't affect the currently playing song).

## Information

*   `/lyrics`
    *   Tries to find and display the lyrics for the song that is currently playing. (Note: This might be disabled if the bot owner hasn't set up the required API keys).

## Playlist Management

These commands are part of the `/playlist` group. Start them like `/playlist create`, `/playlist add`, etc.

*   `/playlist create <name> [public]`
    *   Creates a new personal playlist with the given `name`. You can optionally set `public` to `True` if you want others to be able to see and load it (default is `False` - private).

*   `/playlist delete <name>`
    *   Deletes one of your playlists specified by its exact `name`.

*   `/playlist list [user]`
    *   Shows a list of your own playlists. If you provide a `user`, it shows that user's public playlists instead.

*   `/playlist show <name> [user]`
    *   Displays the list of songs inside a specific playlist named `name`. Use the optional `user` argument to view someone else's public playlist.

*   `/playlist add <playlist_name> <query>`
    *   Adds a song to one of your playlists. Specify your `playlist_name` and the song `query` (YouTube URL or search term).

*   `/playlist remove <playlist_name> <song_number>`
    *   Removes a song from your playlist. Specify the `playlist_name` and the `song_number` (the position number you see when using `/playlist show`).

*   `/playlist load <name> [user]`
    *   Adds all the songs from the specified playlist `name` to the end of the current server queue. Use the optional `user` argument to load someone else's public playlist.

*   `/playlist savequeue <name> [public]`
    *   Saves all the songs currently in the server's queue (including the one playing) as a new playlist under your name. Specify the `name` for the new playlist and optionally set `public` to `True`.

*   `/playlist privacy <name> <is_public>`
    *   Changes whether one of your playlists (`name`) is public or private. Set `is_public` to `True` to make it public, or `False` to make it private.

