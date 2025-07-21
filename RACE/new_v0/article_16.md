## Abstract

非接触式感知技术在工业自动化、自动驾驶、智能家居和医疗康复等众多领域发挥着日益重要的作用，通过不直接接触物体来获取信息。本研究收集并评估了目前在雷达、Wi-Fi、光学和声学非接触式感知领域中表现最佳的算法策略，并分析了它们的输入信号特性及准确率。

雷达感知方面，其输入信号通常为雷达回波信号、时频图像或合成孔径雷达（SAR）图像，有时也包括IQ数据。深度学习算法，特别是**YOLO系列算法**、卷积神经网络（CNN）、循环神经网络（RNN）和生成对抗网络（GAN），显著提升了目标检测、识别与分类的性能。例如，改进的YOLOv3通过多尺度检测和残差单元优化了小目标检测性能 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])；VGG19在热红外图像目标检测中表现卓越，Faster R-CNN结合ResNet50有效提升了SAR图像船舶和小目标检测精度 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。YOLO算法通过优化骨干网络、注意力机制、多尺度特征融合和损失函数，在速度和精度之间取得了平衡，但仍面临小目标召回率低、复杂背景干扰等挑战 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[9](https://pdf.hanspub.org/csa_1543597.pdf)])。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-13-11992/article_deploy/html/images/applsci-13-11992-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Multi-Sensor Data Fusion Method Based on Self-Attention ...
  </div>
</div>

Wi-Fi感知主要利用无线局域网（WLAN）信号特征，如信号强度（RSSI）或信道状态信息（CSI）的隐含特征，实现室内定位。主要算法包括**指纹定位**和**测距定位**，它们可利用现有Wi-Fi基础设施，部署成本较低 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。虽然部署便捷，但Wi-Fi感知的精度相对有限，且易受多径效应影响 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

光学感知涵盖视觉传感器、深度相机和激光雷达（LiDAR），输入信号包括RGB图像、热红外图像、SAR图像、RGB-D图像以及视频流。**CNN**、**RNN**和**GAN**等深度学习算法广泛应用于光学图像/视频的目标识别、定位和环境感知。改进的Otsu算法提高了深度图像特征提取能力，计算效率提升15%以上 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。然而，传统视觉SLAM易受光照剧烈变化或纹理缺失影响，深度相机对光照稳定性要求高 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-13-11992/article_deploy/html/images/applsci-13-11992-g004.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Multi-Sensor Data Fusion Method Based on Self-Attention ...
  </div>
</div>

多传感器融合系统，特别是**LiDAR-IMU-视觉融合**，通过结合LiDAR点云、IMU惯性数据和视觉图像（RGB/RGB-D）的优势，有效克服了单一传感器的局限性。常见的融合算法包括**扩展卡尔曼滤波（EKF）**、改进的**PL-ICP算法**以及基于注意力机制的深度融合方法 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。这些融合系统显著提升了定位精度和鲁棒性，例如，某EKF融合算法在初始角度偏差45°时仍能保持99.7%以上的定位精度小于0.001m ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])；“视觉+激光”融合系统在KITTI数据集（07）上将最大绝对姿态误差从10.36m降低至1.46m ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。然而，不同传感器数据频率和精度差异、以及动态环境下的鲁棒性仍是挑战 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-13-11992/article_deploy/html/images/applsci-13-11992-g005.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Multi-Sensor Data Fusion Method Based on Self-Attention ...
  </div>
</div>

本研究还探讨了优化策略，如数据增强、超分辨率技术、多尺度特征融合、上下文信息学习、无锚框方法及损失函数优化等，以进一步提升感知性能 ([[8](https://www.opticsjournal.net/Articles/OJ5cbbc2792599d7da/FullText)])。

**常用数据集和评估指标**
*   **权威数据集**：包括用于SAR图像目标识别的MSTAR数据集 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])，自动驾驶领域广泛使用的KITTI数据集 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)])，以及信号调制识别的RML 2018.01数据集 ([[17](https://patents.google.com/patent/CN113298031A/zh)])。
*   **评估指标**：主要包括定位精度（如偏差值、RMSE）、鲁棒性、处理速度，以及分类和检测任务的混淆矩阵、准确率（Accuracy）、精确率（Precision）、召回率（Recall）、F1值、ROC曲线和平均精度（mAP）等 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。

下表总结了主要感知模态的输入信号、代表性最佳算法及典型的准确率或特点：

| 感知模态/系统 | 输入信号特性 | 最佳算法策略（举例） | 准确率/特点 |
| :------------ | :----------- | :------------------- | :---------- |
| **雷达感知**    | 雷达回波信号、SAR图像、时频图像、IQ数据 | YOLO系列 (YOLOv3, YOLO-G, YOLOv5s)、CNN (VGG19, ResNet, Faster R-CNN)、RNN/LSTM、GANs | 高精度目标检测与分类，实时性强，改进YOLOv3优于其他算法 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。 |
| **Wi-Fi感知**   | WLAN信号特征 (RSSI等) | 指纹定位、测距定位、EKF融合 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)]) | 部署方便，成本低，但精度有限，易受多径效应影响 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。 |
| **光学感知**    | RGB图像、热红外图像、SAR图像、RGB-D图像、视频流 | CNN (AlexNet, VGGNet, ResNet)、RNN/LSTM、GANs、SIFT、改进Otsu ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]) | 目标识别和检测性能强，改进Otsu算法计算效率提升15%以上 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。 |
| **多传感器融合** | LiDAR点云、IMU数据、RGB/RGB-D图像、GPS、Wi-Fi定位数据 | EKF、改进PL-ICP、PSO-BP改进UKF、注意力机制融合 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)]) | 高精度、高鲁棒性定位建图。EKF融合定位精度可达99.7%以上小于0.001m ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。KITTI数据集上最大姿态误差显著降低 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。 |

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-13-11992/article_deploy/html/images/applsci-13-11992-g006.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Multi-Sensor Data Fusion Method Based on Self-Attention ...
  </div>
</div>

未来的研究将侧重于算法优化、轻量化、更深层次的多传感器数据融合、构建多样化数据集、提升通用性和鲁棒性，以及结合Transformer等前沿技术，以期在更广泛的实际应用中发挥非接触式感知的巨大潜力 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)]).
## Introduction

非接触式感知技术是指在无需直接物理接触目标物体的情况下，通过收集和分析其发射或反射的能量场（如电磁波、声波等）来获取目标信息的技术。这类技术广泛利用各种非专业传感器，包括但不限于惯性测量单元（IMU）、麦克风、射频收发器（如Wi-Fi和雷达）以及光学传感器（如深度相机和普通摄像头）等，因其具备低成本、低功耗和易于部署的优势，在多个领域展现出巨大的应用潜力 ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)], [[12](https://crad.ict.ac.cn/article/doi/10.7544/issn1000-1239.202440396?viewType=HTML)])。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-11-01235/article_deploy/html/images/applsci-11-01235-g007.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Recent Advances in Wearable Devices for Non-Invasive Sensing
  </div>
</div>

非接触式感知在现代社会中扮演着日益重要的角色，其应用场景极其广泛，涵盖了工业自动化、航空航天、自动驾驶、智能家居以及医疗康复等关键领域 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)])。例如，在工业自动化中，它能实现对生产线上物体的实时监测与识别；在自动驾驶中，则是环境感知和障碍物检测的核心；在智能家居中，可用于人员活动检测与健康监测；而在医疗康复领域，则为患者提供无干扰的生理信号监测和运动评估 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)])。通过避免物理接触，这些技术能够有效提升安全性、卫生性和便利性，特别是在一些特殊或危险环境中，其重要性更为凸显。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/sensors/sensors-18-03953/article_deploy/html/images/sensors-18-03953-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    A Non-Intrusive Approach for Indoor Occupancy Detection in ...
  </div>
</div>

本研究旨在收集和整理目前非接触式感知领域中表现最佳的算法策略，并对它们的输入信号特性及准确率进行评估。为此，本文将深入探讨当前主流的非接触式感知模态，包括雷达感知、Wi-Fi感知、光学感知和声学感知，并详细分析它们所面临的挑战。重点关注各模态下表现优异的算法策略，特别是机器学习和深度学习领域的算法，如卷积神经网络（CNN）、循环神经网络（RNN）、生成对抗网络（GAN）以及YOLO系列算法等，并阐述多传感器融合（尤其是LiDAR-IMU-视觉融合）技术如何进一步提升感知系统的整体性能。

本文结构如下：第二章将概述雷达、Wi-Fi、光学和声学等主要感知模态的特点及其各自的挑战。第三章将详细介绍当前非接触式感知领域中领先的算法策略，包括基于机器学习、深度学习及多传感器融合的方法，并着重评估它们在不同输入信号下的准确率表现。第四章将列举非接触式感知技术的典型应用案例。最后，第五章将对全文进行总结，并对非接触式感知技术的未来发展方向进行展望。通过对这些先进算法和融合策略的系统性评估，本研究旨在为非接触式感知领域的进一步发展提供有价值的参考和指导。
# 非接触式感知模态概述

非接触式感知技术通过在不直接接触物体的情况下获取信息，在工业自动化、航空航天、自动驾驶、智能家居以及医疗康复等众多领域中发挥着越来越重要的作用 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)]。这些技术通常利用各种非专业传感器，如惯性测量单元（IMU）、麦克风、射频收发器（包括Wi-Fi和雷达）以及光学传感器（如深度相机和普通摄像头）来完成感知任务，它们具有低成本、低功耗和易部署的优点 [[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)], [[12](https://crad.ict.ac.cn/article/doi/10.7544/issn1000-1239.202440396?viewType=HTML)]。当前非接触式感知领域主要涵盖雷达、Wi-Fi、光学和声学等多种模态。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="http://www.aas.net.cn/fileZDHXB/journal/article/zdhxb/2025/1/PIC/AAS-CN-2023-0809-9.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    非接触式感知在工业巡检中的应用
  </div>
</div>

### 1.1 雷达感知 (Radar Sensing)

雷达感知通过发射和接收电磁波来探测、识别和跟踪目标物体，其核心在于利用电磁波在传播过程中与目标相互作用后携带的信息。该模态广泛应用于军事侦察、民用监测和交通管理等领域 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。在自动驾驶等新兴应用中，毫米波雷达也能有效用于汽车目标检测与分类 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。

*   **优势:**
    *   **环境适应性强:** 雷达信号不易受光照、灰尘、雨雪、雾霾等恶劣天气条件影响，能快速获取高精度环境信息，使其适用于各种复杂光照和环境条件 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **高精度与实时性:** 在工业自动化、航空航天、自动驾驶等对实时性要求高的领域，雷达信号的目标检测是关键技术，能够提供高精度的距离、速度和角度信息 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。

*   **挑战:**
    *   **复杂环境下的性能下降:** 在低信噪比、多目标、高杂波等复杂环境下，传统雷达检测方法精度容易下降，易出现漏检或虚警现象 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
    *   **成本与易受影响:** 尽管文档中提到多线激光雷达成本昂贵且易受雨、尘影响 [[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)]，这在一定程度上反映了高精度雷达（特别是激光雷达）面临的共性挑战，即高级传感器的成本和环境敏感性问题。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://radars.ac.cn/fileLDXB/journal/article/ldxb/2021/3/R20113-1.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    雷达通信频谱共享
  </div>
</div>

### 1.2 Wi-Fi感知 (Wi-Fi Sensing)

Wi-Fi感知利用无线局域网（WLAN）信号的特征（如信号强度RSSI、信道状态信息CSI、信号飞行时间ToF）来确定设备位置或感知环境，例如通过信号指纹、测距等方法。该技术广泛应用于商场、医院、机场等室内环境的定位和人机交互 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。

*   **优势:**
    *   **部署便捷与低成本:** Wi-Fi感知可以利用现有的Wi-Fi基础设施进行部署，无需额外购置昂贵的硬件设备，从而大大降低了部署成本，具有较高的经济性 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **广泛可用性:** 几乎所有智能设备都支持Wi-Fi功能，使得该技术具有极高的普及率和易用性。

*   **挑战:**
    *   **精度限制与多径效应:** Wi-Fi感知的定位精度相对有限，且易受室内环境中多径效应（信号通过不同路径到达接收端，造成干扰）的影响，导致感知结果不够稳定和准确 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **低功耗感知共性挑战:** 在追求低功耗的感知场景中，Wi-Fi感知面临跨域信号弱相关、通信感知弱兼容以及感知设备弱资源等共性挑战 [[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)], [[12](https://crad.ict.ac.cn/article/doi/10.7544/issn1000-1239.202440396?viewType=HTML)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://radars.ac.cn/fileLDXB/journal/article/ldxb/2025/1/R24189-1.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    无线信号人体姿态估计
  </div>
</div>

### 1.3 光学感知 (Optical Sensing)

光学感知模态通过捕捉光线信息来理解环境，主要涵盖视觉传感器（如普通相机）、深度相机和激光雷达（LiDAR）等。

*   **优势:**
    *   **视觉传感器（相机）:** 成本低廉，覆盖范围广，能够提供极其丰富的环境特征信息（如纹理、颜色、形状），符合人类视觉直观感受，易于理解和处理 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **深度相机:** 除了常规图像信息外，还能提供物体与传感器之间的深度信息，这显著提升了同步定位与建图（SLAM）的精度，并能够实时识别和重建物体表面，对于三维环境感知至关重要 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **激光雷达 (LiDAR):** 能够提供高精度、高密度的三维点云数据，直接获取环境的几何结构信息，且受光照变化影响小。

*   **挑战:**
    *   **视觉SLAM的局限性:** 传统的视觉SLAM（同步定位与建图）方法易受光照剧烈变化、纹理缺失区域以及相机快速运动带来的模糊影响，导致定位精度下降，存在累积误差导致的漂移问题和尺度不确定性 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **深度相机的环境要求:** 深度相机对光照稳定性要求较高，主要适用于光照条件相对稳定的室内环境或特定场景，在室外强光或暗光条件下性能会大幅下降 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
    *   **多传感器融合的复杂性:** 将视觉信息与其他传感器数据进行融合时，可能会导致时延增加和融合设计复杂，需要精巧的算法来保证数据同步和一致性 [[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://img4.pconline.com.cn/pconline/images/pconline_cms/20240704/21267575.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    光学影像设备
  </div>
</div>

### 1.4 声学感知 (Acoustic Sensing)

声学感知利用声波进行信息获取，通过分析声波在传播、反射、衰减过程中的变化来感知环境或目标状态。该模态通常使用麦克风作为主要的感知设备，可用于多种任务，例如环境声学分析和人体生理信号监测 [[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)], [[12](https://crad.ict.ac.cn/article/doi/10.7544/issn1000-1239.202440396?viewType=HTML)]。

*   **优势:**
    *   **设备普及与低成本:** 麦克风作为一种通用设备，成本低廉且易于获取和集成，使其在多种非接触式感知任务中具有广泛的应用潜力 [[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)], [[12](https://crad.ict.ac.cn/article/doi/10.7544/issn1000-1239.202440396?viewType=HTML)]。
    *   **非侵入性:** 通过麦克风阵列或单个麦克风即可实现对环境或人体生理信号的感知，无需物理接触，提升了用户体验和便利性。

*   **挑战:**
    *   **生物电信号的干扰:** 在医疗康复等领域，声学感知有时会与生物电信号（如表面肌电sEMG、脑电图EEG）结合使用。其中，表面肌电（sEMG）信号采集易受其他电信号干扰，需要复杂的滤波和放大处理以保证信号质量 [source]6。
    *   **信号弱与噪声敏感:** 脑电图（EEG）信号极其微弱且非平稳，极易受到外部噪声（如工频干扰、眼电、肌电等）污染，导致采集和处理过程繁琐，对设备和算法要求较高 [source]6。
    *   **环境噪声干扰:** 声学感知容易受到背景噪声和回声的影响，降低感知准确性，需要复杂的信号处理算法进行去噪和分离。
# 最佳算法策略及其评估

非接触式感知技术通过利用雷达、Wi-Fi、光学和声学等多种模态获取环境信息，在自动驾驶、智能家居、医疗康复等众多领域发挥着关键作用。为了应对复杂多变的感知挑战，研究人员开发并应用了多样化的算法策略，其中机器学习和深度学习算法占据主流，并与多传感器融合技术相结合，以显著提升感知系统的性能。本节将详细阐述目前非接触式感知领域最先进的算法策略，并评估它们的输入信号特性与准确率。

## 1. 雷达感知YOLO系列算法

雷达感知通过发射和接收电磁波来探测、识别和跟踪目标物体，尤其在工业自动化、航空航天、自动驾驶等领域中，雷达信号的目标检测是关键技术 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。传统的雷达检测方法在低信噪比、多目标和高杂波等复杂环境下，精度往往下降，易出现漏检或虚警 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。为此，深度学习方法，特别是YOLO系列算法，因其自动学习深层次特征的能力，被广泛应用于提升雷达目标检测性能。

### 1.1 输入信号特性

雷达感知YOLO系列算法的输入信号通常是雷达回波信号经过预处理后的数据。这些信号特性包括：
*   **雷达回波信号**：原始IQ（In-phase/Quadrature）数据或其衍生的幅度和相位信息，可能经过滤波、去噪等预处理 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[17](https://patents.google.com/patent/CN113298031A/zh)])。
*   **时频图像**：对于高速机动目标，雷达回波信号常通过时频分析（如短时傅里叶变换、小波变换）转换成时频图像，将目标的微多普勒效应等动态特征可视化，作为YOLO网络的输入 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **合成孔径雷达（SAR）图像**：对于SAR系统，输入通常是振幅图像，有时也会结合散射中心特征，用于目标检测与识别，如船舶检测或军事目标识别 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **多普勒频移特征**：对于运动目标，其在快时间维度下的多普勒频移特性是关键输入，YOLOv5s模型可直接检测和分类这类特征 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。

### 1.2 算法与特性

YOLO (You Only Look Once) 算法以其高效和实时性强而闻名，能够在雷达信号处理中实现目标检测与分类的有效整合 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **改进的YOLOv3多尺度目标检测**：为优化小目标检测性能，该算法通过IOU（交并数）推导选择更合适的锚框，并将检测尺度从3个扩展到4个；同时，整合卷积层为残差单元，以避免梯度衰减并增强特征复用性 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **YOLO-G模型**：针对军事目标检测，引入轻量级GhostNet作为特征提取骨干网络，并通过坐标注意力块增强目标特征表示能力、抑制干扰。结合DIOU损失函数和Focal Loss函数，进一步提升了检测精度 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
*   **基于YOLOv5s的雷达运动目标智能检测与识别**：该模型通过构建专用数据集，处理雷达接收回波信号，能够准确检测并分类运动目标的多普勒频移特征 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **结合DenseNet的YOLOv3改进模型**：针对遥感目标检测中尺度差异大、分布密集和背景复杂等挑战，引入DenseNet以增强特征提取能力，并将检测量表增加至4个，从而提升对不同尺度目标的检测性能 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **双波束SAR中的YOLO网络**：用于强杂波环境下的慢速移动目标检测与分类，并能有效排除静止目标 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **YOLOv8**：在自动驾驶等领域，YOLOv8在速度、精度和易用性之间实现了平衡，通过RepConv、C2f结构、Anchor-Free范式、TaskAlignedAssigner、SIoU/WIoU损失等优化，显著提升了交通标志、车辆等目标的实时检测能力 [[9](https://pdf.hanspub.org/csa_1543597.pdf)], [[11](https://www.opticsjournal.net/Articles/OJ8d249a888feac672/FullText)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://pub.mdpi-res.com/electronics/electronics-14-01104/article_deploy/html/images/electronics-14-01104-g001.png?1741859395" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Object Detection YOLO Algorithms and Their Industrial ...
  </div>
</div>

### 1.3 准确率与挑战

YOLO系列算法在雷达目标检测中展现出优越的性能，尤其是在处理速度和精度方面。
*   **准确率**：改进的YOLOv3算法在特定雷达目标检测任务中，其性能优于其他一些先进目标检测算法 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。YOLO-G模型通过结合注意力机制等改进，也显著提高了军事目标检测的准确性 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **挑战**：尽管YOLO系列算法在雷达感知中取得了显著进展，但仍面临一些挑战，如小目标召回率低、复杂背景干扰、高计算资源需求以及在多目标密集场景下性能下降等问题 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。

### 1.4 相关数据集

*   **MSTAR（Moving and Stationary Target Acquisition and Recognition）数据集**：主要用于合成孔径雷达（SAR）系统目标识别的权威数据集。许多深度学习模型，如FEC框架，在该数据集上的目标分类和识别任务中展现出优异的有效性和鲁棒性 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **自定义战场军事目标识别数据集**：包含多种军事目标，用于评估不同CNN模型在雷达信号识别任务中的性能 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **针对雷达移动目标的自定义数据集**：专门为训练YOLOv5s模型而构建，用于识别雷达运动目标的多普勒频移特征 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。

## 2. Wi-Fi CSI感知算法

Wi-Fi感知利用无线局域网（WLAN）信号特征来确定设备位置或感知环境，在商场、医院、机场等室内环境中应用广泛 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。虽然搜索结果中未直接提及“CSI”（信道状态信息），但提供了Wi-Fi定位算法的详细信息，其核心正是对信号特性的利用。

### 2.1 输入信号特性与模态

Wi-Fi定位技术通过分析无线信号来确定位置。主要输入信号特性包括：
*   **RSSI（Received Signal Strength Indicator）**：接收信号强度指示，这是最常见的Wi-Fi信号特征，用于构建指纹库。指纹定位方法通过预先采集区域内不同位置的RSSI值建立指纹库，定位时将实时采集的RSSI与指纹库匹配 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **TOF（Time of Flight）**：信号飞行时间，用于基于测距的定位方法，通过测量信号从发射到接收所需时间来计算距离 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **AOA（Angle of Arrival）**：信号到达角，通过测量信号到达接收天线阵列的角度来确定信号源方向。

本报告主要来源侧重于**指纹定位**方法，因为它不需要精确了解信号源位置，不易受多径效应和非视距传播的显著影响，能在复杂室内环境中提供较稳定的定位服务，且部署成本较低，利用现有Wi-Fi基础设施即可实现 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

### 2.2 算法与特性

Wi-Fi定位算法主要包括：
*   **指纹定位**：
    *   **算法原理**：离线阶段采集不同位置点的RSSI指纹信息，构建指纹数据库。在线定位阶段，实时测量待定位点的RSSI，并与数据库中的指纹进行匹配，根据匹配结果估算位置。
    *   **优势**：部署方便，利用现有Wi-Fi基础设施，无需额外硬件设备，成本较低 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   **应用**：在多传感器融合定位框架中，Wi-Fi定位结果可与其他传感器测量值（如激光雷达、深度相机、IMU）进行融合。例如，在基于扩展卡尔曼滤波（EKF）的融合框架下，Wi-Fi定位数据可作为一项输入进行融合，以提升定位的准确性和鲁棒性 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **测距定位**：通过计算设备与已知位置的信号源之间的距离，利用三角测量或多边测量模型确定位置 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

### 2.3 准确率与挑战

Wi-Fi感知技术虽然部署便捷，但其固有的精度限制和易受环境因素影响是主要挑战。
*   **准确率**：Wi-Fi信号定位的精度通常有限 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。虽然具体精度值未在提供的资料中明确指出，但普遍认为其定位精度不如激光雷达等高精度传感器。
*   **挑战**：Wi-Fi信号感知易受多径效应影响，即信号在传播过程中会遇到反射、散射和衍射，导致同一信号沿不同路径到达接收端，从而干扰信号特征的稳定性和准确性 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。此外，信号穿透墙壁等障碍物会造成衰减，进一步影响精度。

## 3. 光学图像/视频深度学习算法

光学感知涵盖视觉传感器（相机）、深度相机和激光雷达（LiDAR）等，通过捕捉光线信息来理解环境。结合深度学习算法，光学感知在目标识别、定位和环境感知方面具有广泛应用 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。

### 3.1 输入信号特性

光学图像/视频深度学习算法的输入信号形式多样：
*   **RGB图像**：由普通摄像头（视觉传感器）采集的彩色图像，提供丰富的纹理和颜色信息，是自动化驾驶中常用的2D环境表示 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。
*   **热红外图像**：在低光照或夜间环境下，热红外相机捕捉的热量辐射图像，可用于目标识别 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **SAR图像**：虽然是雷达模态，但SAR图像的性质使其常与光学图像处理算法结合，用于军事目标或船舶检测 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **RGB-D图像**：由深度相机（如Kinect）采集，除了RGB彩色信息外，还包含每个像素的深度信息，显著提升SLAM精度，并能实时识别和重建物体表面 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **视频流**：实时获取的连续图像序列，可能需要进行视频帧预处理，如去噪、增强、尺度调整，再作为深度学习模型的输入 ([[18](https://patents.google.com/patent/CN117726687B/zh)])。

### 3.2 算法与特性

深度学习算法，特别是各种卷积神经网络（CNN）及其变体，是处理光学图像/视频数据的主流。
*   **卷积神经网络（CNN）**：通过卷积层、池化层和全连接层自动提取图像的多层次特征，在图像处理任务中表现优异 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
    *   **经典CNN模型**：AlexNet、VGGNet（VGG16, VGG19）、ResNet（ResNet50）、GoogLeNet等被广泛应用于军事目标识别和SAR图像目标识别等任务中 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
    *   **特征金字塔融合轻量级CNN**：结合多尺度空间理论和轻量级网络，可提高在低信噪比条件下雷达目标识别（类比图像识别）的准确性和鲁棒性 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
    *   **FEC框架**：基于改进的VGGNet，通过引入判别相关性分析（DCA）增强特征融合效果，用于SAR系统目标识别 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
    *   **Faster R-CNN**：结合ResNet50作为骨干网络，有效应用于SAR图像中的船舶检测及小目标检测，提高了检测精度和速度 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **循环神经网络（RNN）和长短时记忆网络（LSTM）**：虽然主要用于序列数据，但在结合图像特征处理时序信息（如视频中的行为识别）时也展现出能力，如结合频谱图和微多普勒特征进行人体运动识别 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **生成对抗网络（GAN）**：用于生成逼真的图像数据以增强训练数据集的多样性，提升模型泛化能力。例如，在SAR目标识别中解决数据不足问题 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **SIFT算法**：在视觉定位中，SIFT（尺度不变特征转换）算法用于提取视频帧中的特征点，结合2D-3D点对和solvePnP算法计算摄像机位姿，实现高精度的视觉重定位 ([[18](https://patents.google.com/patent/CN117726687B/zh)])。
*   **改进的Otsu算法**：用于深度图像的特征提取，通过选取多个阈值进行二值化，提高处理速度和分割质量，能够精准区分不同距离的目标物体并保留目标轮廓特征 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

### 3.3 准确率与挑战

光学图像/视频深度学习算法在性能上取得了显著提升，但也存在固有挑战。
*   **准确率**：
    *   CNNs通过自动学习深层次特征，显著提升图像目标检测性能，尤其在复杂环境下优于传统方法 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
    *   VGG19在FLIR热红外数据集上表现卓越 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])，ResNet和VGGNet的平均精度优于AlexNet ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
    *   Faster R-CNN结合ResNet50骨干网络有效改进了SAR图像船舶检测的精度和速度，特别提高了小目标检测精度 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
    *   改进的Otsu算法在计算效率上优于K-means和曲线变换算法15%以上，并能有效保留目标基本特征 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   结合实景三维数据和视频的视觉重定位方法，提高了视觉定位的精度和效率 ([[18](https://patents.google.com/patent/CN117726687B/zh)])。
*   **挑战**：
    *   传统视觉传感器易受光照剧烈变化、纹理缺失区域以及动态环境的影响，存在漂移问题和尺度不确定性 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)], [[18](https://patents.google.com/patent/CN117726687B/zh)])。
    *   深度相机对光照条件稳定性要求高，主要适用于光照稳定的室内环境 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   CNN模型仍面临梯度消失、过拟合、稳定性与泛化能力不足、对数据集规模和质量的限制以及小目标漏检等问题 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。

## 4. 多传感器融合（LiDAR-IMU-视觉）系统

多传感器融合技术是提升非接触式感知系统整体性能的有效途径，通过优势互补解决单一传感器局限性，在机器人室内定位、导航和自动驾驶中扮演核心角色 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。

### 4.1 输入信号特性

多传感器融合系统集成了多种模态的传感器数据：
*   **LiDAR（激光雷达）**：提供高精度、高密度的环境几何信息（点云数据：x,y,z坐标和激光反射强度i），不受光照条件影响 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。其数据可转换为距离图像 ([[16](https://patents.google.com/patent/CN113065590B/zh)])。
*   **IMU（惯性测量单元）**：提供机器人的线性加速度和角速度信息，更新频率高，对自主导航和姿态控制至关重要 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
*   **视觉传感器（相机/深度相机）**：
    *   **相机RGB图像**：提供丰富的纹理和颜色信息，成本低，覆盖范围广 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。
    *   **深度相机/RGB-D图像**：提供深度信息，有助于提升SLAM精度 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **GPS（全球定位系统）**：提供全天候、全球覆盖的绝对位置信息，且误差不随时间累积 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
*   **Wi-Fi定位数据**：作为绝对位置参考，可用于修正长期运行的累积误差，但其精度有限 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

### 4.2 融合算法与特性

多传感器融合系统通常采用分层或紧耦合的架构，以提高定位和环境感知的准确性和鲁棒性。
*   **扩展卡尔曼滤波（EKF）**：常用融合算法，能融合来自多个传感器的数据，解决障碍物遮挡导致的点云失准问题 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。在SLAM算法中用于分离机器人姿态估计和地图建模，提高效率和精度 ([[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)])。
*   **改进的PL-ICP（Point-to-Line Iterative Closest Point）算法**：在LiDAR-惯性里程计（LIO）子系统中用于点云配准，通过引入特征点约束和自适应权重策略，显著提升遮挡场景下的点云匹配精度和速度（收敛时间从310毫秒减少到260毫秒） ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **紧耦合LiDAR-IMU融合（如Fast-LIO 2）**：利用IMU预积分去除激光雷达点云畸变，并通过激光雷达里程计消除IMU累积误差，实现高精度建图与定位。后端图优化增加回环检测因子、激光雷达里程计因子、IMU预积分因子，提升定位建图的全局一致性 [[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)]。
*   **基于PSO-BP改进UKF的组合导航系统**：在一级融合中结合惯性导航系统（INS）与GPS，通过训练好的神经网络在GPS信号丢失时进行误差校正，输出更精确的速度和坐标信息作为全局绝对位置约束，并有效减小IMU偏置和噪声 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
*   **“视觉+激光”二级融合系统**：结合VIO（视觉惯性里程计）和LIO（雷达惯性里程计），VIO利用激光雷达为视觉特征提供深度信息，LIO采用VIO提供的位姿预测信息进行点云快速配准，实现高精度和高鲁棒性实时定位 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
*   **基于注意力机制的视觉与激光雷达多模态数据融合**：将点云数据转换为距离图像，与RGB图像共同输入融合模型，通过自注意力机制进行深度融合，旨在有效提升点云信息量，提高3D目标检测算法精度，尤其对行人、骑行者等小目标 ([[16](https://patents.google.com/patent/CN113065590B/zh)])。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://pub.mdpi-res.com/remotesensing/remotesensing-14-02835/article_deploy/html/images/remotesensing-14-02835-g001.png?1655128234" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    A Review of Multi-Sensor Fusion SLAM Systems Based on 3D LIDAR
  </div>
</div>

### 4.3 准确率与挑战

多传感器融合显著提升了系统的定位精度和鲁棒性。
*   **准确率**：
    *   多传感器融合EKF算法在定位精度上优于单一改进PL-ICP方法和传感器SLAM方法，在初始角度偏差达45°时仍能保持99.7%以上的定位精度小于0.001m ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   “视觉+激光”融合地图构建效果更精确，道路旁房屋建筑识别更精细，地图元素更丰富 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
    *   在KITTI数据集（07）上，改进后的算法使绝对姿态误差显著降低：最大误差从10.36m降至1.46m，平均误差从1.97m降至0.60m ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
    *   基于注意力机制的视觉与激光雷达融合方法可以增加3D目标检测精度，尤其对行人、骑行的人等小目标有明显精度提升 ([[16](https://patents.google.com/patent/CN113065590B/zh)])。
*   **挑战**：
    *   室内环境中障碍物遮挡导致点云匹配不准确，不同传感器数据频率和精度差异导致融合困难 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   IMU长时间测量存在积分漂移和误差累积问题 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
    *   GPS在卫星信号受阻区域（如城市峡谷、茂密树林）精度大幅下降甚至失效 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
    *   简单地对激光雷达点云和相机RGB图像进行像素级融合可能产生负面作用，降低感知精度 ([[16](https://patents.google.com/patent/CN113065590B/zh)])。
    *   点云的稀疏性和无序性限制了激光雷达的独立检测能力 ([[16](https://patents.google.com/patent/CN113065590B/zh)])。

### 4.4 相关数据集

*   **YAHBOOM ROSMASTER X3小车**：作为实验平台，配备思岚A1激光雷达和Astra深度相机传感器，用于验证多传感器融合定位的有效性 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **KITTI数据集**：广泛用于自动驾驶领域的公开数据集，包含激光雷达点云数据、相机RGB图像、IMU数据和GPS数据，是评估3D目标检测、定位和环境感知任务的权威基准 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。

## 5. 权威数据集与评估指标

为了客观评估非接触式感知算法的性能，研究界建立了多个权威数据集并采用一系列标准化的评估指标。

### 5.1 权威数据集

*   **MSTAR数据集**：作为合成孔径雷达（SAR）目标识别领域的黄金标准，提供了多种军事目标的SAR图像数据，用于评估不同算法在目标分类和识别任务中的性能和鲁棒性 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **KITTI数据集**：在自动驾驶和机器人领域广受欢迎，包含真实世界场景下的立体相机图像、激光雷达点云、IMU和GPS数据。它被广泛用于评估3D目标检测、物体跟踪、视觉里程计/SLAM和立体匹配等任务 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。
*   **RML 2018.01数据集**：这是一个开放源代码的信号调制识别数据集，包含24种不同的调制方式的IQ数据。它被广泛用于评估雷达信号（IQ数据）的调制识别算法，具有很高的挑战性 ([[17](https://patents.google.com/patent/CN113298031A/zh)])。
*   **FLIR热红外数据集**：用于评估基于CNN的深度特征提取器在热红外图像中目标识别的鲁棒性 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。

### 5.2 评估指标

机器学习和深度学习算法在感知任务中常用的评估指标包括：
*   **定位精度（Localization Accuracy）**：通过将融合后的传感器数据与地面真实数据（Ground Truth）进行对齐，计算两者之间的偏差来衡量定位的准确性。通常以米和弧度表示误差值，并计算在特定精度区间（如<0.001m）内定位成功的概率 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **鲁棒性（Robustness）**：评估系统在面对障碍物、复杂背景干扰、恶劣天气或动态环境等挑战性条件下，能否保持准确和稳定的感知能力 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **处理速度（Processing Speed）/实时性（Real-time Capability）**：衡量算法或融合过程的运行时间，确保其能在实时或可接受的时间范围内完成感知任务 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **平均绝对姿态误差 (Absolute Pose Error, APE)**：衡量机器人轨迹的整体准确性，包括最大值 (Max)、平均值 (Mean)、中位数 (Median)、最小值 (Min)、均方根误差 (RMSE)、误差平方和 (SSE) 和标准差 (Std) 等统计量 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
*   **混淆矩阵（Confusion Matrix）**：分类任务的基础，通过表格形式展示真阳性（TP）、真阴性（TN）、假阳性（FP）、假阴性（FN）的数量 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **精确率 (Precision / 查准率)**：在所有被预测为正例的样本中，实际为正例的比例：TP / (TP + FP) ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **召回率 (Recall / 查全率 / 真正例率 TPR)**：在所有实际为正例的样本中，被正确识别为正例的比例：TP / (TP + FN) ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **F1值 (F1-score)**：精确率和召回率的调和平均值，综合反映了模型的性能：2 * (Precision * Recall) / (Precision + Recall) ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **平均精度（mAP, Mean Average Precision）**：目标检测任务中最常用的评估指标，通过计算所有类别的平均准确率的平均值来衡量模型的检测性能 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **假正例率 (FPR)**：所有负例的样本中，被错误预测为正例的比例：FP / (TN + FP) ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **P-R曲线 (Precision-Recall Curve)**：通过在不同分类阈值下绘制精确率与召回率的关系曲线，用于评估模型在正负样本不平衡数据集上的性能 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **ROC曲线 (Receiver Operating Characteristic Curve)**：通过绘制不同分类阈值下的真正例率（TPR）和假正例率（FPR）的关系曲线，用于评估二分类模型的性能 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **AUC (Area Under ROC Curve)**：ROC曲线下的面积，值越接近1表示分类器性能越好 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **敏感性 (Sensitivity / 灵敏度)**：实际为阳性的样本中，被判断为阳性的比例：TP / (TP + FN)（与召回率相同） ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。
*   **特异性 (Specificity / 特异度)**：实际为阴性的样本中，被判断为阴性的比例：TN / (TN + FP) ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。

这些评估指标能够量化模型在分类、回归、检测等不同任务中的表现，为研究人员和工程师比较不同算法的优劣、指导模型优化提供了客观依据。

## 6. 总结与展望

非接触式感知技术通过融合多种传感器模态和先进的机器学习/深度学习算法，在解决传统方法局限性方面取得了显著进展。雷达、Wi-Fi、光学和声学等传感器的协同工作，结合CNN、RNN、GAN、YOLO、Transformer等深度学习模型以及EKF、PL-ICP等融合算法，能够有效应对复杂环境中的目标检测、定位、识别和跟踪等挑战。

未来的研究方向包括：
*   **算法优化**：进一步提升深度学习算法的鲁棒性、实时性，并提高其在复杂应用环境中的适应能力。例如，克服梯度问题、过拟合、模式崩溃等挑战 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **轻量化算法**：发展高效、轻量化的算法以适应资源受限的环境（如无人机、小型移动平台）和边缘计算平台 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[9](https://pdf.hanspub.org/csa_1543597.pdf)])。
*   **多传感器数据深度融合**：探索更高级别的多传感器数据融合策略，如引入智能算法（深度学习）实现环路闭合约束，以提升导航和定位的精度和密度 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **数据集建设**：针对小目标和特定应用场景，构建更大规模、更多样化、标注更完善的数据集，并研究弱监督或无监督学习方法以减少对大量标注数据的依赖 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[8](https://www.opticsjournal.net/Articles/OJ5cbbc2792599d7da/FullText)])。
*   **通用性与鲁棒性**：提升算法在不同场景下的通用性和应对极端条件（如恶劣天气、严重遮挡）的鲁棒性 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)])。
*   **结合前沿技术**：探索将Transformer、领域自适应、强化学习等技术与现有方法结合，以应对更具挑战性的感知任务 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)])。

通过持续的创新和跨学科的融合，非接触式感知技术有望在更广泛的实际应用中发挥巨大潜力。
# 非接触式感知应用案例

非接触式感知技术利用多种模态传感器及其先进算法，在不直接接触目标的情况下获取环境和目标信息，已广泛应用于工业自动化、航空航天、自动驾驶、智能家居、医疗康复等诸多领域。这些应用案例展现了非接触式感知技术在提升效率、保障安全和改善生活质量方面的巨大潜力 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)], [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)])。

以下是目前非接触式感知领域中具有代表性的应用案例及其所采用的核心算法策略、输入信号特性与准确率评估：

| 感知模态 | 应用场景 | 算法策略举例 | 效果/特点 | 来源 |
|---|---|---|---|---|
| 雷达 | 自动驾驶目标检测 | 深度学习算法 (CNN, RNN, GAN, YOLO等) | 提高检测精度和处理速度，处理复杂环境下的多目标、高杂波问题 | ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]) |
| 雷达/LiDAR | 机器人室内定位和导航 | 多传感器融合 (LiDAR, 深度相机, Wi-Fi, IMU) + 改进PL-ICP + 改进Otsu + EKF | 提高定位精度和稳定性，增强遮挡场景下的点云匹配和特征提取 | ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]) |
| LiDAR | 园区三维建图 (自动驾驶) | LiDAR + IMU 紧耦合 + 后端图优化 (回环检测, IMU预积分) + iVox结构 | 提升位姿估计精度和地图构建精度，消除累积误差 | ([[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)]) |
| LiDAR | 室内同步定位与建图及自主导航 | 单线2D-LiDAR + IMU畸变矫正 + Gmapping算法 + Dijkstra路径规划 | 快速获取环境信息，良好建图性能，低时延自主导航与避障 | ([[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)]) |
| LiDAR | 输电线路智能预警评估 | 机载LiDAR扫描系统获取点云和光学影像 + 三维建模 + 数据分析与判断 + 预警 | 快速高精度三维量测和空间分析，用于弧垂计算、风偏校核、隐患分析等 | ([[5](https://patents.google.com/patent/CN105244805A/zh)]) |
| 光学/视觉 | 自动驾驶汽车检测 | YOLO系列算法 (YOLOv3, YOLOv7, YOLOv8及其改进) | 实时监测车辆、行人、交通标志、交通灯等，具有更快的速度和更高的精确度 | ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[9](https://pdf.hanspub.org/csa_1543597.pdf)], [[11](https://www.opticsjournal.net/Articles/OJ8d249a888feac672/FullText)]) |
| 光学/深度传感器 | 脑卒中患者上肢功能智能评估 | IMU, sEMG, 深度传感器, EEG + 机器学习算法 (多元线性回归, CNN, RNN, SVM, KNN, 随机森林, 模糊支持向量机等) | 提供客观、精准的评估数据，缩短评估时间，提高结果一致性 | ([[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)]) |
| Wi-Fi | 室内定位 | 指纹定位和测距定位；EKF融合 | 提供位置参考，适用于多种室内场景 | ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)]) |
| 声学 | 生理感知 | 麦克风信号分析 | 用于呼吸、心跳、打鼾等生理信号监测，用户认证等 | ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)]) |

### 1. 雷达感知应用案例

雷达感知通过发射和接收电磁波来探测、识别和跟踪目标物体，在自动驾驶等高精度、全天候要求的场景中发挥关键作用 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。

#### 1.1 自动驾驶目标检测

*   **应用场景：** 自动驾驶系统需要实时、准确地检测和识别车辆、行人及其他障碍物，尤其是在复杂环境（如恶劣天气、低光照）下，雷达感知是重要的补充模态。
*   **输入信号特性：** 雷达感知YOLO系列算法的输入信号通常是经过预处理的雷达回波信号，如滤波去噪后的IQ（In-phase/Quadrature）数据 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[17](https://patents.google.com/patent/CN113298031A/zh)])，或通过时频分析转换为时频图像，尤其适用于高速机动目标检测 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。对于合成孔径雷达（SAR）系统，输入信号是SAR图像，包括振幅图像或结合散射中心特征 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **算法策略：** 主要采用基于深度学习的YOLO系列算法及其改进版本，包括改进的YOLOv3、YOLO-G（结合GhostNet和注意力块）、基于YOLOv5s的雷达运动目标识别等 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。这些算法通过优化网络结构（如扩展检测尺度、整合残差单元、引入轻量级骨干网络GhostNet）和损失函数（如DIOU损失函数和Focal loss），显著提升检测性能 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
*   **效果与准确率：** YOLO系列算法在雷达目标检测中展现出高效和实时性。例如，针对雷达运动目标多普勒频移特性的YOLOv5s模型能够实现运动目标检测和分类 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。改进的YOLOv3在多尺度目标检测中表现优于其他先进算法 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。YOLO-G模型通过注意力机制等改进，提高了军事目标检测精度，能够有效抑制干扰 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。然而，雷达YOLO算法仍面临小目标召回率低、复杂背景干扰、计算资源需求高和多目标密集场景下性能下降等挑战 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **相关数据集：** MSTAR（Moving and Stationary Target Acquisition and Recognition）数据集广泛用于SAR目标识别 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])；此外，研究者也会构建自定义的雷达移动目标数据集进行训练和评估 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **评估指标：** 目标检测中常用的平均精度（mAP）、精确率、召回率、F1值等 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。

### 2. 光学感知应用案例

光学感知利用视觉传感器、深度相机等获取光线信息，在需要丰富环境特征信息的场景中占据主导地位 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

#### 2.1 自动驾驶汽车检测

*   **应用场景：** 在自动驾驶中，光学感知用于实时监测车辆、行人、交通标志、交通灯等，为车辆决策提供关键的视觉信息 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)])。
*   **输入信号特性：** 主要输入为RGB图像或视频流。RGB图像提供密集的2D空间信息，通过像素位置和数值表达特征，但缺乏直接的深度信息 ([[16](https://patents.google.com/patent/CN113065590B/zh)])。视频流则提供连续的帧图像数据，需要进行预处理如去噪、增强、尺度调整 ([[18](https://patents.google.com/patent/CN117726687B/zh)])。
*   **算法策略：** YOLO系列算法（如YOLOv3、YOLOv7、YOLOv8及其各种改进版本）是主流选择 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[9](https://pdf.hanspub.org/csa_1543597.pdf)], [[11](https://www.opticsjournal.net/Articles/OJ8d249a888feac672/FullText)])。这些算法通过骨干网络优化（如Darknet-53, RepConv, CSPStackRep）、引入注意力机制（如坐标注意力、EMA模块）、改进多尺度特征融合（如FPN, PANet, SPPF）以及优化损失函数（如EIOU, SIoU, WIoU）和锚框策略（Anchor-Free），提升检测性能 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)], [[9](https://pdf.hanspub.org/csa_1543597.pdf)], [[10](https://s3plus.meituan.net/v1/mss_e63d09aec75b41879dcb3069234793ac/file/2022%E5%B9%B4%E7%BE%8E%E5%9B%A2%E6%8A%80%E6%9C%AF%E5%B9%B4%E8%B4%A7-%E5%90%88%E8%BE%91.pdf)], [[11](https://www.opticsjournal.net/Articles/OJ8d249a888feac672/FullText)])。
*   **效果与准确率：** YOLO系列算法以其高效和实时性，在自动驾驶车辆检测中实现了更快的速度和更高的精确度 ([[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)])。例如，YOLOv8模型在速度、精度和易用性之间实现了平衡，广泛应用于交通要素检测 ([[9](https://pdf.hanspub.org/csa_1543597.pdf)], [[11](https://www.opticsjournal.net/Articles/OJ8d249a888feac672/FullText)])。然而，光学视觉SLAM易受光照剧烈变化或纹理缺失区域影响，存在漂移问题和尺度不确定性 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。小目标召回率低、复杂背景干扰以及多目标密集场景下的性能下降仍是挑战 ([[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)])。
*   **相关数据集：** KITTI数据集是自动驾驶领域广泛使用的公开数据集，包含丰富的视觉数据，用于3D目标检测和轨迹评估 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)])。
*   **评估指标：** 主要使用mAP、精确率、召回率、F1值以及处理速度（FPS）等指标 ([[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)])。

#### 2.2 脑卒中患者上肢功能智能评估

*   **应用场景：** 利用非接触式传感器对脑卒中患者上肢功能进行客观、精准的评估，以取代传统的主观评估方式，缩短评估时间并提高结果一致性 ([[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)])。
*   **输入信号特性：** 该应用结合多种模态传感器：
    *   **深度传感器：** 提供深度图像（RGB-D图像），包含物体的三维空间信息，能够实时识别和重建物体表面 [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。对光照稳定性要求较高，主要适用于光照稳定的室内环境 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   **IMU（惯性测量单元）：** 提供运动姿态数据。
    *   **sEMG（表面肌电图）：** 采集肌肉电活动信号。
    *   **EEG（脑电图）：** 采集大脑电活动信号。
*   **算法策略：** 综合运用多种机器学习和深度学习算法，如多元线性回归、CNN、RNN、SVM、KNN、随机森林、模糊支持向量机等 ([[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)])。这些算法通过分析多模态信号数据，提取与患者上肢功能相关的特征，进行量化评估。
*   **效果与特点：** 这种智能评估系统能够克服传统评估的局限性，提供更为客观和精准的评估数据，大幅缩短评估时间，并增强评估结果的一致性 ([[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)])。
    <div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://pub.mdpi-res.com/sensors/sensors-23-08950/article_deploy/html/images/sensors-23-08950-g002.png?1699001081" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    The Role and Importance of Using Sensor-Based Devices in ...
  </div>
</div>

### 3. Wi-Fi感知应用案例

Wi-Fi感知利用现有的无线局域网基础设施，通过分析Wi-Fi信号特征来感知环境或定位设备，具有部署方便、成本低的优势 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

#### 3.1 室内定位

*   **应用场景：** 在商场、医院、机场等室内环境中，为人员或设备提供定位服务，实现导航、资产追踪或人流监测 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **输入信号特性：** 主要利用Wi-Fi信号特征，包括：
    *   **RSSI（信号强度指示器）：** Wi-Fi指纹定位通过预先采集不同位置的RSSI值建立指纹库，定位时匹配实时RSSI值 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   **TOF（信号飞行时间）：** 测距定位方法通过计算信号从发射到接收的时间来估算距离 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   本报告主要聚焦指纹定位，因其无需精确的信号源位置信息，且在复杂室内环境下不易受多径效应和非视距传播的显著影响，能够提供较稳定的定位服务 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **算法策略：** 主要包括指纹定位（如KNN、SVM、神经网络）和测距定位（如三角测量、多边定位），并常与其他传感器数据（如激光雷达、IMU）通过扩展卡尔曼滤波（EKF）等融合算法进行融合，以提升定位准确性和鲁棒性 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **准确率与挑战：** Wi-Fi信号定位虽然部署方便，但其精度相对有限，且易受多径效应（信号在传播过程中被反射、折射、散射导致路径复杂）影响，使得信号特征不稳定 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。在多传感器融合框架下，Wi-Fi可作为绝对位置参考，有助于校正其他传感器（如IMU）的累积漂移，但其自身的精度限制仍需通过融合来弥补 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。

### 4. 声学感知应用案例

声学感知利用声波进行信息获取，通过麦克风等设备采集声学信号，适用于多种感知任务 ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)])。

#### 4.1 生理感知

*   **应用场景：** 利用麦克风等通用设备，非接触式地监测人体生理信号，如呼吸、心跳、打鼾，甚至用于用户认证 ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)]).
*   **输入信号特性：** 主要为麦克风采集的声学信号，这些信号可能包含人体的微弱生理声音，也可能伴随环境噪声 ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)])。
*   **算法策略：** 通常涉及信号预处理（如滤波、降噪），然后通过特征提取（如频谱分析、梅尔频率倒谱系数MFCC）结合机器学习或深度学习算法（如CNN、RNN、SVM）进行分类或模式识别 ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)])。
*   **效果与特点：** 麦克风作为低成本的通用设备，为多种非接触式生理感知应用提供了便利。然而，声学感知易受环境噪声干扰，信号处理复杂性较高 ([[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)]).

### 5. 多传感器融合应用案例

多传感器融合是提升系统整体性能的关键，通过结合不同传感器的优势来克服单一模态的局限性，显著增强系统的鲁棒性、准确性和适用范围 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。

#### 5.1 机器人室内定位和导航 (雷达/LiDAR-深度相机-Wi-Fi-IMU融合)

*   **应用场景：** 机器人需要在复杂的室内环境中进行高精度定位和自主导航，应对障碍物遮挡、动态环境和数据频率/精度差异等挑战。
*   **输入信号特性：**
    *   **LiDAR（激光雷达）：** 提供高精度、高密度的点云数据，包含环境的几何信息，不受光照条件影响 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
    *   **深度相机：** 提供RGB-D图像，包含深度信息，显著提升SLAM精度 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   **Wi-Fi：** 提供位置参考，利用RSSI或TOF数据 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    *   **IMU（惯性测量单元）：** 提供线加速度和角速度信息，短时精度高，更新频率快 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
*   **算法策略：** 通常采用改进的PL-ICP（Point-to-Line Iterative Closest Point）算法处理激光雷达点云配准，引入特征点约束和自适应权重策略以提升遮挡场景下的点云匹配精度和速度 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。改进的Otsu算法用于增强深度图像特征提取能力 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。核心融合算法常采用扩展卡尔曼滤波（EKF）自适应加权融合点云、图像和Wi-Fi定位数据 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
*   **效果与准确率：** 该融合系统有效解决了室内障碍物遮挡、数据频率和精度差异以及动态环境鲁棒性问题 ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。EKF融合算法的定位精度显著优于单一PL-ICP方法和传感器SLAM方法，即使在初始角度偏差达45°时，仍能保持99.7%以上的定位精度小于0.001m ([[2](https://pdf.hanspub.org/sea_2691136.pdf)])。
    <div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/sensors/sensors-24-00048/article_deploy/html/images/sensors-24-00048-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Multi-Sensor Fusion Simultaneous Localization Mapping Based ...
  </div>
</div>

#### 5.2 园区三维建图与自动驾驶定位 (LiDAR-IMU融合)

*   **应用场景：** 在自动驾驶和机器人导航中，需要构建高精度、全局一致的园区三维地图，并实现精准定位。
*   **输入信号特性：**
    *   **LiDAR：** 提供高精度、高密度的三维点云数据，用于环境建模。
    *   **IMU：** 提供高频的运动数据，用于预积分和畸变矫正，克服激光雷达数据在高速运动时的畸变 ([[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)])。
*   **算法策略：** 采用紧耦合（tight coupling）的融合策略，即LiDAR和IMU数据在优化后端共同参与位姿估计。IMU预积分用于去除激光雷达点云畸变，而激光雷达里程计则用于消除IMU累积误差 ([[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)])。后端图优化中，增加回环检测因子、激光雷达里程计因子和IMU预积分因子，提升定位建图的全局一致性。例如，Fast-LIO 2引入Incremental Voxels (iVox) 增强增量式地图维护速度，并采用ICP回环检测消除累积误差 ([[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)])。
*   **效果与准确率：** LiDAR-IMU紧耦合融合系统能够显著提升位姿估计精度和地图构建精度，有效消除IMU的积分漂移和累积误差 ([[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。例如，在KITTI 07数据集上的评估显示，改进算法的绝对姿态误差显著降低，最大误差从10.36m降至1.46m，平均误差从1.97m降至0.60m ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。地图构建效果更精确，道路旁房屋建筑识别更精细，地图元素更丰富 ([[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)])。
    <div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/electronics/electronics-13-04717/article_deploy/html/images/electronics-13-04717-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    A Multi-Sensor Fusion Autonomous Driving Localization System ...
  </div>
</div>

#### 5.3 室内同步定位与建图及自主导航 (单线2D-LiDAR-IMU融合)

*   **应用场景：** 小型机器人或移动平台在室内环境中进行同步定位与建图（SLAM）和自主导航，要求低成本和高效率。
*   **输入信号特性：**
    *   **单线2D-LiDAR：** 提供平面内的距离信息，成本较低。
    *   **IMU：** 提供机器人的姿态和运动信息，用于校正2D激光雷达数据的畸变 ([[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)])。
*   **算法策略：** 通过IMU对2D激光雷达数据进行畸变矫正，然后结合GMapping算法（基于Rao-Blackwellized粒子滤波）进行同步定位与建图 ([[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)])。Dijkstra算法用于路径规划以实现自主导航和避障 ([[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)])。
*   **效果与特点：** 该系统能快速获取环境信息，具有良好的建图性能和低时延的自主导航与避障能力 ([[4](https://pdf.hanspub.org/csa2024145_81543242.pdf)])。

#### 5.4 输电线路智能预警评估 (机载LiDAR-光学影像)

*   **应用场景：** 对输电线路进行智能化巡检和预警评估，以确保电力系统安全运行。
*   **输入信号特性：**
    *   **机载LiDAR扫描系统：** 获取高精度的三维点云数据，用于线路及周围环境的建模。
    *   **光学影像：** 提供视觉信息，辅助识别线路组件和环境特征。
*   **算法策略：** 主要涉及三维建模、点云数据分析与判断技术 ([[5](https://patents.google.com/patent/CN105244805A/zh)])。通过对LiDAR点云和光学影像进行融合处理，重建输电线路及其周边环境的三维模型，进而进行数据分析与隐患识别。
*   **效果与特点：** 实现输电线路的快速高精度三维量测和空间分析，可用于弧垂计算、风偏校核、隐患分析等，大幅提升输电线路的安全预警能力和运维效率 ([[5](https://patents.google.com/patent/CN105244805A/zh)])。

### 总结与评估

非接触式感知应用案例表明，通过多样化的传感器模态和先进的算法策略，可以有效地解决不同场景下的复杂感知问题。深度学习（特别是CNN、RNN、YOLO系列和Transformer）在特征学习和目标识别方面展现出强大能力，而多传感器融合（如LiDAR-IMU-视觉-Wi-Fi融合）则通过优势互补显著提升了系统的鲁棒性和精度，尤其在自动驾驶和机器人导航等关键应用中发挥了核心作用。

未来，随着传感器技术和算法的持续演进，非接触式感知将在更多领域实现突破，并朝着更轻量化、更鲁棒、更智能的方向发展。对大数据集、弱监督/无监督学习以及更高级别融合策略的探索，将进一步推动非接触式感知技术的广泛应用。
# 总结与展望

非接触式感知技术作为连接物理世界与数字信息的重要桥梁，通过融合雷达、Wi-Fi、光学、声学等多种传感器模态，并结合先进的机器学习与深度学习算法，已在克服传统感知方法局限性方面取得了显著进展。本报告对非接触式感知领域当前最佳的算法策略进行了深入探讨，并评估了其输入信号特性、准确率、所使用的权威数据集及关键评估指标。

## 关键发现与进展总结

### 1. 多模态感知的协同优势
当前非接触式感知领域主要利用雷达、Wi-Fi、光学和声学等多种模态。每种模态各具优势，也面临特定挑战：
*   **雷达感知**：具备穿透性强、不受光照影响的优点，在自动驾驶、军事侦察等领域表现出色，但复杂环境下的抗干扰和多目标识别仍具挑战 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
*   **Wi-Fi感知**：利用现有基础设施，部署成本低廉，适用于室内定位，但精度有限且易受多径效应影响 [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
*   **光学感知**：提供丰富的视觉信息，成本低，尤其深度相机能提供深度信息，但易受光照变化和纹理缺失影响，存在漂移问题 [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
*   **声学感知**：利用麦克风等通用设备，成本低廉，可用于生理信号监测，但易受噪声干扰 [[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)], [[7](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)]。

### 2. 先进算法策略的核心作用
机器学习和深度学习算法已成为非接触式感知领域的主流，极大提升了感知性能。
*   **传统机器学习算法**：如SVM、KNN在小规模数据和特定场景下表现良好，例如在雷达系统中用于小型空中目标识别 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。但其依赖手动特征工程，在处理大规模、高维数据时存在局限性 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
*   **深度学习算法**：以其自动特征学习能力和强大的泛化性，显著提升了感知性能。
    *   **卷积神经网络 (CNN)**：在雷达信号目标检测和图像处理中广泛应用，通过多尺度、残差网络、注意力机制等改进策略，提高了复杂环境下的识别准确性 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[8](https://www.opticsjournal.net/Articles/OJ5cbbc2792599d7da/FullText)]。
    *   **循环神经网络 (RNN) 和长短时记忆网络 (LSTM)**：擅长处理时序数据，被应用于雷达信号的时序特性分析、人体运动识别等 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
    *   **生成对抗网络 (GAN)**：通过数据生成增强模型泛化能力，解决了数据不足等问题，如SAR目标识别和GPR数据增强 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
    *   **YOLO系列算法**：因其高效、实时性强而在自动驾驶、雷达目标检测中表现突出，通过骨干网络、注意力机制、损失函数和无锚框等改进，持续提升检测速度和精度 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [source]1, [[9](https://pdf.hanspub.org/csa_1543597.pdf)]。
    *   **Transformer-based Models**：如DETR，通过全局上下文感知能力在小目标检测中展现潜力，但计算复杂度高、训练收敛慢 [[8](https://www.opticsjournal.net/Articles/OJ5cbbc2792599d7da/FullText)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://smartdev.com/wp-content/uploads/2025/02/67.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    AI and IoT in 2025: How Smart Integration Transforms ...
  </div>
</div>

### 3. 多传感器融合的必然趋势
多传感器融合技术是提升系统整体性能的关键，通过优势互补解决了单一传感器的局限性，特别是在复杂环境下的鲁棒性和精度。
*   **LiDAR-IMU融合**：通过紧耦合和后端图优化，显著抑制点云畸变，减少累积误差，提升定位和建图精度 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[3](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)]。
*   **LiDAR-视觉-IMU-Wi-Fi深度融合**：通过EKF、改进PL-ICP等算法，有效解决了室内障碍物遮挡、数据频率和精度差异以及动态环境鲁棒性问题，实现了高精度、高鲁棒性的室内定位和导航 [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://images-eureka.patsnap.com/patent_img/487b62ff-06b0-4898-9af3-1fa015c657dd/US20080215204A1-20080904-D00000.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Sensor fusion patented technology retrieval search results ...
  </div>
</div>

### 4. 主要感知模态、算法、输入信号与性能总结

下表总结了报告中涉及的雷达、Wi-Fi、光学和多传感器融合系统在非接触式感知领域的关键信息：

| 感知模态/系统 | 典型输入信号特性 | 核心算法策略 | 典型准确率/优势 (示例) | 挑战/局限 | 权威数据集 (示例) | 主要评估指标 |
|---|---|---|---|---|---|---|
| **雷达感知 (YOLO)** | 雷达回波信号 (时频图, SAR图像, IQ数据) [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[17](https://patents.google.com/patent/CN113298031A/zh)] | 改进YOLOv3/v5s/G, DenseNet+YOLOv3, 双波束SAR+YOLO [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)] | 实时性强，高速检测；通过优化可提升小目标和复杂背景下精度 (YOLO-G提高军事目标检测精度 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]) | 小目标召回率低；复杂背景干扰；计算资源需求高 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)] | MSTAR [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], RML 2018.01 [[17](https://patents.google.com/patent/CN113298031A/zh)] | 精度, 精确率, 召回率, F1-score, mAP [[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)] |
| **Wi-Fi CSI感知** | Wi-Fi信号特征 (RSSI, CSI) [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | 指纹定位, 测距定位 (基于RSSI/TOF), EKF融合 [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | 部署方便，成本低；与多传感器融合后可显著提升定位精度 [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | 精度有限；易受多径效应影响 [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | (报告中未直接提及CSI特定权威数据集) | 定位精度, 鲁棒性, 处理速度 [[2](https://pdf.hanspub.org/sea_2691136.pdf)] |
| **光学图像/视频 (深度学习)** | RGB图像, 热红外图像, SAR图像, RGB-D图像, 视频流 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[16](https://patents.google.com/patent/CN113065590B/zh)], [[18](https://patents.google.com/patent/CN117726687B/zh)] | CNN (VGG, ResNet, Faster R-CNN), RNN/LSTM, GAN, SIFT, 改进Otsu [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | 自动学习深层特征，显著提升目标检测识别性能 (VGG19热红外图像检测卓越 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]) | 梯度消失/过拟合；稳定性/泛化能力不足；光照敏感 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | FLIR热红外数据集 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)] | 精度, 精确率, 召回率, F1-score, mAP [[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)] |
| **多传感器融合 (LiDAR-IMU-视觉)** | LiDAR点云, IMU数据, RGB图像, 深度图像, GPS, Wi-Fi数据 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)] | EKF, 改进PL-ICP, PSO-BP改进UKF, 视觉+激光二级融合, 注意力机制融合 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)] | 定位精度高，鲁棒性强 (EKF融合精度优于单一方法；KITTI数据集轨迹误差显著降低 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)]) | 障碍物遮挡；不同传感器数据差异；动态环境鲁棒性待提升 [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)] | KITTI数据集 [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)], YAHBOOM ROSMASTER X3小车 (实验验证) [[2](https://pdf.hanspub.org/sea_2691136.pdf)] | 定位精度 (米, 弧度), 鲁棒性, 处理速度, 平均绝对姿态误差 (APE) [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)] |

### 5. 权威数据集与评估指标

为确保算法性能的公平比较与验证，领域内广泛采用以下权威数据集和评估指标：
*   **数据集**：
    *   **MSTAR数据集**：SAR图像目标识别的基准 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
    *   **KITTI数据集**：自动驾驶领域的核心数据集，包含激光雷达、相机等多模态数据，用于目标检测、跟踪、定位等任务 [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)], [[16](https://patents.google.com/patent/CN113065590B/zh)]。
    *   **RML 2018.01数据集**：信号调制识别的开源数据集 [[17](https://patents.google.com/patent/CN113298031A/zh)]。
*   **评估指标**：
    *   **定位任务**：定位精度、鲁棒性、处理速度、平均绝对姿态误差 (APE，包括RMSE、最大值等) [[2](https://pdf.hanspub.org/sea_2691136.pdf)], [[13](https://www.hanspub.org/journal/paperinformation?paperid=88032)]。
    *   **分类/检测任务**：精度 (Accuracy)、精确率 (Precision)、召回率 (Recall)、F1值、混淆矩阵、P-R曲线、ROC曲线、AUC、mAP (Mean Average Precision) [[22](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)]。

这些量化指标为算法的优劣提供了客观依据，并指导后续的模型优化。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/sensors/sensors-25-02794/article_deploy/html/images/sensors-25-02794-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    A Survey of the Multi-Sensor Fusion Object Detection Task in ...
  </div>
</div>

## 展望

非接触式感知技术未来将持续发展，以下几个方向将是研究的重点和潜在的突破口：

### 1. 算法优化与轻量化
未来的研究将侧重于进一步提升深度学习算法的鲁棒性、实时性，并提高其在复杂应用环境中的适应能力。这包括解决梯度消失、过拟合、模式崩溃等现有挑战 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。同时，为适应资源受限的环境（如无人机、边缘计算设备），轻量化算法的发展至关重要，需要在保证性能的前提下，降低模型的计算复杂度与内存占用 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)], [[9](https://pdf.hanspub.org/csa_1543597.pdf)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.semi.org/sites/semi.org/files/2023-06/SEMI_Smart_Manufacturing_Roadmap.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    AI-Driven Autonomous Factory of the Future | SEMI
  </div>
</div>

### 2. 多传感器数据深度融合
探索更高级别的多传感器数据融合策略是提升系统性能的关键。未来的融合算法将不仅仅停留在信息层面的简单融合，而是深入到特征层面、决策层面的深度融合，通过引入更智能的算法（如深度学习驱动的融合）来实现环路闭合约束，从而显著提升导航和定位的精度、密度与全局一致性 [[2](https://pdf.hanspub.org/sea_2691136.pdf)]。例如，在自动驾驶等高安全性要求场景中，融合技术将变得更加关键。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/remotesensing/remotesensing-15-02256/article_deploy/html/images/remotesensing-15-02256-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Multilevel Data and Decision Fusion Using Heterogeneous ...
  </div>
</div>

### 3. 数据集建设与弱监督/无监督学习
高质量、大规模、多样化且标注完善的数据集是深度学习模型性能提升的基石。未来需针对特定应用场景（尤其是小目标检测）构建更丰富的专用数据集 [source]1, [[8](https://www.opticsjournal.net/Articles/OJ5cbbc2792599d7da/FullText)]。同时，为减少对大量人工标注数据的依赖，研究弱监督或无监督学习方法将成为重要方向，例如利用生成对抗网络进行数据增强和半监督学习 [[0](https://pdf.hanspub.org/jisp2025142_42670408.pdf)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://pub.mdpi-res.com/applsci/applsci-13-07082/article_deploy/html/images/applsci-13-07082-g001.png?1686659731" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Re-Thinking Data Strategy and Integration for Artificial ...
  </div>
</div>

### 4. 通用性与鲁棒性提升
提升算法在不同场景下的通用性和应对极端条件（如恶劣天气、严重遮挡、强干扰）的鲁棒性是非接触式感知技术走向广泛应用的关键 [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)]。这要求算法不仅能在理想环境下工作，更要能在现实世界的复杂多变中保持稳定和准确的性能。

### 5. 人机交互的智能化
在医疗康复、智能家居等特定领域，未来将更注重设计更加完善和智能的人机交互界面。通过提供即时反馈、指导和鼓励，减少专业人员的参与度，使得非接触式感知系统能够更好地服务于用户，实现更自然、便捷的交互体验 [[6](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://images.prismic.io/intuzwebsite/Z4kDHpbqstJ99hzC_AISmartHome_ABuilder%27sGuidetoFuture-ProofProjects.png?auto=format,compress" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    AI Smart Home | Transforming Smart Home Automation | Intuz
  </div>
</div>

### 6. 结合前沿技术
将Transformer、领域自适应（Domain Adaptation）、强化学习等前沿技术与现有感知方法结合，有望解决更具挑战性的感知任务 [[1](https://pdf.hanspub.org/csa20231100000_79216452.pdf)]。例如，Transformer的全局注意力机制可用于捕捉更丰富的上下文信息；领域自适应可解决跨域数据差异问题；强化学习可用于优化感知策略和资源分配。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://media.springernature.com/full/springer-static/image/art%3A10.1038%2Fs41746-025-01471-y/MediaObjects/41746_2025_1471_Fig1_HTML.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Convergence of evolving artificial intelligence and machine ...
  </div>
</div>

综上所述，非接触式感知技术正处于快速发展阶段。通过持续的算法创新、传感器融合策略的深化、高质量数据集的构建以及与新兴技术的交叉融合，该领域有望在未来展现出更强大的潜力，并在更广泛的实际应用中发挥关键作用，推动智能自动化、人机交互等领域迈向新的高度。


# References

- [基于雷达信号目标检测的深度学习算法综述](https://pdf.hanspub.org/jisp2025142_42670408.pdf)
- [基于YOLO算法的自动驾驶汽车检测研究综述](https://pdf.hanspub.org/csa20231100000_79216452.pdf)
- [基于多传感器融合与改进算法的机器人室内定位方法](https://pdf.hanspub.org/sea_2691136.pdf)
- [激光雷达与惯性测量单元同步融合下的 园区三维建图](https://ope.lightpublishing.cn/rc-pub/front/front-article/download/49059272/lowqualitypdf/%E6%BF%80%E5%85%89%E9%9B%B7%E8%BE%BE%E4%B8%8E%E6%83%AF%E6%80%A7%E6%B5%8B%E9%87%8F%E5%8D%95%E5%85%83%E5%90%8C%E6%AD%A5%E8%9E%8D%E5%90%88%E4%B8%8B%E7%9A%84%E5%9B%AD%E5%8C%BA%E4%B8%89%E7%BB%B4%E5%BB%BA%E5%9B%BE.pdf)
- [一种基于激光雷达的同步定位建图与自主导航算法研究](https://pdf.hanspub.org/csa2024145_81543242.pdf)
- [一种基于激光雷达的输电线路智能预警评估方法和系统](https://patents.google.com/patent/CN105244805A/zh)
- [脑卒中患者上肢功能智能评估系统研究进展](https://pmc.ncbi.nlm.nih.gov/articles/PMC10950765/)
- [深度学习在生物医药领域中的应用](https://biomed-dl.bioinfo-assist.com/?page=398&pub_year=2024&pub_month=03)
- [基于深度学习的小目标检测技术研究进展(特邀)](https://www.opticsjournal.net/Articles/OJ5cbbc2792599d7da/FullText)
- [基于改进YOLOv8的交通标志检测算法研究](https://pdf.hanspub.org/csa_1543597.pdf)
- [](https://s3plus.meituan.net/v1/mss_e63d09aec75b41879dcb3069234793ac/file/2022%E5%B9%B4%E7%BE%8E%E5%9B%A2%E6%8A%80%E6%9C%AF%E5%B9%B4%E8%B4%A7-%E5%90%88%E8%BE%91.pdf)
- [基于YOLOv8s改进的自动驾驶目标检测](https://www.opticsjournal.net/Articles/OJ8d249a888feac672/FullText)
- [智能物联网低功耗感知综述](https://crad.ict.ac.cn/article/doi/10.7544/issn1000-1239.202440396?viewType=HTML)
- [基于多传感信息融合的移动机器人定位与环境感知技术](https://www.hanspub.org/journal/paperinformation?paperid=88032)
- [一种融合信号液压马达故障诊断方法及系统](https://patents.google.com/patent/CN117628005A/zh)
- [PowerPoint 演示文稿](https://aibook.ren/upload/2025%E5%B9%B4%E4%B8%AD%E5%9B%BDAI%20Agent%E8%A1%8C%E4%B8%9A%E7%A0%94%E7%A9%B6%E6%8A%A5%E5%91%8A.pdf)
- [一种基于注意力机制的视觉与激光雷达多模态数据融合方法](https://patents.google.com/patent/CN113065590B/zh)
- [一种考虑信号物理和时序特性的信号调制识别方法及应用](https://patents.google.com/patent/CN113298031A/zh)
- [一种融合实景三维与视频的视觉重定位方法](https://patents.google.com/patent/CN117726687B/zh)
- [基于数据分析的用户信用风险评估方法及系统](https://patents.google.com/patent/CN117557361B/zh)
- [一种基于时序遥感数据的作物单产及长势评估方法](https://patents.google.com/patent/CN114118679B/zh)
- [一种基于体检数据的癌症早期风险评估方法和系统](https://patents.google.com/patent/CN113393935A/zh)
- [评估指标 — PaddleEdu documentation](https://paddlepedia.readthedocs.io/en/latest/tutorials/deep_learning/metrics/evaluation_metric.html)
- [多灾种风险评估方法述评——基于5份国际权威报告的对比分析](https://www.progressingeography.com/CN/10.18306/dlkxjz.2023.01.016)
- [基于大数据技术的供应商企业风险评估方法及系统](https://patents.google.com/patent/CN118153964B/zh)
- [推荐系统中的准确性、新颖性和多样性的有效耦合与应用](https://jns.nju.edu.cn/CN/10.13232/j.cnki.jnju.2022.04.005)
- [化妆品安全评估新规合集](https://www.cirs-group.com/cn/cosmetics/hua-zhuang-pin-an-quan-ping-gu-xin-gui-he-ji)
