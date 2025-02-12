Hi, this is a rough tutorial how to create AAPS WITHOUT ANDROID STUDIO

#0 You need to fork the project from the official repository. To do this, go to this page https://github.com/nightscout/AndroidAPS and click the 'Fork' button on the right-hand side.

#1 go to Settings (top bar on your project page)->Secrets and variables->Actions->New repository secret

#2 Name secret 'SIGNING_KEY' and in text area paste your keystore (you can cat it, or open with notepad, copy and paste values)

#3 Click on Actions (top bar)

#4 Search for android

#5 Click configure

#6 paste content from https://github.com/msarna/AndroidAPS/blob/master/.github/workflows/android.yml to textarea 

#7 Adjust 47 line (replace msarna with your keystyore alias) and 48/49 with your keystore password

#8 Click commit changes

#9 Under actions you should see workflow run

#10 when it is finished and green, you should be able to download "APK release generated" 

#11 unpack it, and transfer as you usualy do file 'app-full-release-unsigned-signed.apk'
