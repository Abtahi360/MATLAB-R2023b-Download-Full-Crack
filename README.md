## 🛠️ Installation Process (MATLAB R2023b)

> ⚠️ This is for educational purposes only. Please ensure you have the proper license or rights to use MATLAB.

### 📦 Requirements

* **MATLAB R2023b Windows ISO** file (`R2023b_Windows.iso`)
* Optional: **MATLAB R2022b ISO** for `license.lic` file
* Mounting tool (e.g., *Daemon Tools Lite* if you're on Windows 8 or older)

---

### 🔧 Steps

1. **Mount the ISO file**
   Mount `R2023b_Windows.iso` to a virtual drive.

   * On **Windows 10+**: Right-click → *Mount*
   * On **Windows 8 or below**: Use *Daemon Tools Lite*

2. **Run `setup.exe`**

   * If prompted with a login screen, click **Advanced Options** → select **“I have a File Installation Key”**
   * If no internet: this mode will auto-select.

3. **Enter the Installation Key**

   ```
   19888-45209-61323-29230-25497-43412-35108-15123-25580-54377-05875-31006-25681-45018-46907-09460-23253-25339-58435-17194-52867-38929-08174-61608-35890-10321
   ```

   Parallel Server Key (if needed):

   ```
   11317-39170-30581-06794-33638-30864-39215-17095-10747-02684-27090-22009-16584-56488-15039-17855-31650-45204-02949-59443-61430-56121-38824-55110-16755
   ```

4. **Select License File**
   Choose `license.lic` from the folder containing `Matlab913_R2022b_Win64.iso`.

5. **Choose Installation Path**
   Example: `C:\Program Files\MATLAB\R2023b`

6. **Choose Products to Install**

   * Full install ≈ 30 GB
   * MATLAB only ≈ 3 GB

   > 💡 SSD recommended for faster startup.

7. **Add Shortcut**
   Select the option **"Add shortcut to desktop"**.

8. **Wait for Installation**

   * Progress may appear stuck (e.g., always 0%).
   * Check `<matlabfolder>` size manually if unsure.
   * If size stalls, close and restart from Step 1.

9. **Patch File Replacement**

   * Copy `libmwlmgrimpl.dll` from ISO folder to:

     ```
     <matlabfolder>\bin\win64\matlab_startup_plugins\lmgrimpl
     ```

   * Confirm **overwrite** prompt. No overwrite = issue!

   > 🔁 For Polyspace:
   > `C:\Program Files\Polyspace\R2023a\bin\win64\matlab_startup_plugins\lmgrimpl`

10. **Fix Desktop Shortcut (if needed)**
    If not created or broken, manually point it to:

```
<matlabfolder>\bin\win64\MATLAB.exe
```

11. ✅ **Launch MATLAB and enjoy!**

---

### 📺 Demo Video

[🔗 Watch Installation Demo](#): 

---

### ⬇️ Download

📥 Download R2023b ISO: https://www.terabox.app/sharing/link?surl=crEZakKX6spFGPQgxGRT9w

---

### ⚠️ Notes

* Some add-ons or products may not be available.
* If setup freezes during steps 1–7, restart setup.
* For updates/changes, repeat Step 8 (replacing `libmwlmgrimpl.dll`) but skip Step 3.
