# ffupdate
This is a shellscript for updating firefox on linux.
It checks if firefox needs to be updated, and if it does, it updates firefox. It only looks for its own installation of firefox, so if you haven't run this script before, it will try to install firefox for you.

Firefox will exist in $dir/firefox/firefox, where dir is ~/.local/ffupdate/mozilla or whatever you specify. I prefer /opt/mozilla myself; it just seems more correct, especially since google uses /opt/google.

ffupdate checks if it has permissions to create the folder structure and asks to run as root if it doesn't.

It can install vanilla firefox, developer edition, nightly, or the latest beta.
