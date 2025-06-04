# FloZF Sequences for pFI-Based Determination of Dissolved Aluminium in Seawater

This repository contains method sequence and configuration files for use with **FloZF software** on the **MiniSIA-2** programmable Flow Injection (pFI) analyzer. These files were developed for the method described in:

**"A matrix-independent method for direct nanomolar dissolved aluminum analysis in seawater using programmable Flow Injection (pFI)"**  
M. M. Grand and M. Hatta, 2025, submitted to *Analytical Chemistry*.

The method uses lumogallion fluorescence detection and includes sequences optimized for both low- and high-Al seawater samples.

---

## 📁 Contents

- `Grand&Hatta_BrijEnhanced_FloZF_sequencefile.xml`  
  → Sequence file optimized for **low-Al seawater (open ocean)**. Includes **Brij** to enhance fluorescence and includes autocalibration routine using a single Al standard prepared in ultrapure water. 

- `Grand&Hatta_NoBrij_FloZF_sequencefile.xml`  
  → Sequence file for **high-Al samples (>400 nM)**. Brij is excluded to avoid signal saturation (note: for high accuracy best to prepared standard manually in low Al seawater, see manuscript for details). 

- `devices.xml`  
  → Defines MiniSIA-2 hardware configuration (valves, pumps, etc.).

- `resource steps.xml`  
  → Contains logic for reagent flow, pump volumes, and resource coordination.

- `sequence log.sqlg.xml`  
  → Required by FloZF to track sequence execution and data logging.

---

## 🧪 How to Use

These files are specific to the **GlobalFIA MiniSIA-2 platform** and require the proprietary **FloZF software**.

### 1. Create a new FloZF Project
- Create a new FloZF project or open an existing one.
- Locate your project directory (e.g., `C:\Users\YourName\Documents\FloZF Projects\YourProject`).

### 2. Copy Configuration Files
Copy the following into the `misc` folder inside your FloZF project. Overwrite any existing files:
- `devices.xml`
- `resource steps.xml`
- `sequence log.sqlg.xml`

### 3. Add Sequence Files
Place the `.xml` sequence files into the `sequences` folder within your FloZF project directory:
- Use `Grand&Hatta_BrijEnhanced_FloZF_sequencefile.xml` for open-ocean samples.
- Use `Grand&Hatta_NoBrij_FloZF_sequencefile.xml` for high-Al samples (>400 nM).

### 4. Load and Run the Sequence
- Launch FloZF.
- Navigate to the **Sequences** tab and load your selected sequence file.
- Ensure reagent compositions, valve positions, and instrument settings match the manuscript.

---

## 🧰 Instrument Setup (Used for Method Development)

| Component          | Specification                               |
|-------------------|----------------------------------------------|
| Analyzer          | MiniSIA-2 (GlobalFIA)                        |
| Detection         | Lumogallion fluorescence assay               |
| Excitation Source | 470 nm LED                                   |
| Emission Filter   | 530 nm bandpass                              |
| Holding Coils     | 1350 µL PTFE, 0.8 mm ID                      |
| Carrier/Reagents  | As described in manuscript                   |
| Software          | FloZF (Windows only, commercial license)     |

Refer to the manuscript for reagent formulations, segment timing, and additional validation details.

---

## 📄 Citation

If you use or adapt these files, please cite:

> Grand, M. M., & Hatta, M. (2025). A matrix-independent method for direct nanomolar dissolved aluminum analysis in seawater using programmable Flow Injection (pFI). Submitted to *Analytical Chemistry*.

---

## 📬 Contact

Questions or feedback? Please reach out:

- **Maxime Grand** – maxime.grand@sjsu.edu  
- **Mariko Hatta** – mhatta@hawaii.edu

---

## 📜 License

These sequence and configuration files are shared under the  
[Creative Commons Attribution 4.0 International License (CC BY 4.0)](LICENSE).

You are free to:
- Share and redistribute the material in any medium or format  
- Adapt, transform, and build upon it for any purpose

**As long as** you provide appropriate credit to the original authors.

> ⚠️ **Note:** FloZF is **proprietary software** developed by **GlobalFIA**. These files require a licensed copy of FloZF to operate.  
> For software access or licensing, visit: [https://www.globalfia.com](https://www.globalfia.com)

---


