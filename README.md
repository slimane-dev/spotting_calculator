# WellSpot 0.5.1 for Windows x64

[Download WellSpot 0.5.1 for Windows x64](https://github.com/slimane-dev/spotting_calculator/raw/refs/heads/wellspot-v0.5-download/WellSpot-0.5.1-Windows-x64.zip)

Close the previous app. Right-click the downloaded ZIP, choose **Extract All**, then double-click **WellSpot.exe** in the extracted folder. Keep its bundled files together. No separate runtime or installer is required. Existing saved jobs remain in the same local data folder.

## Read a wellbore picture

1. Select **Cement Job** or **Well Kill / Pill Spotting**.
2. In **Well geometry**, click **Import well picture…**, above the casing table.
3. Select a PNG, JPG/JPEG, BMP or TIFF from your computer. Reading starts offline. If you cancel the chooser, use **1. Choose picture…** in the reader window.
4. Review and edit the suggested values and actual pipe IDs, tick the review confirmation, then click **3. Apply reviewed values**. Click **Save** to retain the job.

The calculator stays usable during reading. **Cancel reading** stops the private OCR worker; a 90-second overall timeout bounds a stalled reading. Pictures are processed locally and remain editable.

Version 0.5.1 fixes the reader's opening error, clarifies picture selection, isolates OCR failures and preserves edits made during review. Cement-job and kill/pill calculations, editable pump output and stroke results, named jobs and the single small **Created by Slimane Hadj** footer are retained.

Validation: **320 application checks + 12 isolated-worker checks** passed on Linux, including runs with internet sockets denied. **38 Windows desktop/reader checks** passed on Windows Server 2025 (NT 10.0.26100, x64), with outbound traffic blocked for the app and harness. The actual portable executable recognized the synthetic fixture using bundled Tesseract 5.0.0. [Windows run and report](https://github.com/slimane-dev/spotting_calculator/actions/runs/37590992821).

The package includes validation logs, example picture and manual checks. Review field images carefully; automated fixture checks do not guarantee every image's reading. Target-PC display scaling, physical file-chooser interaction and other supported formats remain manual checks.

The executable is unsigned. Product/company metadata does not establish a trusted publisher signature.

The earlier 0.5 ZIP is retained for reference; use **0.5.1** for the reader fix.

ZIP SHA-256:

```
c462e8e6730f0a8c01cc7141379fedb1a7745a749978d7fcd8fdbc088e92fec7
```
