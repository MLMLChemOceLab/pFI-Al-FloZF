# FloZF Sequences for pFI-Based Determination of Dissolved Aluminium in Seawater

This repository contains FloZF method sequence files used in:

**"A matrix-independent method for direct nanomolar dissolved aluminum analysis in seawater using programmable Flow Injection (pFI)"**  
M. M. Grand and M. Hatta, 2025, submitted to *Analytical Chemistry*.

These sequences were developed for the [MiniSIA-2](https://www.globalfia.com/shop/systems?view=article&id=126:minisia-2&catid=57) platform running FloZF software. They implement a programmable Flow Injection (pFI) method for determining dissolved Al in seawater using the lumogallion fluorescence assay.

---

## 📁 Contents

- `Grand&Hatta_BrijEnhanced_FloZF_sequencefile.xml`:  
  Sequence file optimized for **open-ocean samples**, includes **Brij** to enhance fluorescence yield.

- `Grand&Hatta_NoBrij_FloZF_sequencefile.xml`:  
  Sequence file for **high-Al samples (>400 nM)**, does **not** include Brij.

- `devices.xml`:  
  Configuration file for MiniSIA-2 hardware. Required by FloZF to recognize the components used in this method (valves, pumps, etc.).

---

## 🧪 How to Use

These files are specific to the GlobalFIA MiniSIA-2 platform and FloZF software. To use:

1. Place the `devices.xml` file in your FloZF installation directory (typically `C:\Program Files\FloZF\Devices` or similar).
2. Load either sequence file in FloZF depending on sample type:
   - Use the **Brij-enhanced** sequence for low-concentration (open-ocean) samples.
   - Use the **No-Brij** version for high-Al (>400 nM) samples.
3. Refer to the manuscript for reagent composition, valve configuration, and instrument timing details.

---

## 📄 Citation

If you use or adapt these files, please cite:

> Grand, M. M., & Hatta, M. (2025). A matrix-independent method for direct nanomolar dissolved aluminum analysis in seawater using programmable Flow Injection (pFI). Submitted to *Analytical Chemistry*.

---

## 📬 Contact

Questions or suggestions? Please contact:  
**Maxime Grand** – maxime.grand@sjsu.edu

---

## 📄 License

The sequence and configuration files in this repository are licensed under the  
[Creative Commons Attribution 4.0 International License (CC-BY 4.0)](LICENSE).

This means you are free to **reuse, adapt, and redistribute** the content, **with attribution** to the original authors.

Please note:
- These files are designed specifically for use with the **FloZF software**, developed by **GlobalFIA**.
- FloZF is **proprietary and not open-source**. You must have a valid FloZF license to run these files.
- For software access or licensing inquiries, contact:  
  👉 [https://www.globalfia.com](https://www.globalfia.com)

