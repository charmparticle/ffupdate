# ffupdate
![here's what ffupdate looks like](ffupdate.gif "ffupdate in the terminal. This gif was created using ttystudio.")

This is a shellscript for updating firefox on linux.
It checks if firefox needs to be updated, and if it does, it updates firefox. It only looks for its own installation of firefox, so if you haven't run this script before, it will try to install firefox for you.

Firefox will exist in $dir/mozilla/$flavor/firefox/firefox, where $dir is whatever you specify (I prefer /opt/mozilla myself; it just seems more correct, especially since google uses /opt/google.), and $flavor is "vanilla", "beta", "devedition", and or "nightly".

**If you chown the $dir to your user account, ie `sudo chown -R janedoe:janedoe /opt/mozilla`, then firefox will update itself, so this script isn't really needed, although it will still work. Same is true for thunderbird incidentally.**

ffupdate checks if it has permissions to create the folder structure and asks to run as root if it doesn't.

It can install vanilla firefox, developer edition, nightly, or the latest beta.

# tbupdate

I have added a separate shellscript, tbupdate, for installing and updating thunderbird.

It's nearly identical to ffupdate, so I figured I'd throw it in here.

Thunderbird will install to $dir/mozilla/$flavor/thunderbird/thunderbird

