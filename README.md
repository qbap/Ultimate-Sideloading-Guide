# Verified to be working with many users reporting valid results

Disclaimer: This costs me money! While I can easily afford this, I'd really appreciate some sort of donations, even if it is 50cents lol. Thank you!

[Here](https://shorturl.at/82U3M) is the PayPal donation link! 

This will help me keep this service free and not charge $20 like signing services

## Introduction
Hello, Welcome to my guide on how to sideload on Apple Devices using a method I came across to a while back. This sideloading method has worked for long periods of time, without any app limits and without a pc. I eventually found some small let-downs such as the go-to DNS at the time was and is still made by some random Vietnamese guy with no open-sourced data which naturally has some privacy concerns. ESign also had undesirable analytics which are now blocked by my DNS.

After a few months of using both of these services I decided to reverse-engineer the DNS and how the enterprise signed ESign was downloaded over the web with the click of a button. With enabling better preventions against revokes unlike other people who keep on using other people's DNS and put no effort in themselves with bad instructions to say the least. 

My DNS is compatible with other services such as Scarlet, Feather and any other enterprise signing app, More info [here](#scarlet-feather-and-other-sideloaders)

If you are new to sideloading, Please read the [wiki](#wiki) and learn about simple terms in the world of sideloading.

Without further ado, welcome to my Ultimate Sideloading Guide, if you have any issues, requests or ideas please make an issue here on GitHub.

## Scarlet, Feather and other sideloaders
My DNS is compatible with all services as long as they rely on enterprise certificates to install.

Follow Part 1 of my main guide to install the DNS blocker for these services.

You do not need to follow Part 2, 3 and 4 as these install ESign itself.

## How does this method work?
By using leaked business enterprise certificates, We can sign apps using their credentials which means Apple lets us install the apps without any hassle, however after a while Apple revokes the certificate, this is where the WhySooooFurious DNS Blocker comes in, the DNS blocker blocks Apple servers from contacting your device about the expired/revoked/blacklisted certificate which in turn lets you use the apps for however long you'd like. The DNS also blocks ESign analytics.

## Before we start
- This will NOT unrevoke your apps!
- Make sure you have not been using services such as Scarlet and Feather before as the certificates used to install ESign on your device might be revoked! 
- If you are blacklisted from Apple for already using services such as Scarlet and Feather you will need to follow this [guide](#revoked-or-blacklisted)
- This method will work as long as you read and do all of the steps required

## Compatibility
This should work for all iOS, iPadOS and even macOS devices, on the latest versions of all iOS, iPadOS and macOS.

Versions that might not be supported are below iOS 12, iPadOS 13 and macOS 11.

## Part [1/4] Installing the WhySooooFurious DNS Blocker
1. Go down to [Downloads](#downloads) and click on the WhySooooFurious DNS Blocker, allow the download and close the prompt
2. Now, open settings and go to General > VPN & Device Management
3. Click on the downloaded profile and install it, you may need to input your password
4. The DNS should now automatically be enabled, Do not change the DNS settings to automatic otherwise your apps will get revoked!
5. Now, go back and then go to General > About > Certificate Trust Settings
6. Enable Full Trust for the NextDNS Root Certificate, if Full Trust does not show you cannot use VPNs at all
7. Continue onto [Part 2](#part-24-installing-esign)
 if you want to install ESign

## Part [2/4] Installing ESign
1. Go down to [Downloads](#downloads) and click on ESign Direct Install
2. Click on install once the popup comes up
3. Open settings and go to General > VPN & Device Management > HDFC Life Insurance Company Limited
4. Click on Trust at the top then click on allow, after this your device might need to be restarted
5. If your device was restarted, swipe up and click on install profile
6. ESign should now be on your home screen, fully functional
7. Continue onto [Part 3](#part-34-setting-up-esign) to setup ESign
 
## Part [3/4] Setting up ESign
1. Open ESign and accept the agreements
2. Go into settings and click on get device UDID
3. Select allow and then you should be redirected to settings
4. After opening settings go to General > VPN & Device Management
5. Install the Query Device UDID profile
6. You should be redirected back to ESign
7. Now go down to [Downloads](#downloads) and click on Certificate
9. Go into ESign settings and click on Import Resources
10. Find and select the certificate you downloaded back in Step 7 and click on Import
11. Now go over to AppStore in ESign and click on App Source
12. Click on the plus icon and paste in the sources from [here](#esign-sources), click on add all
13. You now have setup ESign with all sources ready to install apps
14. Continue onto [Part 4](#part-44-using-esign)

## Part [4/4] Using ESign
1. Download any app using the AppStore in ESign or you can import your own .ipa using Import Resource in which case you can skip to step 4
2. Check the download status in the Download tab if downloading from the ESign AppStore
3. Click on the download and select Import App Library
4. Your app should now be visible in the Unsigned Apps tab, select unsigned or signed by selecting the bar on top of ESign
5. Click on the app and select Signature
6. You can change your app and edit it here
7. Select Signature and ESign should sign the app using the certificate you selected before
8. There might be red text saying this certificae is revoked, this is normal! Click on the blue button saying install, then click install on the prompt again
9. The app should be on your homescreen now
10. Open settings and go to General > VPN & Device Management
11. Select the app you installed and click on Trust
12. Click on allow, after this your device might need to be restarted
13. If your device was restarted, swipe up and click on install profile
14. The app should now be on your home screen, fully functional
15. Now read the [Post Install Notes](#postinstsllnotes)

## Post-Install-Notes
- You must never disable the DNS otherwise your apps will get revoked almost instantly
- Don't exit ESign while the app is being signed
- Don't use Cowabunga Lite otherwise the DNS will disappear! There is a workaround, i'll make a guide soon

## Downloads
[WhySooooFurious DNS Blocker](https://shorturl.at/fwIJk)

[ESign Direct Install](https://shorturl.at/Jx5gX)

[Certificate](https://shorturl.at/xs6K8)

## Questions/Answers

**Q -** Won't a VPN bypass the DNS and revoke my apps?

**A -** It shouldn't , based on the settings I used, I do not recommend using a VPN. If you really want to use a VPN, Use this [guide](#using-a-vpn)

---

**Q -** Will a restart bypass the DNS and revoke my apps?

**A -** Simple answer, No.

---

**Q -** OMG, Are you going to track my furry content?

**A -** No, I have no need to look at your expenditures.

---

**Q -** Um, I'm a cocky big-time dev and I need to look at your code thingies to ensure they don't have viruses.

**A -** Sure, Go over [here](https://shorturl.at/zHEbJ) to look at what is used in the process!

---

**Q -** Can I see the NextDNS settings used?

**A -** Yes, make an issue and mention your email and I will send you a viewing invitation if you're that paranoid.

---

# Miscellaneous Guides

## Using a VPN 
So you want to use a VPN with the DNS blocker, follow the steps below and you should be able to use your VPN normally and on-demand, I still do not recommend using a VPN with the DNS, You should know how to configure your VPN's DNS server yourself as there are different steps for each VPN app.

### Method 1
1. 45.90.28.51 and 45.90.30.51 are the DNS servers you need to replace in your VPN's settings

## Revoked? or Blacklisted?
So you've gotten yourself blacklisted, either from my DNS (which seems very unlikely) or from another creator's DNS. Follow the methods listed below and you should be unrevoked. 

Use Method 2 if Method 1 does not work.

You must not use your backups with Method 2 otherwise you will get revoked again.

### Method 1
1. Back up your device, here is a [guide](https://support.apple.com/en-us/118426)
2. After backing up, reset your device, here is a [guide](https://support.apple.com/en-au/guide/iphone/iphea1c2fe48/ios)
3. Now if you have an iCloud backup you should be prompted to restore from your backup after logging in to your Apple ID, if you have a local backup all you need to do is plug your phone in, go on either Finder for macOS or iTunes for Windows and click on restore backup from your device's menu
4. Then follow the guide for Part 1 of the WhySooooFurious DNS Blocker to prevent revokes in the future

### Method 2
1. Follow this [guide](https://support.apple.com/en-au/guide/iphone/iph7a2a9399b/ios)
2. Then follow the guide for Part 1 of the WhySooooFurious DNS Blocker to prevent revokes in the future

## ESign Sources
My sources for ESign                    
###
    source[5GHxhb1U7Lc5jIMpumASbN2teg9dyK5EAazzwnfm1/gPKQPTWzcz/GqmMyJ96qOpN9I+sobaxc2bOxLJOnEOvCBO0S3fPLfBifsFqblxWBSpvpIt92QQghflQC3w+Exfmk/TRgDUpbmR0WYET6IlVgzUUt7zvQnk7OiXHlKE211IckI8xJGGbC6i4pHK7a2i7uAzEJjZ612XcSAUVA/z9d09OYgTx3UQwP6vQ6pG/tTT6Miy/oiQOfn4EY1keR6ER2m4J09StZmkEnFVBn2x+CED9WuUY6lqPIE/qSQ+ituWE6E67AbhSk4crGGNzlcO9PoeyHjGA3w+SQVoiVbgetHxdx0c4fdqt+GG0vZvZK7TLp7iWFgDcewQhC9MEOuzVfQy267Uy7Ag6VAw37qcUP/WJOkbUuFRGUgICFesTlR1BDRsQyOmT3jek2XBLBC8nVR7EQlgm6Ggkf3bOhm3OBi/dHxwbtB4zPa8l3TyAwp8rhDwsE493pH84s84Bfws5KQNh2/XQRVRL4CwnkUe1eljMIZgewKrS0GR37coqecAkiPJNnurDLN0nqf5ddRd0d3+9wl40Q8LPv2vuBWk0mqwlgDaLwmJK1ZmT/ikcagjd79u3RoQo3uSZHJbGPA/WoDgxLHGPcPgC0DgzBu3/8D1dmp3nzzUtNppbr7IJkdmizglxmitKG6jbbMylxEDcBcu/b33wu2E8AsL31mmxXCHk8oqylqP8QscHrExXuIDcPck/f7596VWXDGAWxfjRi7RdJ6ePpPY3HYYkWhXjzVgzIk4zT2+6NbCvICyYun7HjOXLPZTA1UFg32dt096Ej+W+tM6o6Ve27+XplpPdp5cBIE3kvP141ejnG76dKdUkuR+m/udL/26PSNPjbMkihWXpCUKPmV5hqbnyZQ2e4l+TelnEGOCkWFBMzgESBQkAvdvNfEgFwtYlYVcvSgYVOl4JyI8zpbQVRWBAo1ba/OJANB0JJrDSMbxfuMi4u6QDp6F1SiR9ah5Q5knGELpREQwbYPgEHalW0z5FovlNn/70jNKP8Keas8F/5g7FdfNE7Y7C/YJpcBwqfBBvP3cAZ6ZZIZIgN+BNfNrqBzCx2jBxpEj2jrujw1qUcaJ8kQj8N9aalGysKnqMaUNjm3Mi2GKSugVMZU3CmwdfAfP8Zc8y89L+Il7/EVtwDHjss8SEHMj8oKJNZT2vL7l4a8S9fr2r30wbUix/oLm1Vy7h7rFjEwCiKXc2uUZdD4bTlwjlrp99fdqxjHLvcdelq73ncgAc8MeqPXIgkLmLTVrfu4UdUfD5PYLuKC4QB62gP84QSpCW60WxImA6jR5wSVS+gu6+srQVjSajO3Z6YfxkFg2KdDqw5tbhDoDPaAgM9iWO0pjpsDyYZkWKPUSxvsO7jxLJFeWp41SaYZtIqDEt8lQMHoOzpTd282hRAxNYAbUlL1aZLMWj3Wb16ma9QR58IPsbBdHHfGZOAeQV5ASYgbflLiw581wRPtCMzlPO4LLBYnNDHPSegZz3O2zGaTj1GA+ZkYsj+j+82cqGtZQiaP5bulAie/KaYBZm2z04TVb0Ez+j6QRXAPeB80xgovZ2AEbxMdwLizDaBbGc966M8ibOY0f2xyokC1q45MaEVOSLLkfo9uVX/RKq0o0Mm54nscNJ5Oy+ewCiRaLQCiJteWNYfQEqTOb2QAVLJvl0Ts=]

## Tips & Tricks for ESign
Making use of ESign settings!

### Adding sources
Adding sources to ESign
1. Either copy a link that looks like the one above, or copy a link, note that not all links are compatible with ESign
2. Go to the AppStore tab in ESign
3. Click on App Source on the top left
4. Click the plus button on the top right
5. ESign should prompt you to paste the contents in, if not, copy in the prompt and click on add

### Exporting sources
Export selected sources from ESign.
1.  Go to the AppStore tab in ESign
2. Click on App Source on the top left
3.  Click the Select button on the bottom right
4. Select which sources you want and then click share

### Deleting sources
This will delete selected sources from ESign.
1. Go to the AppStore tab in ESign
2. Click on App Source on the top left
3. Click the Select button on the bottom right
4. Select which sources you want and then click on delete

### Enabling Auto Import
When an app is downloaded, ESign will automatically import your files into your app library.
1. Go into the Download tab
2. Click on the 3 dots on to top left corner
3. Click on settings
4. Enable Auto Import

### Enabling Auto Delete
When an app is downloaded, ESign will automatically delete the app, recommended use with Auto Import.
1. Go into the Download tab
2. Click on the 3 dots on to top left corner
3. Click on settings
4. Enable Auto Delete

### Default Sign Config
This will let you pick a predefined config for your apps.
1. Go onto the Settings Tab
2. Click on Sign Default Config
3. Change the settings as desired

### Keep Running in Background
Let ESign run in the background (won't work while signing an app) and keep ESign vertical
1. Go onto the Settings Tab
2. Enable Keep Running in Background

### Lock Vertical
Keep ESign vertical.
1. Go onto the Settings Tab
2. Enable Lock Vertical

### Change Theme
Change the ESign theme and icon, you can change the icon only when using with Altstore.
1. Go onto the Settings Tab
2. Click on Theme
3. Change the settings as desired

## Wiki

### Sideloading
The process of installing apps on iOS or iPadOS devices from sources other than the Apple App Store. This often involves using alternative methods or tools to bypass the App Store’s restrictions.

### IPA
The file format used to package iOS applications for distribution and installation. Sideloading an app typically involves downloading an IPA file and using tools to install it on the device.

### Provisioning Profile
A file that ties an app to a specific developer account and device. It includes certificates and app-specific permissions. When sideloading an app, the provisioning profile ensures the app is allowed to run on the target device.

### Enterprise Certificate
A special type of certificate used by organizations to distribute apps internally to employees. Enterprise certificates are managed through the Apple Developer Enterprise Program and allow sideloading apps outside the App Store for internal use. Misuse of enterprise certificates for distributing apps to the public can lead to revocation by Apple.

### Developer Certificate
A certificate issued by Apple to developers, used to sign apps and verify their authenticity. Developer certificates are necessary for sideloading apps through methods like Cydia Impactor or AltStore.

### App Signing
The process of applying a digital signature to an IPA file to ensure it is trusted and verified by iOS. App signing involves using a valid developer or enterprise certificate and provisioning profile.

### UDID (Unique Device Identifier)
A unique identifier assigned to each iOS device. UDIDs are used in provisioning profiles to specify which devices are allowed to run a particular app. When sideloading apps, a UDID may be required to register the device for app installation.

### Ad-Hoc Distribution
A method of distributing iOS apps to a limited number of devices for testing or internal use. Ad-Hoc distribution involves creating a provisioning profile that includes the UDIDs of the devices allowed to install the app.

### Enterprise Distribution
A method used by organizations to distribute apps internally via an enterprise certificate. This method is intended for distributing apps within an organization, not to the general public.

### App Re-signing
The process of updating an app’s signature, often done to extend the validity of a sideloaded app. Since sideloaded apps are subject to certificate expirations, app re-signing helps maintain functionality.

### Revokes/Blacklisting
Is when Apple bans the certification signature from running on your device remotely, this results with a "App integrity not verified error".

### ESign
App manager that can install apps and sign them on device, makes everything a lot easier.

### WhySooooFurious DNS Blocker
Blocks Apple servers from revoking certificates on your device.
