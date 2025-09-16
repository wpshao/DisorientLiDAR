# DisorientLiDAR: Physical-World Adversarial Attack on LiDAR-Based Localization for Autonomous Vehicles

## Authors

- **Yizhen Lao**\(^1,2,#\),  
- **Yu Zhang**\(^1,#\),  
- **Ziting Wang**\(^1\),  
- **Chengbo Wang**\(^2\),  
- **Yifei Xue**\(^2\),  
- **Wanpeng Shao**\(^1,*\)

### Affiliations

^1^ College of Information Science and Engineering, Hunan University,  
No. 2, Lushan South Road, Yuelu District, Changsha, Hunan Province, 410082, China.

^2^ School of Design, Hunan University,  
No. 2, Lushan South Road, Yuelu District, Changsha, Hunan Province, 410082, China.

### Notes

- ^#^ denotes equal contribution.
- ^\*^ denotes corresponding author.
  
DisorientLiDAR is a novel adversarial attack that stealthily disrupts LiDAR-based localization in autonomous vehicles by strategically hiding key 3D regions via near-infrared absorbing materials. Unlike prior works focusing on 3D perception, we target the localization pipeline, demonstrating that removing just a few critical keypoints can severely degrade point cloud registration accuracy and induce significant localization drift.

## 🔍 Key Insights:

- We reverse-engineer DNN-based registration models (e.g., HRegNet, D3Feat, GeoTransformer) and show they heavily rely on local geometric key regions.
- By identifying and occluding these key areas (e.g., with IR-absorbing tape), attackers can degrade localization in both simulation (KITTI) and the physical world.

## 🚗 Impact:

- Causes notable localization errors on Autoware, threatening navigation safety.
- Validated on three SOTA registration models and extended to real-world scenarios.

## 🛡️ Defense Suggestions:
Adversarial training & anomaly detection.

## 📂 Code & data coming soon.

## 🔗 For more details, see our paper [Paper Title / ArXiv Link](#).
@Article{es1686, 
author="Lao, Yizhen and Zhang, Yu and Wang, Ziting Wang Chengbo and Xue, Yifei and Ji, Tie and Shao, Wanpeng", 
title="DisorientLiDAR: Physical Attacks on LiDAR-based Localization", 
journal="Engineered Science", 
year="2025", 
volume="36", 
pages="1686", 
issn="2576-9898", 
doi="10.30919/es1686", 
url="http://dx.doi.org/10.30919/es1686" 
}
