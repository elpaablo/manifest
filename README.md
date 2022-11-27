<p><b>Alpha AOSP</b></p>

<p>Alpha is a custom AOSP ROM based on Pixel Experience, with a vanilla variation, using RiceDroid core AOSP apps and a customized version of Lineage Trebuchet. Memory optimizations and performance tweaks are ported from RiceDroid and ProtonAOSP. Extra features are cherry-picked from other custom ROMs and adapted to our needs.</p>

<p>Credits:</p>

<p>* Base:<br/>
** Pixel Experience (https://github.com/pixelexperience)<br/>
** RiceDroid (https://github.com/RiceDroid)<br/>
** LineageOS (https://github.com/LineageOS)<br/>

<p>* Performance tweaks:<br/>
** RiceDroid (https://github.com/RiceDroid)<br/>
** ProtonAOSP (https://github.com/ProtonAOSP)</p>

<p>* UI:<br/>
** dotOS (https://github.com/dotos)<br/>
** xdroidOSS (https://github.com/xdroid-oss)<br/>
** NusantaraProject (https://github.com/NusantaraProject-ROM/)</p>

<p>* Extra features:<br/>
** RiceDroid (https://github.com/RiceDroid)<br/>
** crDroid Android (https://github.com/crDroidAndroid)<br/>
** Spark OS (https://github.com/spark-rom)<br/>
** VoidUI (https://github.com/voidui-tiramisu)</br>

<p>* Alpha logo:<br/>
** berkahjaya (https://stock.adobe.com/pt/contributor/210355228/berkahjaya?load_type=author&prev_url=detail)<br/>
** nexusby (https://stock.adobe.com/pt/contributor/204357292/nexusby?load_type=author&prev_url=detail)</p>


### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/elpaablo/manifest -b default

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```

