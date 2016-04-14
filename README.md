# ffupdate
This is a shellscript for updating firefox on linux.
It checks if firefox needs to be updated, and if it does, it tries to create a folder, ~/ffupdate/mozilla (or some folder you specify in the script), and if it succeeds, it untars firefox there. It only looks for its own installation of firefox, so if you haven't run this script before, it will try to install firefox for you.

Firefox will exist in $dir/firefox/firefox, where dir is ~/ffupdate/mozilla or whatever you specify. I prefer /opt/mozilla myself; it just seems more correct, especially since google uses /opt/google.

ffupdate checks if it has permissions to create the folder structure and asks to run as root if it doesn't.

It can install firefox, aurora (the developer addition), or nightly. If an unbranded edition comes out, I'll add that to the script. aurora or nightly get installed in $dir/aurora or $dir/nightly.
