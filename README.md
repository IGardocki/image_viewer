# image_viewer
Practice at using pySimpleGUI to build a desktop app, then using pyinstaller to create an exe file from that app.

### Things I learned:
- pySimpleGUI defintely doesn't have the "out of the box" modern look that streamlit does (This is something I need to look into more with styling). But, it seems like using pyinstaller to package it up into one simple exe file for a user to download and use to manipulate local files is much simpler than trying to open a web app
- pySimpleGUI seems like the best choice for desktop apps, while streamlit is better for web apps
- pyinstaller is super cool. Basically takes your python script, and creates an exe file (for Windows users) that's a one-click download, and its good to go without a user having to install all the python libraries and dependancies themselves. Good for getting code out to non-devs. You run it on the python file you're looking to package up, and it creates build and dist directories in the dir you're in. Non-dev users only need to download the exe file in the dist folder, and can rock out your app!
-- Probably best to use this command, run from the dir the py file you're trying to package: pyinstaller --onefile img_viewer.py

-- This creates only one exe file, making things a lot easier

- Have not quite figured out how to use pyinstaller with streamlit yet. Seems like there's a lot of talk of forums about this, but not a clear answer that I've found yet