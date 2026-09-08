# Call Recorder releases

Public release feed for Call Recorder, a menu bar app for macOS that records both
sides of a call and transcribes it. The source is private; this repository holds
the signed downloads and the Sparkle appcast the app checks for updates.

Downloads are on the [Releases](https://github.com/yoavcaspi1/callrecorder-releases/releases)
page. The app updates itself from `appcast.xml` in this repository.

## Requirements

- An Apple Silicon Mac (M1 or newer). There is no Intel build.
- macOS 14 (Sonoma) or newer.

## Install

1. Download `CallRecorder-<version>.zip` from the latest release and unzip it.
2. Drag `CallRecorder.app` into your Applications folder.
3. Open it. The icon appears in the menu bar, near the clock. There is no Dock
   icon and no window until you open one.

The app is signed with an Apple Developer ID and notarized by Apple, so it opens
normally. There is no "Open Anyway" step and no trip to Privacy and Security.
macOS may ask once whether you are sure you want to open something downloaded
from the internet: click Open.

On first run a wizard asks for Microphone (your side of the call), Screen and
System Audio Recording (the other side) and Notifications, and asks where to save
recordings. macOS has no separate "record system audio" permission, which is why
an audio-only app asks for a screen one. The app captures audio only.

Transcription defaults to Apple Speech, which runs on your Mac and needs no
account and no key. Cloud engines are optional and each needs your own API key.
Recording works with no key at all. No key is bundled with the app.

## Licence

Copyright (c) 2026 Yoav Caspi. All rights reserved.

Call Recorder is proprietary software. It is not open source and it is not free
software. Nothing in this repository grants a licence to it.

A licence to install and use the app is granted only to a person the copyright
holder has personally supplied a copy to, and to that person only, on Macs they
own or control, for their own personal, non-commercial purposes.

That permission does not include the right to copy or redistribute the app to
anyone else; to publish, sell, rent, lease or sublicense it; to use it to provide
a service to others; to use it in a business or for commercial advantage; to
modify or make derivative works of it; or to reverse engineer, decompile or
disassemble it, except to the extent that restriction cannot lawfully be excluded.

### No warranty, no liability

The app is provided "as is", without warranty of any kind, express or implied,
including any warranty of merchantability, fitness for a particular purpose, or
the completeness, accuracy or reliability of any recording or transcript.
Automatic transcription is imperfect.

To the fullest extent permitted by law the copyright holder is not liable for any
loss or damage arising out of or in connection with the app or its use, including
any lost, incomplete, corrupted or inaccurate recording or transcript, and any
indirect or consequential loss. Do not rely on it for anything where a lost or
inaccurate recording would matter, without keeping an independent record.

### Recording consent is your responsibility

The app records calls and conversations. The law on doing that varies by country
and, in some countries, by region. In many places every party to a call must be
informed and must consent before recording begins, and recording without that
consent is a criminal offence, a civil wrong, or both.

You are solely responsible for knowing the law that applies to you and to every
other party on any call you record, and for complying with it, including
obtaining any consent required and handling recordings and transcripts in line
with any applicable data protection law. The copyright holder accepts no
responsibility for any use of the app that breaks such a law.

### Your data

The app runs on your Mac. Recordings, transcripts and settings are stored on your
Mac, in the folder you choose and in `~/Library/Application Support/CallRecorder`.
There is no account and no telemetry, and nothing is sent to the copyright holder.

If you choose a cloud transcription, diarization or naming engine, your audio or
transcript is sent to that provider under your own account and their terms. No
such engine is enabled by default.

The full end user licence agreement is in the app, under Preferences, About,
Licence.
