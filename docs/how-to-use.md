# How To Use

### Installation

You can download Recall Toolbox from the Mac App Store [here](https://apps.apple.com/us/app/recall-toolbox/id6448816971).

When you run Recall Toolbox for the first time, it will load the Menu Bar icon:

![](/static/menubar.png)

You can easily access Recall Toolbox from the Menu Bar icon at any time:

![](/static/menubar-fresh-install.png)

You can also access Recall Toolbox directly in Final Cut Pro as a Workflow Extension.

You can find it in the Workflow Extension button:

![](/static/workflow-extension-button.png)

You can also find it in the Workflow Extension menu:

![](/static/workflow-extension-menu.png)

The Menu Bar version of the application and the Workflow Extension version are independent, sandboxed versions of the same application, and also use iCloud to share information between each other.

---

### Accessibility Permission

Recall Toolbox requires Accessibility Permission to trigger the Paste command in Final Cut Pro.

The first time you double click a saved Item in Recall Toolbox you'll be presented with this macOS alert:

![](/static/accessibility-permission.png)

You should click **Open System Settings**.

You'll then be presented with:

![](/static/accessibility-system-prefs.png)

You should click the grey toggle next to Recall Toolbox to enable Accessibility Permissions.

Once enabled, Recall Toolbox will be able to trigger the Paste shortcut key in Final Cut Pro.

---

### Folders

Recall Toolbox is very simple - on the left sidebar you have a list of **Folders**, and within each Folder you have a list of **Items**.

You can click the **New Folder** Item in the bottom left corner to create a new folder:

![](/static/new-folder.png)

Once a Folder is created, you can right-click on it to **Rename** it.

![](/static/rename-folder.png)

You can delete Folders by clicking the **Remove Folder** button in the bottom left:

![](/static/remove-folder.png)

You can rename Folders by right-clicking on the Folder and selecting **Rename**.

---

### Items

Once you have created a **Folder**, you can now populate it with **Items**.

The easiest way to create an item is to copy something in Final Cut Pro (for example, a Title in your project/timeline), then with a Folder selected, press the **New Item** button:

![](/static/new-item.png)

If you have nothing in the Final Cut Pro Pasteboard, you'll be presented with this alert:

![](/static/empty-pasteboard.png)

Once you create a New Item:

![](/static/create-new-item.png)

You'll be presented with a confirmation alert:

![](/static/new-item-created.png)

Anything that can be copied in Final Cut Pro, can be saved in Recall Toolbox.

You can also drag-and-drop items from the Final Cut Pro Browser to Recall Toolbox, and it will save those items as FCPXML data.

You can also drag-and-drop files from Finder (or other applications) to Recall Toolbox, and it will save **links** to those files - meaning it just saves the file path, not the actual file data. This can be useful if you have Shared Storage, and you want to save common assets in Recall Toolbox to be shared between multiple machines.

Every item can also have it's own thumbnail. Simply drag an image from Finder (or other applications) into an Item to update the thumbnail.

You can also right-click on an Item to access the contextual menu:

![](/static/item-menu.png)

**Copy Item to Pasteboard** allows you to copy an Item to the Pasteboard without triggering a Paste in Final Cut Pro.

**Rename Label** allows you to rename the Item.

**Browse Thumbnail** allows you to select a new Thumbnail.

**Replace Item with Pasteboard Contents** allows you to replace the Item's contents with whatever is on the Final Cut Pro Pasteboard.

---

### Sharing Folders

If you want to share a Folder with other iCloud users, simply select the Folder you want to share, and press the **Share** button.

You'll be presented with this, whist the initial sharing takes place:

![](/static/sharing-in-progress.png)

Once the Folder has been shared, you can press the **Share** button again to add the email addresses of other iCloud users you want to share the folder with:

![](/static/share-options.png)

---

### Sandboxing

The Menu Bar version of the application and the Workflow Extension version are independent, sandboxed versions of the same application, and also use iCloud to share information between each other.

This means that if you drag a file from Finder to the Menu Bar version of Recall Toolbox, only the Menu Bar version has access to that file - the Workflow Extension does not.

This is the same for if you're sharing a File between multiple machines - due to macOS sandboxing, you need to give Recall Toolbox explicit permission to access those files on each machine.

When a file can't be accessed, the File tag background will be red:

![](/static/file-offline.png)

However, to solve this, in the Workflow Extension, you can use press the **Settings** icon and then **Grant Sandbox Access** to the folder or drive which contains the folder.

![](/static/sandbox-access.png)

There's also the option to **Reset Sandbox Access** to revoke permission to any locations you've previously granted it permission too.