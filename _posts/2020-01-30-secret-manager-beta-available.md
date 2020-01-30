---
layout: post
title: "Secret Manager Beta on Google Play"
date: 2020-01-30 12:40
permalink: /posts/secret-manager-beta-available
tags: [miguel, romeral, release, available, secret, manager]
---

## Secret Manager App now available on Google Play

The last project is released since today! Secret Manager has appeared on [Google Play](https://play.google.com/store/apps/details?id=es.miguelromeral.secretmanager) in its Beta channel and you can download it for free.

This app is very similar to [mrCiphER=](https://play.google.com/store/apps/details?id=es.uah.edu.miguelangelgarciar.mraes), which it was released on 2017, but with some new features, expleaned below:

First of all, the language used is Kotlin, [the main language for Android applications since in 2017 was announced in Google I/O](https://techcrunch.com/2019/05/07/kotlin-is-now-googles-preferred-language-for-android-app-development/?guccounter=1&guce_referrer=aHR0cHM6Ly93d3cuZ29vZ2xlLmNvbS8&guce_referrer_sig=AQAAAHuUxPjgx4fFh4BeLPLzeudv3JOw9Rvf0JAnw8vlAnluM5dgWOoElPAIQpFlRbYQkmq4XpgHtVFDeeaElXfKuYiLbhXlnk7c7dG0yJoqxmupbBS7mGt3sGjPKlmxanq3rw73-kYwT_BP9b5R7IfNYr9lCbEabQvq4o05KECKMoCd). Also, the app counts with most common Android development pattern MVVM, using such tools like ViewModels or jobs and couroutines for background operations.

Another significative difference is there's no longer possible to decide what algorithm to use, so in mrCiphER= you can choose between AES, RSA and even 3DES among others, but in Secret Manager there's only AES and it's transparent for the user to know that, because the user should be only concerned about using the same password for encrypt some text and in other moment to decrypt it.

<div style="text-align: center;">
<img src="https://raw.githubusercontent.com/miguelromeral/SecretManager/master/screenshots/Screenshot_1580320480.png" height="300" width="auto">
</div>

The app also allows the user to store the secret stored just on the own app, with a Room database that stores the content of secret encrypted and an alias to be able to identify it, so the user can open it in any moment. Another feature included makes easier to export the data from one device and then import it to another android smartphone. The app will need storage permission from the user to generate a CSV file (readable by Microsoft Excel, Libre Office or any text editor).

<div style="text-align: center;">
<img src="https://raw.githubusercontent.com/miguelromeral/SecretManager/master/screenshots/Screenshot_1580320842.png" height="300" width="auto">
</div>

The other main update from its predecessor its the ability of process files no larger than 50 MB, so the file encrypted can be shown by the Android Device (download_encrypted.png in picture below) but not opened because its content is encrypted and for the device it hasn't sense at all. But when you open it from the app and decrypt it with the right password, then another file is created and it's exactly the same as first file used (download_restored.png in picture below).

<div style="text-align: center;">
<img src="https://raw.githubusercontent.com/miguelromeral/SecretManager/master/screenshots/Screenshot_1580320662.png" height="300" width="auto">
<img src="https://raw.githubusercontent.com/miguelromeral/SecretManager/master/screenshots/Screenshot_1580322527.png" height="300" width="auto">
</div>

Secret Managar has some other functionalities like Dark Theme, QR images for text processed, encrypt text from other apps using intent-filters, open any file.

You can find further information in its [GitHub repository page](https://github.com/miguelromeral/SecretManager) and also you can take a look to the open source code.