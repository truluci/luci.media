# Media Omarchy Plugin

This is an Omarchy plugin that provides an MPRIS media control service and an interactive bar widget to control your currently playing media. It integrates with MPRIS and Pipewire to smoothly track active media players and audio streams.

<img width="482" height="287" alt="image" src="https://github.com/user-attachments/assets/f042f7b8-2e4b-4d7c-b605-e966ef40c661" />


## Features

- **Media Control Service:** Tracks running MPRIS players, proxies, and audio streams, correctly selecting the active player based on playing state and history.
- **Bar Widget:** Displays a clean indicator on your bar showing the playback state, track title, and artist. It features scrolling text for long titles.
- **Interactive Popup:** A detailed popup card featuring:
  - Album art, track title, artist, and album.
  - Interactive media progress bar (seek control).
  - Play, Pause, Next, and Previous controls.
  - A selectable list of all available media sources to easily switch active players.
- **OSD Integration:** Works with Omarchy OSD to show feedback when switching tracks or sources.

## Usage

You can interact with the widget on your bar using the following mouse actions:

- **Left Click**: Play / Pause
- **Right Click**: Open the detailed popup card
- **Middle Click**: Next track
- **Scroll Wheel**: Next / Previous track

## Technical Details

- **Entry Points:** 
  - `Service.qml` (handles the backend logic, MPRIS bindings, Pipewire node tracking, and playing queue)
  - `BarWidget.qml` (the frontend UI widget for the bar)
- **Requirements:** Quickshell (with MPRIS and Pipewire services enabled)
