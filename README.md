

# 🌸 dji-neo2-labs // Hardware & 3D Mods 

[![Build Status](https://img.shields.io/badge/OS-DJI_O4-pink?style=flat-square)]()
[![Hardware](https://img.shields.io/badge/Frame-Sub--250g-blueviolet?style=flat-square)]()
[![Theme](https://img.shields.io/badge/Theme-Sakura_Vaporware-ffb7c5?style=flat-square)]()

Toolkit modular focado em otimização de payload, ergonomia e proteção para o ecossistema **DJI Neo 2**. Este repositório centraliza recursos técnicos, assets e arquivos de manufatura aditiva (3D) sob uma estética *cyber-sakura*.

---

## 🛠 Tech Specs (Hardware Profile)

```yaml
drone:
  model: DJI Neo 2
  weight: 151g (dry weight)
  sensor: 1/2-inch CMOS | 12MP | f/2.2
  video_stack: 4K/60fps | 1080p/100fps
  radio_protocol: O4 (Up to 10km FCC / 6km CE)
  storage: 49GB internal flash
  safety: Omnidirectional Obstacle Avoidance + LiDAR Front-end
  flight_time: ~19min (optimal conditions)
```

---

## 📂 Project Structure

```bash
root@dji-neo2-labs:~# tree -L 1
.
├── 🌸 CAD/             # Raw STEP/STL files for mods
├── 📝 docs/            # Technical whitepapers & assembly guides
├── ⚙️ print_configs/   # .3mf profiles (BambuLab/Prusa/Cura)
├── 📦 modules/         # Modular cases & expansion bays
└── 🎨 assets/          # Lo-Fi aesthetics & UI icons
```

---

## ⚡ Hardware Patches (3D Printing)

### 01. Sakura-Box (Modular Case System)
Sistema de transporte articulado otimizado para tolerâncias mecânicas precisas, eliminando a necessidade de magnetos.
- **Features:** Dobradiça *print-in-place*, trava de compressão.
- **Payload:** Drone + RC-N3/Goggles 3/N3 + 2x Flight Batteries + Tools.
- **Print Time:** ~8h @ 200mm/s.
- **Material:** `PLA+` ou `PETG` (para resistência térmica > 50°C).

### 02. Minimalist "Slim-Shell"
Case de baixo perfil para *fast-deployment*.
- **Mounting:** Clipes externos para fixação de bateria e loop para paracord.
- **Custom:** Template disponível para gravação de ID/Logotipo na camada superior.

---

## 🛠 Manufacturing Parameters (Slicer Settings)

Para garantir a integridade estrutural dos mods, utilize os seguintes parâmetros:

| Parameter | Recommended Value |
| :--- | :--- |
| **Layer Height** | 0.20mm (0.12mm for threads) |
| **Wall Loops** | 3 (Minimum) |
| **Infill** | 15% Gyroid (Stress distribution) |
| **Support** | Not required (Optimized geometry) |
| **Material** | Pink/White PETG (Sakura Vibe) |

---

## 🧩 Expansion & Contribution

Se você desenvolveu um *fix* ou novo módulo:

1. **Fork** o repositório.
2. Adicione seu módulo em `/CAD/` (Preferencialmente em `.STEP` para fácil edição).
3. Documente o `BOM` (Bill of Materials) se houver hardware externo (parafusos, vedações).
4. `git commit -m "feat: add ultralight gimbal guard"`
5. **Push** e abra o PR.

---

## 🌸 Gallery & Aesthetics

> *"Code in the morning, fly under the cherry blossoms at dusk."*

![Sakura Lo-Fi Banner](https://img.shields.io/badge/Vibe-Steady-pink)

---

## 📜 License & Legal
Distribuído sob **CC BY-SA 4.0**. 
*Disclaimer: Modificações físicas podem alterar o centro de gravidade (CoG) e a eficiência térmica do hardware original. Use por sua conta e risco.*

```bash
echo "Happy Flying." && exit 0
```

---

### O que mudou nesta versão "Dev Senior":
1.  **YAML/Code Blocks:** Informações técnicas organizadas como arquivos de configuração (`.yaml`) ou saída de terminal (`tree`).
2.  **Linguagem Direta:** Menos adjetivos, mais dados (tolerâncias, CoG, payload, materiais).
3.  **Brevidade:** Seções curtas e escaneáveis.
4.  **Terminologia Maker/Hacker:** Uso de termos como `Bill of Materials (BOM)`, `Print-in-place`, `Gyroid infill`, `Deployment`.
5.  **Branding:** O tema cerejeira foi mantido nos emojis e badges, mas a estrutura do texto é puramente técnica.
