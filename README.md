# Prerequisite

Before running any of the following, you'll need to make sure you have Notepad++
setup as the default application for opening any file (.txt, .html, .json, etc)

# How to install

Simply drag the `file.ico` icon into the C:\Program Files\Notepad++\ directory.
Once that is done, just run the `setup.reg` file to setup the registry key to
point to the new icon file.

If your path to Notepad++ isn't in the program files folder, you'll need to
go about the setup slightly different.

# How to install manually

Make sure to store the `file.ico` file anywhere that won't get deleted. Once
done, make sure you take note of the path to the icon.

Next you'll want to open up regedit, which you can do by just opening run
with Win + R, and then typing regedit. Inside of regedit you'll want to
navigate to the following directory

`Computer\HKEY_CURRENT_USER\Software\Classes\Applications\notepad++.exe\`

Once inside, right click notepad++.exe and create a new key, and call it
`DefaultIcon`. Once done, click on the new folder/key, and on the right,
double click the `(Default)` option, and for ValueData, paste in your path
to the `file.ico`.

Once done you just need to restart explorer or wait until Windows naturally
refreshes the icon data.