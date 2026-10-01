# ⏱️ Tymer

<p align="center">
  <b>Track your time directly in Outlook Calendar.</b>
</p>

<p align="center">
  No timesheets. No separate app. Just your calendar.
</p>

---

## 📖 About

Tymer turns your Outlook Calendar into a time tracker.

Record what you're doing as you go, and Tymer automatically keeps your appointments aligned and gap-free.

<p align="left">
  <img height="350" alt="Adding a new appointment with Tymer" src="https://github.com/user-attachments/assets/a865cd3b-d8e1-4e19-b573-be9f9a4c6e0a" />
</p>

> **Requires Outlook (classic) for Windows.**

---

## 📦 Install

1. Close Outlook and download the latest [**Tymer.zip**](https://github.com/patryk-91/Tymer/releases/latest/download/Tymer.zip).

2. Unzip it and copy `VbaProject.OTM`.

3. Open **File Explorer** (<kbd>Windows</kbd> + <kbd>E</kbd>) and paste this path into the address bar:

   `%APPDATA%\Microsoft\Outlook`

   <img height="100" alt="Opening Outlook VBA folder" src="https://github.com/user-attachments/assets/d07f34de-7a90-46ff-a1c9-23f18be87a44" />

4. **Back up** your existing `VbaProject.OTM`, then replace it with the new one. ⚠️

5. Open **Outlook (classic)**.

6. **(Optional)** Add Tymer to the Quick Access Toolbar for easier access. See [FAQ](#%EF%B8%8F-faq).

---

## ⏱️ Using Tymer

Open Tymer from the Quick Access Toolbar or use its keyboard shortcut (e.g. <kbd>Alt</kbd> + <kbd>3</kbd>).

<p align="left">
  <img height="150" alt="Tymer window" src="https://github.com/user-attachments/assets/05289c59-94d6-4f53-b088-097391c3db84" />
</p>

Enter what you're working on and click **OK**.

Tymer adds a new appointment and automatically aligns the previous one:

<p align="left">
  <img height="200" alt="Aligned appointments in Outlook Calendar" src="https://github.com/user-attachments/assets/2030d6e2-1d10-441e-9aa9-2dc0170306d2" />
</p>

Repeat this whenever you switch activities. **Your calendar becomes your timesheet.**

---

## 🛠️ FAQ

<details>
<summary><b>Tymer doesn't work in my version of Outlook</b></summary>

<br>

Make sure you're using **Outlook (classic)** for Windows.

Tymer does not work with the new Outlook for Windows.

</details>

<details>
<summary><b>I can't find Tymer.StartTracking</b></summary>

<br>

Check that `VbaProject.OTM` was copied to:

`%APPDATA%\Microsoft\Outlook`

Then restart Outlook.

</details>

<details>
<summary><b>I already have Outlook macros</b></summary>

<br>

⚠️ Installing Tymer by replacing `VbaProject.OTM` will replace your existing Outlook VBA project.

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

<details>
<summary><b>Tymer is missing on the Quick Access Toolbar</b></summary>

<br>

1. Right-click the Outlook ribbon.
2. Select **Customize Quick Access Toolbar...**
3. Select **Macros** from the dropdown.
4. Select `Tymer.StartTracking`.
5. Click **Add**.
6. Optionally, click **Modify** to change the display name and icon.
7. Click **OK**.

You should now see the Tymer button in the Quick Access Toolbar:

<p align="left">
  <img height="60" alt="Tymer button in the Quick Access Toolbar" src="https://github.com/user-attachments/assets/eb55bb25-838e-4d23-a666-6f5b965412f2" />
</p>

Buttons in the Quick Access Toolbar automatically get a keyboard shortcut.

For example, if Tymer is the third button, press <kbd>Alt</kbd> + <kbd>3</kbd>.

</details>

<details>
<summary><b>How do I uninstall Tymer?</b></summary>

<br>

1. Close Outlook.
2. Open **File Explorer** and go to `%APPDATA%\Microsoft\Outlook`.
3. Delete the Tymer `VbaProject.OTM`.
4. Restore your original `VbaProject.OTM` from the backup.
5. Open Outlook.

If you didn't have a `VbaProject.OTM` before installing Tymer, simply delete the Tymer file.

You can also remove the Tymer button from the Quick Access Toolbar.

</details>

<details>
<summary><b>How to change Tymer's icon on Quick Access Toolbar?</b></summary>

<br>

Currently, it's a manual step:

1. Right-click QAT and click **Customize Quick Access Toolbar...**

   <img height="100" alt="image" src="https://github.com/user-attachments/assets/01166008-20db-41e5-9dd6-9659ba45d221" />
   
2. Select the macro Tymer.StartTracking and click **Modify**:
   
   <img  height="200" alt="Screenshot 2026-09-17 134113" src="https://github.com/user-attachments/assets/214f4c35-ee03-4889-9160-fca59d721ab7" />
   
3. Pick an icon and click OK
   
   <img height="200" alt="Screenshot 2026-09-17 134302" src="https://github.com/user-attachments/assets/bdbd1289-c691-4e40-95ff-3c9b2b8c9ac1" />

4. Click OK
  
</details>

<details>
<summary><b>How to keep Tymer on top?</b></summary>

<br>

Double-click the **Appointments** tab to switch to compact view and keep Tymer on top of Outlook.

<img height="200" alt="compact view docked" src="https://github.com/user-attachments/assets/5518860a-21bc-4358-8f4f-b20f0def3ed4" />

</details>

---

## 💬 Contact

Found a bug or have a suggestion?

You can report it through [GitHub Issues](https://github.com/patryk-91/Tymer/issues/new/choose) or contact me directly.

---

## ❤️ Like Tymer?

If Tymer saves you some time, consider sharing it with someone who still fills in their timesheet manually. 🙂

---

<p align="center">
  <b>⏱️ Tymer</b><br>
  <i>Your calendar is your timesheet.</i>
</p>
