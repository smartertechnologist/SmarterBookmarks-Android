# Maintain data and recover from a failed operation

[Documentation home](../README.md) · [Guide library](../GUIDES.md)

Choose the control that matches the problem before changing data. Backups, incoming sources, device sync, and website cache serve different purposes.

| What you need | Start here |
| --- | --- |
| A restorable copy before an import or corrective edit | [ZIP Complete Backup](BACKUP.md#save-a-complete-backup). Keep it in a folder you can access later. |
| Links from another app or backup file | [Import/Restore](BACKUP.md#restore-a-backup-or-import-links). Choose the matching format and duplicate options. |
| New RSS entries or Drive files | [Sources](SOURCES.md). Check the source result before Reimport data. |
| Changes missing on another Android device or Chrome | [Sync status/history](SYNC.md). Check account, network, result, and conflicts before retrying. |
| A website showing stale data or a sign-in problem | [Browser reload/cache](BROWSER.md#use-incognito-with-its-limits). Cache clearing is separate from database reset. |
| Old regular backup files | [View Backups](BACKUP.md#open-share-or-remove-saved-backup-files). Delete only the file you intend to remove. |

## Choose database memory usage

Open **Settings → Database → Import Options → Database memory usage**. The available choices are **Auto (recommended)**, **Memory saver**, **Balanced**, **Performance**, **Maximum**, and **Extreme (uses more memory)**. Keep Auto unless you have a reason to change memory allocation for large import/export work; use a lower allocation on a memory-constrained device rather than assuming the largest setting is suitable.

Changing this preference offers an app **Restart** so it can take effect. Finish current work first, then restart when ready. This setting affects database import/export performance; it does not change which file formats or records are supported.

For a large import, also check **Optimize for very large imports** and **Where to run import** in [Backup](BACKUP.md#restore-a-backup-or-import-links). A partly completed optimized import cannot be undone as one operation. Preserve a current ZIP and review the resulting records before rerunning the same file. **Skip duplicates / Replace duplicates** use the format's matching rules; similarly named collections or tags may remain separate. Check them after importing.

## Reset Database only for an intended empty library

**Settings → Database → Database Management → Reset Database** clears the local library and other information stored in its database. It affects more than one collection and is separate from clearing website cache.

1. Export a current complete ZIP and verify that you can access it before choosing a reset.
2. Tap **Reset Database**, read the first confirmation and choose **Reset** only if you intend to continue.
3. Enter the displayed confirmation code exactly, then tap **Reset** to open the final confirmation.
4. Read the final confirmation and choose **Reset** to start, or **Cancel** to leave without clearing the database.
5. Wait for the reset result and check the library. Use [Import](BACKUP.md#restore-a-backup-or-import-links) if you deliberately want to bring backup records back afterward.

Reset Database is separate from **Reset cloud storage** and **Reset Browser Sync**. Do not treat it as a full wipe of app preferences, files, or connected accounts. Before syncing the empty library with existing cloud data, check the connected account and keep a backup of the data you want to retain.
