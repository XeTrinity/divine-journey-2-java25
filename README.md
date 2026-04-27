
# Divine Journey 2 Java 25 Install Guide

The steps and versions below are what I used to successfully install Java 25 on both the client and server for Divine Journey 2 - 2.23.1.

NOTE: this was done with by piecing together guides and trial and error, it's not perfect.
eventually when I have the time i would love to test each newer version or alternatives to outdated mods to figure out which ones improve performance, gameplay or fix bugs and hopfully get them pushed into the actual DJ2 pack.

NOTE 2: You can also just use the Cleanroom Relauncher and avoid steps 3 and 4 (I'll better list the steps later on... maybe)

## Client Install


1. Download and Install [Prism Launcher](https://prismlauncher.org/download/windows/).

2. Add a new instance and Install Divine Journey 2 - 2.23.1 



3. Download and import [Cleanroom-MMC-instance-0.5.7-alpha](https://github.com/CleanroomMC/Cleanroom/releases) into Prism Launcher.


4. Copy or move the `minecraft` folder from the Divine Journey 2 instance to the Cleanroom instance.

5. Within the Cleanroom instance, go to Settings → Java, then click "Open Java Downloader". 
Select Adoptium → Java 25 → 25.0.2.10, and download it.
After the download completes, click "Detect" and select 25.0.2.10.

6. Delete these mods from the `mods` folder.
- groovyscript-1.3.4.jar


7. Download and Install these mods into the Cleanroom `mods` folder:
- [+Fugue-0.23.4.jar](https://www.curseforge.com/minecraft/mc-mods/fugue/files/7853971)
- [Scalar Legacy-1.0.1.jar](https://www.curseforge.com/minecraft/mc-mods/scalar-legacy/files/6842491)
- [groovyscript-1.4.1.jar](https://www.curseforge.com/minecraft/mc-mods/groovyscript/files/7813868)

(Optional but highly recommended — I saw big performance gains NOTE: I havent had time to test so idk what ones are the best for performance.)

- [Fixeroo-2.3.6.jar](https://www.curseforge.com/minecraft/mc-mods/xp-orb-clump/files/7095475)
- [StellarCore-1.5.22.jar](https://www.curseforge.com/minecraft/mc-mods/stellarcore/files/6480479)
- [loliasm-5.31.jar](https://www.curseforge.com/minecraft/mc-mods/lolasm/files/7671063)
- [gnetum-1.3.5.jar](https://www.curseforge.com/minecraft/mc-mods/gnetum/files/7753856)
- [RenderLib-1.12.2-1.4.5.jar](https://www.curseforge.com/minecraft/mc-mods/renderlib/files/6461209)
- [Nothirium-1.12.2-0.4.9-beta.jar](https://www.curseforge.com/minecraft/mc-mods/nothirium/files/7441674)
- [naughthirium-2.3.0.jar](https://www.curseforge.com/minecraft/mc-mods/naughthirium/files/6473489)
- [EntityCulling-1.12.2-6.5.0.jar](https://www.curseforge.com/minecraft/mc-mods/entity-culling/files/6215595)

You may need to add/ replace these in order for the above optional mods to work.
- Clumps-3.1.2.jar
- fermiumasm-5.28.jar
- JEI-Utilities-1.12.2-0.2.12.jar
- jei_1.12.2-4.16.1.302.jar
- NotEnoughIDs-1.5.4.4.jar
- spark-forge.jar

- [HadEnoughItems_1.12.2-4.29.15.jar](https://www.curseforge.com/minecraft/mc-mods/had-enough-items/files/7515497)
- [RoughlyEnoughIDs-2.3.0.jar](https://www.curseforge.com/minecraft/mc-mods/reid/files/7801299)
- [JEI-Utilities-1.12.2-0.2.13.jar](https://www.curseforge.com/minecraft/mc-mods/jei-utilities/files/6937116)
- [flare-0.7.0.jar](https://www.curseforge.com/minecraft/mc-mods/flare/files/6598523)


## Server Install

1. Download [cleanroom-0.5.7-alpha-installer.jar](https://github.com/CleanroomMC/Cleanroom/releases)

2. Run the installer .jar and select your server folder, and click "Install".

3. Edit launch_config.ini and update the values as shown below:
```
FORGE_JAR=cleanroom-0.5.7-alpha.jar
JAVA_VERSION="Path to java\eclipse_temurin_jre25.0.2+10\bin\java.exe"
JAVA_PARAMETERS=-XX:+UseCompactObjectHeaders -XX:+UseZGC
```

# JVM Arguments

Use these on both Client & Server.

`-XX:+UseCompactObjectHeaders -XX:+UseZGC`
