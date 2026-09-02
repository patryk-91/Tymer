# ⏱️ Tymer

<p align="center">
  <b>Track your time directly in Outlook Calendar.</b>
</p>

<p align="center">
  No timesheets. No separate app. Just your calendar.
</p>

---

## 📖 About

**Tymer** is a simple Outlook add-in for tracking your time directly in your calendar.

It creates consecutive calendar appointments, automatically aligning each new appointment with the previous one.

<p align="left">
  <img height="350" alt="Adding a new appointment with Tymer" src="https://github.com/user-attachments/assets/a865cd3b-d8e1-4e19-b573-be9f9a4c6e0a" />
</p>

> [!TIP]
> Your Outlook Calendar becomes a visual history of what you worked on and how much time you spent on it.

---

## 💻 Requirements

| Requirement                | Supported |
| -------------------------- | :-------: |
| 🪟 Windows                 |     ✅     |
| 📅 Outlook (classic)       |     ✅     |
| 🆕 New Outlook for Windows |     ❌     |
| 🌐 Outlook on the web      |     ❌     |
| 📱 Outlook Mobile          |     ❌     |

> [!IMPORTANT]
> Tymer requires **Outlook (classic)** for Windows because it runs as an Outlook VBA project.

---

## 📦 Install

> [!WARNING]
> `VbaProject.OTM` contains your Outlook VBA project. Replacing it will overwrite any Outlook VBA macros you already have.
>
> **Make sure to create a backup first.**

### 1️⃣ Install Tymer

1. Close Outlook.

2. Download `Tymer.zip`.

3. Unzip the file.

4. Copy `VbaProject.OTM`.

5. Go to:

   ```text
   %APPDATA%\Microsoft\Outlook
   ```

6. Make a backup of your existing `VbaProject.OTM`.

7. Paste the new `VbaProject.OTM` into the folder.

8. Open **Outlook (classic)**.

> [!NOTE]
> When Outlook starts, Tymer will ask whether you want to start tracking immediately.

### 2️⃣ Add Tymer to the Quick Access Toolbar

1. Right-click the Outlook ribbon.
2. Select **Customize Quick Access Toolbar...**
3. Select **Macros** from the dropdown.
4. Select:

   ```text
   Tymer.StartTracking
   ```

5. Click **Add**.
6. Optionally, click **Modify** to change the display name and icon.
7. Click **OK**.

You should now see the Tymer button in the Quick Access Toolbar:

<p align="left">
  <img height="200" alt="Tymer button in the Quick Access Toolbar" src="https://github.com/user-attachments/assets/eb55bb25-838e-4d23-a666-6f5b965412f2" />
</p>

> [!TIP]
> Buttons in the Quick Access Toolbar automatically get a keyboard shortcut.
>
> For example, if Tymer is the third button, press <kbd>Alt</kbd> + <kbd>3</kbd>.

### ✅ Installation checklist

* [ ] `VbaProject.OTM` backed up
* [ ] Tymer installed
* [ ] Outlook (classic) opened successfully
* [ ] Tymer added to the Quick Access Toolbar
* [ ] Tymer window opens

---

## 🚀 Quick Guide

### 1. Start tracking

Click the **Tymer** button in the Quick Access Toolbar.

Or use its keyboard shortcut, for example:

<kbd>Alt</kbd> + <kbd>3</kbd>

The Tymer window will open:

<p align="left">
  <img height="200" alt="Tymer window" src="https://github.com/user-attachments/assets/05289c59-94d6-4f53-b088-097391c3db84" />
</p>

> [!NOTE]
> Tymer automatically shows the previous appointment from your calendar.

### 2. Enter what you're working on

Update the topic and click **OK**:

<p align="left">
  <img height="200" alt="Adding a new appointment" src="https://github.com/user-attachments/assets/ed0c0355-bdb4-472d-af1c-dd829b9f8766" />
</p>

### 3. That's it 🎉

Tymer:

* adds a new appointment,
* aligns the previous appointment with it,
* keeps your calendar timeline continuous.

<p align="left">
  <img height="200" alt="Aligned appointments in Outlook Calendar" src="https://github.com/user-attachments/assets/2030d6e2-1d10-441e-9aa9-2dc0170306d2" />
</p>

> [!TIP]
> Repeat this whenever you switch activities and your calendar gradually becomes your timesheet.

---

## ⌨️ Quick Workflow

Once everything is configured, tracking can be as simple as:

```text
Alt + [number]  →  Enter topic  →  OK
```

For example:

```text
Alt + 3  →  Project XYZ  →  OK
```

---

## 🗑️ Uninstall

1. Close Outlook.

2. Go to:

   ```text
   %APPDATA%\Microsoft\Outlook
   ```

3. Delete the Tymer `VbaProject.OTM`.

4. Restore your original `VbaProject.OTM` from the backup.

5. Open Outlook.

You can also remove the Tymer button from the Quick Access Toolbar.

<details>
<summary><b>What if I didn't have a VbaProject.OTM before installing Tymer?</b></summary>

<br>

Simply remove the Tymer `VbaProject.OTM` file.

</details>

---

## 🛠️ Troubleshooting

<details>
<summary><b>Tymer doesn't appear in Outlook</b></summary>

<br>

Make sure you're using **Outlook (classic)** for Windows.

Tymer does not work with the new Outlook for Windows.

</details>

<details>
<summary><b>I can't find Tymer.StartTracking</b></summary>

<br>

Check that `VbaProject.OTM` was copied to:

```text
%APPDATA%\Microsoft\Outlook
```

Then restart Outlook.

</details>

<details>
<summary><b>I already have Outlook macros</b></summary>

<br>

**⚠️ Caution:** Installing Tymer by replacing `VbaProject.OTM` will replace your existing Outlook VBA project.

Do **not** overwrite your existing file unless you have created a backup.

</details>

<details>
<summary><b>Tymer doesn't ask me to start tracking when Outlook opens</b></summary>

<br>

If Tymer works when started manually, but doesn't show the **"Do you want to start tracking?"** message when Outlook opens:

1. Press <kbd>Alt</kbd> + <kbd>F11</kbd> to open the Visual Basic Editor.
2. Close the Visual Basic Editor.
3. Close Outlook.
4. Open Outlook again.

This can happen when Outlook doesn't detect VBA code after `VbaProject.OTM` has been copied to a computer that didn't previously use Outlook macros.

**Note:** Simply opening the Visual Basic Editor once should make Outlook detect the VBA project on subsequent startups.

</details>

---

## 💬 Contact

Found a bug or have a suggestion?

You can report it through GitHub Issues or contact me directly.

---

## ❤️ Like Tymer?

If Tymer saves you some time, consider sharing it with someone who still fills in their timesheet manually. 🙂

---

<p align="center">
  <b>⏱️ Tymer</b><br>
  <i>Your calendar is your timesheet.</i>
</p>
