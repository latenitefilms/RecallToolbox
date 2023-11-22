# Frequently Asked Questions

### When I double click an Item, nothing happens?

When you double click on a **Item**, the Recall Toolbox menubar tool triggers **COMMAND + V** in Final Cut Pro.

If you're accessing Recall Toolbox from the Final Cut Pro Workflow Extension, it will automatically launch the Recall Toolbox menubar application to trigger the paste.

The first time you do this, you should be presented with an alert requesting Accessibility Permissions:

![](/static/accessibility-permission.png)

You should click **Open System Settings**.

You'll then be presented with:

![](/static/accessibility-system-prefs.png)

You should click the grey toggle next to Recall Toolbox to enable Accessibility Permissions.

Once enabled, Recall Toolbox will be able to trigger the Paste shortcut key in Final Cut Pro.

However, if you were previously using a TestFlight version of Recall Toolbox, it's possible that you granted the TestFlight version permission, but not the App Store version and macOS is silently preventing Recall Toolbox from triggering the virtual shortcut key.

In this case, you should try manually removing Recall Toolbox from the Accessibility Permission list, and then manually adding it back in.

---

### When I drag a clip it drags a `__timelineContainerClip`?

Let's imagine you've copied this single Multicam clip on your Final Cut Pro timeline:

![](/static/regular-multicam-clip.png)

With a **Folder** selected in Recall Toolbox, you've then clicked **New Item** to save this Multicam Clip into Recall Toolbox.

If you double click this newly created item, it will paste it within Final Cut Pro as you'd expect:

![](/static/regular-multicam-clip-2.png)

However, if you instead **drag** the clip from Recall Toolbox to Final Cut Pro, you'll get this `__timelineContainerClip` instead:

![](/static/timeline-container-clip.png)

This is a limitation/quirk of Final Cut Pro and the way it handles Pasteboard items when dragging in from another application.

You can think of this `__timelineContainerClip` as a **Compound Clip**, and you can use the **Clip > Break Apart Items**, to restore it back to it's original form.

---

### Can I access my data on iCloud Drive?

No, Recall Toolbox uses Apple's [CloudKit](https://developer.apple.com/icloud/cloudkit/), as opposed to more user-facing services such as iCloud Drive or iCloud Documents.

All of your Folders & Items are stored on Apple's iCloud Servers.

Recall Toolbox uses CloudKit to talk to Apple's servers to keep the local copy of Recall Toolbox's database synchronised with the iCloud copy.

There's no other interface to access your Recall Toolbox data, apart from using the Recall Toolbox application.