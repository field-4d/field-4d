# FIELD-4D: A Phenotyping Framework for Precision Agricultural Research

---

<div >
<img src="https://avatars.githubusercontent.com/u/71197432?s=400&u=837258e8d4c3b42fe4d44789e3602a3d83b64b61&v=4" alt="F4D Logo" width="230" height="240"> 
 <img src="https://docs.contiki-ng.org/en/master/_static/contiki_logo.png" alt="Contiki-NG Logo" width="256"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Yellow_ribbon.svg/200px-Yellow_ribbon.svg.png" alt="Yellow Ribbon Logo" width="80">
</div>

---

**FIELD-4D** is a modular and extensible **research framework** developed over several years in the **Moshelion Lab** at the Hebrew University of Jerusalem. It is designed to support **real-time outdoor phenotyping**, combining physiological modeling, sensor networks, and scalable cloud infrastructure.

> This repository serves as the central hub of the FIELD-4D ecosystem and integrates three specialized submodules:
> 
> - 📡 **IoT** — environmental sensing, edge computing, and WSN.
> - ☁️ **Cloud** — cloud infrastructure, storage, and APIs.
> - 🧬 **Sci-PHY** — scientific modeling of plant physiology, physics, and phenotypes.

---

## 📁 Repository Structure

```
FIELD-4D/
├── IoT/         # Sensor nodes, data acquisition, field hardware
├── Cloud/       # Cloud integration, APIs, and data pipelines
└── Sci-PHY/     # Physiology models, data analysis, and visualization
```

Each sub-repository is version-controlled independently and contributes to the broader FIELD-4D platform.

---

## Downloading the Repository & Submodules

### A. Downloading Individual Submodules

To download only a specific submodule (e.g., **Cloud**, **IoT**, or **Sci-PHY**) without initializing all submodules:

1. **Clone the main repository without submodules:**
   
   ```sh
   git clone https://github.com/field-4d/field-4d.git
   cd field-4d
   ```

2. **Initialize a specific submodule:**
   
   For example, to download only the **IoT** submodule:
   
   ```sh
   git submodule update --init IoT
   ```

---

### B. Downloading All Submodules

To clone the repository with all submodules in one step:

```sh
git clone --recurse-submodules https://github.com/field-4d/field-4d.git
```

If you already cloned the repository without submodules, initialize all submodules with:

```sh
git submodule update --init --recursive
```

---

## Highlights

- **Research-Driven:** Built on years of empirical research and rigorous field testing.
- **Modular Design:** Flexible integration of multiple sensor types, cloud platforms, and data streams.
- **Scalable Architecture:** Suitable for both small-scale trials and full-scale field deployments.
- **Interdisciplinary Approach:** Merges plant science, physics, and engineering into a cohesive system.
- **Collaboration-Ready:** Tailored for academic partnerships and advanced research initiatives.

---

## Submodules Overview

### 📡 IoT Module (/IoT)

Focuses on field-level data capture and processing:

- Implements wireless sensor network (WSN) protocols.
- Enables power-efficient edge computing.
- Provides real-time measurements of environmental parameters (e.g., temperature, humidity, radiation, VPD).

[View IoT Details »](./IoT)

---

### ☁️ Cloud Module (/Cloud)

Handles cloud infrastructure and data services:

- Integrates with Google Cloud (BigQuery, Firebase, Cloud Run).
- Offers RESTful API endpoints for internal and external applications.
- Employs CI/CD practices, infrastructure-as-code (Terraform), and monitoring solutions.
- Supports data pipelines for real-time and batch processing.

[View Cloud Details »](./Cloud)

---

### 🧬 Sci-PHY Module (/Sci-PHY)

Serves as the scientific engine of the framework:

- Models crop growth and stress responses.
- Simulates light interception, heat balance, and transpiration.
- Supports data processing and visualization (CSV, JSON, NetCDF).
- **Note:** This module may be released as open source for community collaboration.

[View Sci-PHY Details »](./Sci-PHY)

---

## Technologies Used

- **Programming Languages:** Python, C/C++, Bash
- **Frameworks & Tools:** Docker, Terraform, GitHub Actions
- **Cloud Platform:** Google Cloud Platform (BigQuery, Pub/Sub, Firebase)
- **Monitoring:** Prometheus, Grafana, InfluxDB
- **Scientific Libraries:** Pandas, NumPy, Matplotlib, SciPy

---

## Use Cases

- Outdoor phenotyping and physiological experiments.
- Remote crop monitoring and precision irrigation systems.
- Integration with drones, imaging systems, and remote sensing tools.
- Field-ready deployments with research-grade validation.

---

## Collaboration & Access

FIELD-4D is designed for academic and institutional partnerships. While the framework is proprietary, selected modules (such as Sci-PHY) may be shared under an open license upon request. Contributions and collaborations are curated to align with our scientific research objectives.

---

## License

FIELD-4D is a **proprietary academic research framework**. For licensing details and access to specific modules, please refer to the individual submodule documentation or contact us directly.

---

## Developed By

**The Moshelion Lab**  
Robert H. Smith Faculty of Agriculture, Food and Environment  
The Hebrew University of Jerusalem, Rehovot, Israel

- **Idan Ifrach**  
  PhD Student, Hebrew University of Jerusalem, Israel  
  [idan.ifrachi@mail.huji.ac.il](mailto:idan.ifrachi@mail.huji.ac.il) | [GitHub](https://github.com/ifrachi) | [LinkedIn](https://www.linkedin.com/in/ifrachi/) | [ORCID](https://orcid.org/0009-0000-0552-0935)

- **Nir Averbuch**  
  PhD Student, Hebrew University of Jerusalem, Israel  
  [averbuch.nir@gmail.com](mailto:averbuch.nir@gmail.com) | [GitHub](https://github.com/averbuchnir)

- **Shani Friedman**  
  PhD Student, Hebrew University of Jerusalem, Israel  
  [shani.goldfarb@mail.huji.ac.il](mailto:shani.goldfarb@mail.huji.ac.il) | [GitHub](https://github.com/shaniplant)

- **Prof. Menachem Moshelion**  
  Hebrew University of Jerusalem, Israel  
  [menachem.moshelion@mail.huji.ac.il](mailto:menachem.moshelion@mail.huji.ac.il) | [LinkedIn](https://il.linkedin.com/in/menachem-moshelion-45aa689a) | [ORCID](https://orcid.org/0000-0003-0156-2884)

---

## Contact

For institutional inquiries or collaboration opportunities:  
**Email:** [greenroom.lab@mail.huji.ac.il](mailto:greenroom.lab@mail.huji.ac.il)  
**Location:** Rehovot, Israel

---

> *FIELD-4D bridges the complexity of plant science with the power of modern technology.*
