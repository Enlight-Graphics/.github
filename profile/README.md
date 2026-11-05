<div align="center">

# ✦ Enlight Graphics ✦

**Next-generation real-time ray tracing, path tracing & temporal reconstruction framework**

[![DirectX 12 Ultimate](https://img.shields.io/badge/DirectX_12-Ultimate-0078D7?style=for-the-badge&logo=windows&logoColor=white)](#)
[![DXR Path Tracing](https://img.shields.io/badge/DXR-Hardware_Accelerated-76B900?style=for-the-badge&logo=nvidia&logoColor=white)](#)
[![DLSS & FSR](https://img.shields.io/badge/Upscaling-DLSS_|_FSR_3-ED1C24?style=for-the-badge&logo=amd&logoColor=white)](#)
[![C++20](https://img.shields.io/badge/C++-20-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)](#)

---

</div>

## 🌌 Overview

**Enlight** is an advanced modular rendering framework engineered to bring modern graphics technologies — including hardware-accelerated path tracing (DXR), neural/temporal reconstruction, and realistic atmospheric simulation — into classic DirectX 9 game environments (GTA San Andreas, MTA, Province).

By offloading rendering into a dedicated **64-bit isolated rendering host**, Enlight bypasses legacy 32-bit memory boundaries and driver constraints, unlocking modern DirectX 12 Ultimate capabilities.

---

## ⚡ Core Architecture

```
[ Game Process (x86) ]
       │
       ▼ (D3D9 Proxy Capture & Frame Hooks)
[ Render Host Channel (High-throughput Shared IPC) ]
       │
       ▼
[ Enlight Render Host (x64 Native Engine) ]
  ├── Hardware Path Tracer (DXR / BVH Traversal)
  ├── NVIDIA NRD & Temporal Denoising Pipeline
  ├── Volumetric Atmosphere & Meteoros Clouds
  ├── AMD FSR / NVIDIA DLSS Frame Generation
  └── Presentation & Modular RmlUi Overlay
```

---

## 🛠️ Organization Repositories

| Repository | Visibility | Description |
| :--- | :---: | :--- |
| **[`EnlightGraphics`](https://github.com/Enlight-Graphics/EnlightGraphics)** | `Public` | 📦 Official distribution repository for pre-built binaries, client releases, and assets. |
| **`Enlight`** | `Private` | ⚙️ Core rendering framework: D3D9 hook proxy, x64 D3D12 render host, and HLSL compute pipelines. |
| **`EnlightLauncher`** | `Private` | 🚀 Modern desktop client: automated updates, hardware profiling, and runtime settings configurator. |
| **`EnlightServer`** | `Private` | 🌐 Cloud backend: release delivery, update verification, and real-time telemetry. |

---

## 🌟 Key Technologies

- **Hardware Path Tracing (DXR)** — Full global illumination, reflections, refractive dielectrics, and physically-based surfaces.
- **Physical Atmosphere & Meteorology** — Rayleigh & Mie scattering, dynamic diurnal cycles, and 3D volumetric cloud fields.
- **Temporal Reconstruction** — DLSS / FSR integration delivering sharp resolution scaling and fluid frame generation.
- **Modular Studio UI** — Hardware-accelerated RmlUi interface with real-time settings configuration and themes.

---

<div align="center">

<sub>Developed by the Enlight Graphics Team</sub>

</div>
