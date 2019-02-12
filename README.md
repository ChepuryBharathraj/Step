# Step

**Directory Structure**

We designing structure to modularise and easy to maintain.

First create a folder in the root called “app”.

Create folders inside app:

**assets** — In this sub folders are: fonts, icons and images

**components** — In this all shared React components will be created. Usually these components are the ones that we call “dummy”, 
that have no state logic and can be easily reused across the app.

**views** — These are our application screens, the ones that we navigate from one to another. 
These are also React components, but they are the ones that we call containers, because they contain their own state.

**modules** — There are pieces that have no corresponding view part (JSX). 
Typical examples of that is the colors module (contains all the app colors) and 
the utils module (contains utility functions that are being reused).

**services** — These are the functions that wrap the API calls.

**i18n** — These are the translation strings for users of different language and locale

All apps require some type of configuration, so I usually create a file called config.js and put it in there. 
If the configuration file reaches a lot of lines, we can then create a config folder and separate the config in files.

For state manager library, we used 3 folders, one for actions, reducers and providers. 

