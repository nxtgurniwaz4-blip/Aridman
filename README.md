# Aridman’s Happy Place — Codemagic-ready iOS project

Bundle ID: `com.aridman.happyplace`
Display name: `Aridman’s Happy Place`
Target: iPhone + iPad
Minimum iOS: 17.0

## Codemagic
The repository contains `codemagic.yaml` at its root. The workflow:
1. Installs XcodeGen.
2. Generates `AridmansHappyPlace.xcodeproj` from `project.yml`.
3. Applies Codemagic iOS signing profiles.
4. Builds a distribution IPA.
5. Exposes the IPA as a Codemagic artifact.

For signing, configure the appropriate Apple signing credentials in Codemagic. Do not put private `.p12` passwords or certificates in the repository.

## Local Xcode
On a Mac with Xcode and XcodeGen:
`xcodegen generate --spec project.yml`
Then open `AridmansHappyPlace.xcodeproj`.

## Current v0.1
- Tractor, bus, farm, truck, animal and matching activities
- Large touch targets and simple animations
- iPhone/iPad adaptive grid
- Original app icon asset set
- No external dependencies
- No network/video dependency

## Pramod’s Life Videos
The Videos tile now opens a dedicated Pramod’s Life section with category filters for All, Tractors, Buses, Farming, JCB & Machines, and Trucks & Vehicles. Curated YouTube videos are streamed using YouTube's embedded player; the app does not download or redistribute the source videos.

The Buses filter includes a YouTube search fallback when no curated bus videos are available. The channel link opens Pramod’s Life directly on YouTube.
