# WellSpot 0.5.2 for Windows x64

[Download WellSpot 0.5.2 for Windows x64](https://github.com/slimane-dev/spotting_calculator/raw/refs/heads/wellspot-v0.5-download/WellSpot-0.5.2-Windows-x64.zip)

Close the previous app. Right-click the downloaded ZIP, choose **Extract All**, then double-click **WellSpot.exe** in the extracted folder. Keep its bundled files together. No separate runtime or installer is required. Existing saved jobs remain in the same local data folder.

## Read a wellbore picture

1. Select **Cement Job** or **Well Kill / Pill Spotting**.
2. For a saved file, click **Import well picture…** in **Well geometry**, above the casing table. Select PNG, JPG/JPEG, BMP or TIFF.
3. For a copied picture, copy the schematic in Excel or Paint, then click **Paste picture** beside Import. For an Excel cell range, use **Home → Copy → Copy as Picture**. The reader also accepts its Paste button and **Ctrl+V** outside text fields.
4. Review/edit the suggested values and IDs, tick the review confirmation, click **3. Apply reviewed values**, then **Save**.

Reading stays local and offline. The calculator stays usable; Cancel stops its worker and a 90-second overall deadline bounds stalled OCR. Text fields retain normal Ctrl+V.

## Changes in 0.5.2

- **Automatic editable IDs:** selecting a size/weight preset fills dimensions. Image review matches recognized size and weight against the offline database. Unclear weights receive a visibly labelled common default; unknown sizes or conflicting weights remain manually selectable. The catalogue has 257 presets. Numerical provenance and assumptions are included in `TUBULAR-ID-DATABASE.md`.
- **Default kill tubing:** a detected ESP/string reference offers 3.5-in OD / 2.992-in ID / 9.3-lb/ft tubing to that depth. The option is visible and can be disabled to keep your current string. All imported dimensions/depths remain editable. Cement review keeps its cementing string independent of ESP equipment.
- **Clear outputs:** green result headings and a fixed **Live results** heading identify the right output column. Scroll that column below Pump output. Results appear independently as their required inputs become valid; no Calculate button is needed.
- **Focus restoration:** explicit Apply/Close returns to the calculator and Apply selects the matching operation tab. The owned reader shares the app's taskbar entry. Background reading does not activate the calculator.
- The original cement/kill/pill workflows, pump strokes, named jobs, file import, offline OCR and single small **Created by Slimane Hadj** footer remain.

## Validation

397 application checks and 12 isolated-worker checks passed on Linux, normally and with internet sockets denied. **65 Windows desktop/reader checks passed** on Windows Server 2025 (NT 10.0.26100, x64), with outbound traffic blocked for the app and harness. These cover clipboard bitmap/PNG/Excel-format enhanced metafile, text paste, automatic IDs, default tubing, green headings, focus, saving and cancellation. The actual portable worker recognized the fixture with bundled Tesseract 5.0.0. [Successful Windows run](https://github.com/slimane-dev/spotting_calculator/actions/runs/37603895579). The package contains logs, a sample schematic and the target-PC manual checklist.

The automated fixture is synthetic; review results for unclear field images. The supplied reference verifies the new casing/tubing numeric dimensions, while existing drill-pipe dimensions are retained from the previous catalogue.

The executable is unsigned. Product/company metadata does not establish a trusted publisher signature.

Earlier 0.5 and 0.5.1 ZIPs remain for reference; use **0.5.2** for these changes.

ZIP SHA-256:

```
51b05b90a2676d4fbdcd8667f7e9b7b502a74e15e852ded0ca2db539dc9ca873
```
