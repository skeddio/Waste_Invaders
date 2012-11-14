Instructions if you experience a black screen after the intro splash screen : 

1. In Flash Builder 4.6, when exporting your final binary, the folders "assets" and "AppIcons" may not show up in the "Packaged content" panel.
2. This can cause your build not to embed the dependencies (icons and textures) and cause a black screen after the intro (caused by missing dependencies).
3. To workaround this, click "Back" on the "Export Release Build" window, then go to Windows Explorer (Windows) or Finder (MacOS) and look for the "bin-release-temp" directory.
4. Copy all the necessary dependencies (here assets and AppIcons folder) in there ("bin-release-temp"). 
5. Once copied, just go back to the "Export release build" window and click "next", you will then see all the files you added in the "package contents". 
6. Now the required dependencies will be packaged in the final build.