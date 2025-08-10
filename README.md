# Sync-osu-lazer-across-devices-using-OneDrive

So as far as I know, osu! does not have an option to sync data across computers, so I came up with a solution that uses a symbolic link to make a OneDrive folder the default folder location for all of your data.

This method works for osu!lazer, but I assume that it can work for osu!stable as well with some tinkering

1. Create a OneDrive folder that will be used as the directory
2. Navigate to your osu!lazer data folder, this is usually in AppData/Roaming/osu
3. Cut and paste this data into the new OneDrive folder
4. Copy the paths of both folders and paste them into notepad or a similar text editing software
5. Delete the original osu!lazer data folder
6. Open command prompt
7. Run the command `mklink /j "original osu!lazer data path" "new OneDrive folder containing the data"` 
   (make sure to keep the parenthesis when pasting the paths)
8. Do the same thing on the other computer

If you have a Mac, there should just be an option to change the folder location to the OneDrive folder containing all your osu!lazer data

Keep in mind OneDrive is a bit slow, so it might be a second before your data is synced between your devices

I might make a tool to automate this process later, but it seems kind of unnecessary considering how simple the process is 

Feel free to copy and paste this text, or link the github in case someone else asks this question on a forum
