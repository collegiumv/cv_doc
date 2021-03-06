# User Preferences

One of the features of CVOS is its deep customization potential.  All accounts are provisioned with sane defaults; however, some of the more common changes available are documented here.

## Graphical Session

By default, CV accounts use the Cinnamon desktop and in rare cases where hardware acceleration is not available, may fall back to the cinnamon2d desktop.  If you would prefer a different desktop environment, you are free to choose from any of our installed environments using the command line utility `modsession`.  Currently the following environments are installed, though only Cinnamon receives support from the CV Admins team.  All other options will be supported on a best-effort basis.

* Cinnamon (default)
* XFCE
* LXDE
* OpenBox
* Awesome
* i3

A brief description of each:

* Cinnamon - This environment uses modern style and flat elements with rounded corners for a sleek and styled experience.  It features a menu in the lower left hand corner, which can be accessed by pressing the mod4 key (Windows Key) on the keyboard as well as clicking on it.  The menu is text search-able and sorted by category.  Additionally mod4 + arrow keys will snap windows to the side of the screen gestured by the arrow key.  The clock by default will use 24 hour time but this can be changed by right clicking it.
    * Notable features
        * The default desktop wallpaper changes through the day to be darker at night.
        * Apps snap to the top and bottom of the screen allowing for horizontal splits.
    * Most Frequent Complaints
        * Cinnamon is slow to load (~5 seconds).
        * Program icons are sometimes missing in the menu
* XFCE - A much older environment that focuses more on efficiency and speed over looks.  Though it has a slightly dated appearance, many more modern themes are available for those that like a newer look. Users of Apple's OS macOS will likely appreciate XFCE's dock for frequently used applications.
    * Notable Features
        * This is the only environment that includes a dock by default.
        * XFCE has been around for many years, thousands of themes are available.
    * Most Frequent Complaints
        * The default interface feels dated.
        * Customizing XFCE is non-obvious.
* LXDE - Literally the "Lightweight X11 Desktop Environment," this environment was built to be nimble and quick.  Running on our high performance hardware, menus respond almost instantly and programs load quickly.  Most aspects can be changed simply by right-clicking.  A variant of LXDE was previously the default environment in the 2015-2016 school year.  This environment also has a distinctly "Windows XP" feel to it, with its fully text based menu and relatively simple styling.
    * Notable Features
        * Very fast.
        * Easily customized through right-clicking.
    * Most Frequent Complaints
        * The default desktop looks horrific
        * Programs aren't always where you might expect in the menu.
* OpenBox - The most minimal windowing environment that isn't based on tiling.  Once launched, you are provided with a default gray background.  Right-clicking gives the menu which contains programs.  This is the fastest non-tiling environment.
    * Notable Features
        * Very light and distraction free
        * Insanely fast
    * Most Frequent Complaints
        * Too minimalist
        * Not very intuitive.

The final environments from the list (Awesome and i3) fit into a different category called "tiling window managers."  The operation of this category is usually highly user-specialized, but tends to be entirely keyboard driven, focused on maximum productivity, and very minimalist.  Because these environments are so customize-able, the operation and configuration thereof is considered beyond the scope of this article.

If your preferred environment is not listed above, feel free to [ask](bugs-and-features.md#feature-requests).  The only environment at this time which is specifically disallowed is KDE, as it does not play well with others.

## Authorized Keys

If you intend to make use of our remote access server, then you'll need to install at least one authorized key.  To do so use the command `modpubkeys` in a terminal while logged in to a lounge workstation.  This will open your $EDITOR or vi, by default.  Paste in your public key and save the temporary file.  You should see that your record is updated and your key will instantly be available for use.

## Locking your screen

By default your screen will lock after 10 minutes of inactivity.  If you wish to lock your screen before you get up, there is an icon to do so in the main menu located in the lower left corner.  When you return you can press any key to wake up the terminal and use your password to unlock the screen.  Screens may be locked for a maximum of 45 minutes and applications will be forcibly closed at the end of this interval.  Screen locking is meant as a convenience for short intervals where it is necessary to step away from the computer, not for long periods of inactivity.
