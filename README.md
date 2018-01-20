# Pro-Tips

Collection of nifty little tricks and tips that will make your tech-life so much easier.

---

# Table of Contents

- [Web Servers](#web-servers)
  - [Static Files](#ws-static-files)
- [Android](#android)
  - [Enable USB Debugging](#android-enable-usb-debugging)
  - [Booting to Recovery or Bootloader](#android-reboot-recovery)
- [Git](#git)
  - [Amend](#git-amend)
- [Security](#security)
  - [Losing 2FA](#security-losing-2fa)
- [macOS](#macos)
  - [IP Address](#macos-ip)
- [Visual Studio Code](#vscode)
  - [Markdown](#vscode-markdown)
- [License](#license)
- [Contributing](#contributing)
---

<a id="web-servers"></a>
## Web Servers

<a id="ws-static-files"></a>
### Static Files

You can use a one-line Python command to start a static file-server in any directory.

Python 2.x: `python -m SimpleHTTPServer <port - defaults to 8000>`

Python 3.x: `python -m http.server <port - defaults to 8000>`

---

<a id="android"></a>
## Android

<a id="android-enable-usb-debugging"></a>
### Enable USB Debugging

A good practice is to enable USB Debugging on your Android phone as soon as you get it, just in case it goes haywire someday and you need to use your computer to fix it.

First, you need to enable Developer Options. To do this, go to Settings > About Phone, and tap Build Number 7 times.

Next, go to Settings > Developer Options, and turn it On by flicking the switch at the top. Then, look for a USB Debugging option and flick the switch there to turn USB Debugging On.

<a id="android-reboot-recovery"></a>
### Booting to Recovery or Bootloader

If you have `adb` on your computer and have [enabled USB Debugging](#android-enable-usb-debugging) on your phone, you can connect your phone to your computer and execute on cmd/terminal

`adb reboot <bootloader|recovery>`

to boot straight into bootloader/recovery without having to figure out the button-combo to boot into bootloader/recovery manually.

---

<a id="git"></a>
## Git

<a id="git-amend"></a>
### Amend

If you mess up your commit message or need to add more changes to the last commit, use `git commit --amend`.

---

<a id="security"></a>
## Security

<a id="security-losing-2fa"></a>
### Losing 2FA

If you use apps like Google Authenticator for 2FA, if you lose access to the app (lost phone, broken phone, etc.), you won't be able to install Google Authenticator onto a new phone and get immediate access to your 2FA codes. This is because 2FA isn't synced to the cloud. _Kinda defeats the purpose of 2FA if it is synced to the cloud._ ¯\\\_(ツ)_/¯

So, what you can do in this case is back up the QR codes by storing them in a safe place - a place hopefully also secured by 2FA but has backup codes which you have handy. For example, you could store all your 2FA QR Codes in Google Keep and have handy access to your Google 2FA Backup Codes. When you lose access to Authenticator, you can then log into your Google account using your 2FA Backup Codes and add the QR Codes back to Authenticator. Not optimal, but works in a worst-case scenario.

---

<a id="macos"></a>
## macOS

<a id="macos-ip"></a>
### IP Address

You can see details about your network like your machine's IP Address, the router's IP Address, security protocol, channel, etc. by holding down the `Option` key and clicking the Wi-Fi symbol in the menu bar.

---

<a id="vscode"></a>
## Visual Studio Code

<a id="vscode-markdown"></a>
### Markdown

VS Code gives you a live preview of Markdown. While the Markdown file is open in the editor, you can start the preview by pressing `Cmd/Ctrl + K, V` (Cmd/Ctrl + K, and then pressing V) to access the preview. Pretty neat, eh?

---

<a id="license"></a>
## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

---

<a id="contributing"></a>
## Contributing

Create a PR with your tip. Make sure you update the TOC, and the tip is actually helpful.