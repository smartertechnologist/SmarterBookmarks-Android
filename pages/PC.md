# Connect to PC over a local network

[Documentation home](../README.md) · [Guide library](../GUIDES.md)

**Connect to PC** is a Pro feature that serves your phone's library to a computer browser over a reachable local network. It is a temporary connection to the phone, separate from [Cloud sync and Browser Sync](SYNC.md).

## How it works

1. Connect the phone and computer to the same reachable Wi-Fi, or turn on the phone's hotspot and connect the computer to it.
2. In SmarterBookmarks, open the main toolbar menu → **Connect to PC**.
3. On the phone's connection screen, find the address for the network you are using. Enter the complete displayed URL, including its port, in the computer browser.
4. On the phone, check the incoming device's connection request and choose **Accept** to permit it, or **Reject** to deny it.
5. Use the computer page to view/manage the library. For a recognizable check, find **Tomato and chickpea curry** by its saved title and open its collection. Existing library search, editing, and pagination are provided by the local web interface.
6. Return to the phone's Connect to PC screen and choose **Disconnect** when finished.

An internet connection is not required for the local library connection itself. Opening live bookmarked websites or loading online content can still need network access. Keep the phone's connection active while using the computer session, and use **Disconnect** to end it.

## Address controls and connection problems

The screen offers Wi-Fi, local hostname, and hotspot addresses when available. **Copy** puts the chosen URL on the clipboard; **Share** sends it through Android. **Refresh** recalculates the addresses and retries hostname discovery after a network change. Buttons for unavailable addresses are disabled.

If the Wi-Fi/hotspot section asks you to connect and refresh, do that before copying its URL. If the hostname address does not resolve, try the displayed numeric Wi-Fi address instead. Local hostname support depends on the network. Use the actual address shown on your phone rather than a fixed address from another person's example.

If the computer cannot reach the phone, check that both are on the intended Wi-Fi/hotspot and that the phone still shows an available address. Refresh after switching networks, reload the computer page, and check the phone for the approval request. A network that isolates clients can prevent local access even when both devices show the same Wi-Fi name.

The app may request notification access for the connection service. Its permission message opens Android app settings when access is missing. Grant the requested access if you want its service notification; device settings vary.

**Disconnect** closes the approved connection and returns the phone to its address/connection view. It does not delete bookmarks or reset either cloud-sync feature. Use it explicitly at the end of the session.

**Related:** [Backup before substantial edits](BACKUP.md) · [Data maintenance](DATA.md) · [Sharing and home-screen entries](SHARING.md).
