# Windows 10

This is a release repository for MaST Windows 10 that consist of the 4 testing application to assist TM users in troubleshooting home Unifi and Streamyx wireless router.

This document includes a tutorial on how to install a MaST Windows 10 release.

## Installation

1. Download latest installer zip file here.
1. Extract the zip file.
1. Run *.appxbundle file.
1. Follow the installation instruction.
1. Once installed, run *Mast.App* from the *Start Menu*.

> #### If this is the first time you try to install the application, you might encounter error 0x800B0109 similar to the picture below. See [Troubleshooting Error 0x800B0109](#1-error-0x800b0109) for the solution. 
> ![Error 0x800B0109](http://i.imgur.com/RxNZd51.png)

## Troubleshooting

### 1. Error 0x800B0109
This error is triggered by self signed certificates. Self signed certificates are not auto installed. You have to manually install the certificates.

#### Manually installing certificates.

1. Open the extracted installer folder.
1. Double-tap the certificate file (e.g. *Mast_1.0.23.0_x86_x64_arm_Debug.cer*) in the folder ![Certificate file](http://i.imgur.com/RyWhFoS.png) and then tap Install Certificate. ![Install certificate](http://i.imgur.com/LMQ6KSX.png) This displays the Certificate Import Wizard. ![Certificate import wizard](http://i.imgur.com/YO2kPT2.png)
1. In the Store Location group, tap the radio button to change the selected option to Local Machine. ![Local machine](http://i.imgur.com/MUZJMrh.png)
1. Click Next. Tap OK to confirm the UAC dialog.
1. In the next screen of the Certificate Import Wizard, change the selected option to Place all certificates in the following store. ![Place all certificates](http://i.imgur.com/kcvG9Fp.png)
1. Tap the Browse button. In the Select Certificate Store pop-up window, scroll down and select Trusted People, and then tap OK. ![Trusted people](http://i.imgur.com/yOYPOS1.png)
1. Tap the Next button; a new screen appears. Tap the Finish button. ![Finish](http://i.imgur.com/fqVVJd8.png)
1. A confirmation dialog should appear; if so, click OK. ![Complete](http://i.imgur.com/fx3el6C.png)

Once the certificates is installed, reinstall the application. 
