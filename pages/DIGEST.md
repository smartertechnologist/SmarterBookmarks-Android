# Read your Bookmark Digest

[Documentation home](../README.md) · [Guide library](../GUIDES.md)

**Bookmark Digest** gives saved links a reading view with daily selections, notes/highlights, and Android text to speech. Standard Digest uses existing bookmark fields and does not need an AI key. **Open original** takes you to the saved website when you want the full page, such as the curry's complete cooking method.

## Open a library, collection, or single-bookmark Digest

| Start from | Route and scope |
| --- | --- |
| **Bookmarks** | Toolbar → **More options → Digest** for the daily library selection. A Dashboard Digest widget or launcher Digest shortcut opens the same daily flow. |
| A saved bookmark | Its menu → **More Actions → View Digest** initially opens that bookmark in **Explore**. |
| A collection | Collection menu → **More Actions → View Digest**, or its details action, builds a selection from that collection's regular members or Smart Collection matches. |

For the saved recipe example, use **Tomato and chickpea curry → More Actions → View Digest** to begin with that one item. To browse a wider recipe set, use an eligible recipe collection's Digest. **Settings → Collections → Include sub-collections** determines whether the regular collection scope includes descendants. Smart Collections retain their own feature access requirements.

You cannot open a collection Digest for a hidden, archived, or locked collection, or one inside a locked or archived parent. Hidden bookmarks and locked collection trees are excluded from selection. Hiding a collection alone may not prevent its bookmarks from appearing in every Digest, especially when a bookmark also belongs to a visible collection. Review bookmark and collection visibility before using Digest where others can see it.

If there is no content, use the displayed empty state and check that the scope has eligible saved bookmarks. Normal daily selection starts with bookmarks at least 24 hours old and has a fallback when every lane is empty; a newly saved item need not appear immediately in a daily lane. Single-item View Digest gives a direct entry to an accessible bookmark.

## Choose a lane and move between items

Digest automatically chooses a limited selection of bookmarks. There is no search or filter picker on this screen; open the library Digest or a collection Digest to choose the reading set.

| Lane | How its candidates are chosen |
| --- | --- |
| **Catch Up** | Unopened items first, then less recently opened items; newer saves break ties. |
| **Rediscover** | Lower opened counts, older last-opened times, and older saves, after Catch Up selection. |
| **Explore** | A shuffled sample of eligible items remaining after the other selections. |

An empty lane is disabled, so all three need not be available. Tap a lane name or swipe horizontally to move among available lanes. Each lane keeps its own position.

Use **Previous** and **Next** at the bottom to change the item. You can also swipe up at the end of content for the next item, or down at the top for the previous item; ordinary scrolling still moves within long content. Long-press Previous/Next and confirm **Go to first / Go to last digest** to jump to an edge of the lane.

## Resume, shuffle, and understand completion

Reopening a daily library or collection Digest restores its saved lane/item position for the current day's cached selection, while eligible items remain available. The counter and progress bar show where you are in that lane; the unseen cue distinguishes newly displayed items.

Displaying an item records it as **seen**. It is not a measurement of reading duration. If opening statistics are enabled, viewing can also update the item's statistics at most once that day.

**Shuffle this Digest** asks before replacing today's current-lane selection with alternative candidates. Already seen items remain seen; shuffle does not clear seen history or restart a streak. After opening View Digest for one bookmark, Shuffle may include other bookmarks from your library.

In daily library Digest, viewing every item in one lane earns that day's **Reading Streak**. Tap the streak badge to see consecutive-day guidance. The badge is hidden for collection and single-bookmark Digest. Dashboard can show **Today's Digest complete**, and a new day prepares a new daily selection.

The reading screen has no separate completion sheet, Restart action, or reset-streak control. When you reach the end of a lane, continue with another available lane, reopen the original page, or close the screen.

## Read content and use the bookmark menu

Standard Digest shows an existing AI summary if available, otherwise the description, then a saved-link fallback. Title, saved comment, supplementary description, source, and available image/video are separate parts of the reading view. Existing summary text can be displayed without making a new AI request.

Use each available **More / Less** text toggle to expand or collapse a long title, comment, or description. **Open original** follows the bookmark's normal opening route and stops listening before leaving. Available image/video metadata can appear in the header; supported embedded video has its own fullscreen controls. Network/media support determines playback and imagery.

The header's **More** control opens the current bookmark's normal menu. Use its applicable opening, organization, notes, reminder, or other actions as in the [library guides](../GUIDES.md); normal feature/permission requirements still apply here.

The bottom **Share** action stops listening and opens a share-card preview using the current Digest title/text and bookmark. Review it, then **Share** through Android or **Close**. See [Share cards](SHARING.md#share-a-bookmark-as-a-card).

**Settings → Bookmarks → Show digest labels** and **Show Digest source labels** control the associated list labels. **Add Digest to home screen** creates its launcher entry when supported.

## Use the status strip

Only states applicable to the current bookmark appear. Some indicators show information; others open a detail/action view.

| Indicator | What you can do |
| --- | --- |
| Favorite, pinned, archived, hidden, opened count | Read the current state/count. These are not all edit buttons; use More for the applicable changes. |
| Reminder | Tap for the reminder details and **Delete** action. [Reminders](REMINDERS.md) explains creating/editing one. |
| Expiry | Tap for expiry details and **Remove**. |
| Broken/redirected | With Health Monitoring enabled and a recorded issue, tap to inspect the saved address or redirect target and open the page. It shows a recorded result, not a fresh reachability check. |
| Highlights | Tap the counter to review saved marked passages/annotations. |
| Notes | Tap the counter to open attached bookmark notes. |
| Relationships | Tap to review the bookmark's linked relationships. |

Actions keep their normal requirements. A recorded health issue depends on the health feature and prior results; a counter requires existing associated content.

## Highlight text or create an excerpt note

1. Hold/select text in the title, body, comment, or description and adjust its range.
2. Choose **Highlight** to retain the passage, or **Create Note** to create an attached note containing the excerpt.
3. Tap existing marked text or annotation markers for their applicable highlight/annotation actions. Use the Highlights counter for the summary sheet.

Drag selection also supports direct highlighting. A range containing an existing note annotation cannot be replaced through the overlap action. Review the existing annotation rather than selecting across it to overwrite it.

The highlight menu provides annotation, color, copy, note, and deletion operations where supported. [Reading highlights](READING.md#save-text-with-highlights-and-annotations) explains how an annotation differs from a separate note and its access limits. The available highlighting actions can differ between Digest, Browser, and Reader.

## Listen and continue through a lane

Tap **Listen to digest** to read the displayed Digest with Android text to speech and read-along highlights. Tap **Stop listening** to stop. It needs a working TTS engine and available voice, with no generative AI request. [Reader speech setup](READING.md#read-the-article-aloud) explains voice data.

While listening, choose **Auto move to next digest** to play the remaining items in the current lane. Choose **Stop after this digest** to end after the current one. Auto-listen does not cross to another lane automatically.

Keep the reading screen active while listening. Leaving or pausing it stops playback, as does opening the original, sharing, or changing AI content. Digest does not continue playing in the background or show a playback notification.

## Show or refresh AI Digest text

With **Generate AI digests** enabled, the reading controls can offer **Show AI digest / Show standard digest**. Switch to standard mode for existing bookmark fields, or AI mode for available generated digest text.

**Refresh AI digest** in AI mode requests new text for the current bookmark and displays the completed result. This requires enabled digest generation, a supported selected feature model/provider, accessible page text, connectivity, and available API allowance. It is a provider request; simply showing an already saved summary is different. See [AI summaries and Digest settings](AI.md#summaries-and-digest).
