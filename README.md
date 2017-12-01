# libgdx-test
Base LibGDX project to prepare for LD

# Setup Instructions (Eclipse)

1. Clone the repository to any location OUTSIDE of your Eclipse workspace

2. Import > Gradle > Existing Gradle Project

3. Press "Next", then press "Browse" and select the cloned directory (Called "libgdx-test") and press "Finish"

4. Wait for Gradle to download all the dependencies. You should see "Syncronize Gradle project .." in the bottom right of your
Eclipse window. Tap the icon to the right in red to see progress.

![Image](https://i.imgur.com/EUnGnhz.png)

5. Once Gradle has completely finished, it's time to setup and run your project. Expand the "test-desktop" project, then
expand "src" and navigate to the DesktopLauncher class. 

6. Right click > Run As > Java Application. This WILL error due to the working directory not being set for this new run
configuration yet.

7. At the top of your Eclipse window, go to Run > Run Configurations. Select DesktopLauncher, then go to the "Arguments" tab.
Under the "Working directory" section here, press "Other" then "Workspace". Expand "test-core", select "assets", then click OK.

8. Press "Apply" then "Run".

![Image 2](https://i.imgur.com/Asn275J.png)

You're done! With the exception of the desktop launcher, all game code goes under the test-core project. Expand it and find the
"Game" class: This is the root of a LibGDX game.
