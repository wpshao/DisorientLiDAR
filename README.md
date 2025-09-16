# DisorientLiDAR: Physical-World Adversarial Attack on LiDAR-Based Localization for Autonomous Vehicles

## 👥 Authors and Affiliations

| Author | Affiliation |
| :--- | :--- |
| **Yizhen Lao**<sup>#</sup> | College of Information Science and Engineering, Hunan University |
| **Yu Zhang**<sup>#</sup> | College of Information Science and Engineering, Hunan University |
| **Ziting Wang** | College of Information Science and Engineering, Hunan University |
| **Chengbo Wang** | School of Design, Hunan University |
| **Yifei Xue** | School of Design, Hunan University |
| **Wanpeng Shao**<sup>*</sup> | College of Information Science and Engineering, Hunan University |

## 🎯 Abstract

**DisorientLiDAR** is a novel adversarial attack that stealthily disrupts LiDAR-based localization in autonomous vehicles by strategically hiding key 3D regions via near-infrared absorbing materials. Unlike prior works focusing on 3D perception, we target the **localization pipeline**, demonstrating that removing just a few critical keypoints can severely degrade point cloud registration accuracy and induce significant localization drift.

## 🔍 Key Insights

*   **DNN Vulnerability:** We reverse-engineer DNN-based registration models (e.g., HRegNet, D3Feat, GeoTransformer) and show they heavily rely on **local geometric key regions** for point cloud matching.
*   **Practical Attack Vector:** By identifying and **occluding these key areas** (e.g., with IR-absorbing tape), attackers can effectively degrade localization performance in both **simulation (KITTI dataset)** and the **physical world**.
*   **Minimal Perturbation, Maximum Impact:** The attack demonstrates that causing significant localization drift does not require large-scale perturbations, highlighting a critical robustness issue in current systems.

## 🚗 Impact & Evaluation

*   **Causes notable localization errors** on the **Autoware** autonomous driving platform, directly threatening navigation safety and trajectory planning.
*   **Validated on three SOTA point cloud registration models** (HRegNet, D3Feat, GeoTransformer), showing a significant drop in registration accuracy.
*   Successfully **extended to real-world scenarios**, demonstrating the practical feasibility and threat of the attack.

## 🛡️ Defense Suggestions

We propose and discuss the potential of the following mitigation strategies:
*   **Adversarial Training:** Incorporate adversarial examples during model training to improve robustness against such targeted attacks.
*   **Anomaly Detection:** Develop mechanisms to identify point clouds that have been adversarially manipulated by detecting inconsistencies or missing key features.

## 📂 Repository Overview (Code & Data)


> **Note:** We are working on preparing the code and data for public release.

## 🔗 Useful Links

*   📄 **Full Paper:** [Engineered Science, DOI: 10.30919/es1686](http://dx.doi.org/10.30919/es1686)

---

*This README is best viewed on GitHub for the full rendering of Markdown elements.*
