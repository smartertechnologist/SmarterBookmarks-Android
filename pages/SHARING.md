# Save from Android, share cards, and add home-screen entries

[Documentation home](../README.md) · [Guide library](../GUIDES.md)

Use Android's Share action to save a link you found in another app. A home-screen shortcut opens one page or app area; the **Collection List** widget lets you browse a collection without opening the main list.

## Choose an Android save target

In **Settings → Behavior → Share intent options**, enable the targets you want Android to offer. There are three save behaviors; direct saving has a plural label when the sending app shares multiple items.

| Android target | What happens |
| --- | --- |
| **Save bookmark…** | Opens **New bookmark** so you can review the address, inferred title, imagery, and destination before Create. Accepts single or multiple text/image shares containing usable URLs. |
| **Save bookmark / Save bookmarks** | Extracts valid links and saves directly without the editor. Accepts single or multiple shares. |
| **Save and open bookmark** | Saves and opens one resulting bookmark in the app browser. Accepts one shared item; use the review target for several resulting links. |

To review the recipe before saving:

1. In the app/browser displaying the recipe, choose its **Share** action.
2. In Android's chooser, choose **Save bookmark…**.
3. Check **Url** and **Title** in **New bookmark**. Choose a collection if desired, then tap **Create**, as in [Save your first bookmark](SAVE.md).
4. Open **Bookmarks** and check the saved title/address. If there is no valid address, correct it in the draft rather than saving the surrounding message as a link.

Direct saving uses the automatic default collection and URL-cleanup/dynamic-match preferences. For one URL, it can update an existing matching bookmark; it is not always a new record. After a direct save, check Bookmarks or the configured collection. The configured rules run for newly created items, and enabled metadata fetching/classification can continue afterward. AI classification needs its own [AI setup](AI.md); sharing a link does not itself require an AI key.

If a target is absent, check **Share intent options** and that the sending app shares compatible text/image content. Android and the sender determine which chooser entries appear. **Nothing to save** means no usable URL was parsed; paste the address manually using [Save](SAVE.md).

## Review several links and accompanying images

Shared text can contain several addresses. For exactly one URL, a shared title/subject or surrounding text can supply its draft title. Review it: a sender's caption may not be the page's title.

With **Save bookmark…**, extracted URLs are combined in the Url field. Multiple valid URLs enable **Batch mode** and are validated as a group. Review the URL chips, remove unwanted/invalid entries, and choose the intended common options before Create. The current draft limit is 100 URLs; split a larger set into smaller batches. A single title/image is not applied as though every page were the same bookmark. The [bookmark guide](SAVE.md) explains the manual creation fields.

An image share must also contain a valid page URL to become a bookmark. If the shared content contains exactly one valid URL, it can use the first supported accompanying image. Sharing only an image does not create a bookmark, and multiple URLs do not each receive that one image.

Direct saves copy the accompanying image into app storage when possible. With **Save bookmark…**, an image can appear in the draft yet be missing after saving, especially when the sending app grants only temporary access to it. Check the saved bookmark's image. If it is missing, choose one through the bookmark's editing controls.

## Scan a QR or Aztec code

1. Open **New bookmark** using Bookmarks **+** or the launcher **Add bookmark** entry.
2. If the scanner control is present, tap it and point the camera at a QR or Aztec code.
3. Review the value in **Url**. It replaces an empty field or appends a new line to existing content.
4. Correct/remove non-URL text if needed, then finish the normal validated save flow.

The scanner requires a camera, portrait support, and the Google scanner module. The app checks/downloads that optional module before showing the control; readiness can take time. If it is absent, reopen the form after module setup or paste the URL manually. Canceling the scan does not save a bookmark. A scanned value still has to pass normal URL validation; scanning a code is not proof that its destination is suitable.

## Use the app-icon shortcuts

On a supporting launcher, long-press the SmarterBookmarks icon. Shortcuts include **Add bookmark**, **Bookmarks**, **Collections**, **Notes**, and **Bookmark Digest**. Your launcher may show fewer entries.

**Add bookmark** opens an empty draft. Keep **Save bookmark…** enabled in **Settings → Behavior → Share intent options** to use this shortcut. The other entries open their app area; a hidden navigation tab can route to an enabled area instead. **Bookmark Digest** opens the daily [Digest](DIGEST.md). Browser is a separately pinned shortcut, described below.

## Pin a bookmark or collection shortcut

For the recipe, open its menu → **More Actions → Add to home screen**. Check the editable title and icon, enter a nonempty label, confirm, then accept/place the shortcut in your launcher's pin prompt. The icon can use bookmark imagery/favicon or the app icon according to the applicable preferences and available image.

For **Recipes to try**, open the collection menu → **Add to home screen… → Shortcut**, check its name/icon/color, and confirm the launcher's pin request. Opening the shortcut returns to that collection, subject to the normal visibility/lock rules. Collection settings can allow duplicate shortcuts for the same collection.

**Settings → Bookmarks** controls whether bookmark shortcuts use the app's opening rules or hand the URL directly to Android. See [opening preferences](SETTINGS.md#choose-how-bookmarks-open). A shortcut does not copy the full bookmark to the launcher. If the launcher reports pinning unsupported, use the app list instead.

## Pin a Browser shortcut

Open **Settings → Behavior → Add Browser to home screen**, then accept the launcher's pin request. It opens Browser home with the configured tabbed-browser setting. A supporting launcher is required. This entry is separate from the five app-icon shortcuts.

## Add and browse the Collection List widget

1. Open your launcher's widget picker and select SmarterBookmarks **Collection List**, or use a collection's **Add to home screen… → Widget** route where available.
2. In the widget configuration, select **Recipes to try** or the root library, then **Save**.
3. Place and resize the widget using the launcher's controls.
4. Tap a collection to see its children, or tap a bookmark to open it. Use the widget's Back/up control to return toward the root and **Refresh** to reload its list.

This is an Android home-screen widget, separate from the app's [Dashboard widgets](DASHBOARD.md). The app's direct pin request requires Android newer than 8.0 and launcher support. If automatic placement does not appear, use the launcher's widget picker.

The widget uses collection/bookmark display preferences. Hidden-item inclusion follows collection-list preferences, and you cannot browse into locked collections from the widget. Check those preferences before placing a library widget where others can see it. Do not assume that a widget or shortcut hides everything excluded from your current app list.

## Share a bookmark as a card

1. Open the recipe's menu and choose **Share & Copy → Share as card**.
2. Review the preview's title, description, source, and available image/read time.
3. Tap **Share** and choose an Android receiving app, or **Close** to dismiss it.

The app sends a PNG plus a title/link caption. The receiving app decides how to show them. The preview has Share and Close; it does not provide a card editor, theme picker, or template selector. Image fetching may need network access; an unavailable image can produce a card without it.

Digest's Share control makes a card from the text currently displayed in [Digest](DIGEST.md#read-content-and-use-the-bookmark-menu). Card sharing is different from [sharing a URL](BROWSER.md#save-share-or-copy-the-current-page) or [exporting library data](BACKUP.md).
