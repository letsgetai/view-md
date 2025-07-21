## 引言

在现代信息社会中，微电子技术作为其核心驱动力，不断推动着各行各业的创新发展。在精密复杂的芯片制造工艺中，薄膜沉积技术与光刻、刻蚀并列为三大核心步骤，扮演着至关重要的角色 [0-0], [0-1]。其主要功能是在晶圆表面精确地沉积各种薄膜材料，包括介电（绝缘）层和至关重要的金属（导电）层，并通过后续的图案化和刻蚀工艺，构建出复杂的三维器件结构 [0-0], [0-1], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。

随着摩尔定律的持续推进，半导体制造工艺正不断向更小的尺寸迈进，进入了所谓的“先进制程”时代，这通常指的是7纳米（7nm）及以下的技术节点，例如3纳米（3nm）FinFET工艺 [0-0], [0-1]。制程的不断微缩带来了前所未有的制造复杂性。举例而言，90nm CMOS工艺中所需的薄膜沉积工序约为40道，而在3nm FinFET工艺中则激增至超过100道 [0-0]。同时，薄膜材料的种类也从约6种增加到近20种，对薄膜颗粒的控制要求也从微米级提升到纳米级 [0-0]。这些日益严苛的要求对薄膜沉积设备提出了巨大的压力和新的挑战。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://substackcdn.com/image/fetch/$s_!mDA8!,f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F3583ad47-8989-4c84-8094-df2fccaf0799_2759x2163.jpeg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    The Relentless Pursuit of Moore's Law
  </div>
</div>

金属薄膜是先进集成电路中不可或缺的组成部分，它们构成了芯片内部的关键互连线、扩散阻挡层、电极以及栅极结构。先进芯片的性能、可靠性和良率在很大程度上取决于这些金属薄膜的质量，包括其厚度均匀性、附着力、致密性以及在高深宽比（HAR）结构中的台阶覆盖能力 [0-0], [0-1], [0-2]。为了满足这些严苛的需求，多种先进的薄膜沉积技术得到了开发和完善，包括物理气相沉积（PVD）、化学气相沉积（CVD）、电子束蒸发沉积（Electron Beam Evaporation Deposition）、原子层沉积（ALD）以及分子束外延（MBE）等。在当前的先进制程中，PVD、CVD和ALD设备因其在特定应用中的独特优势，在金属薄膜生长中扮演着尤为关键的角色 [0-0], [0-1], [0-2], [0-4]。随着芯片几何结构的不断精细化和三维化，对沉积精度和共形性的要求显著提升，这尤其推动了原子层沉积（ALD）等技术的快速发展和广泛应用，使其能够实现原子层级的精确控制和优异的保形性 [0-0], [0-1], [0-2], [0-4]。本研究将深入探讨这些主流薄膜沉积技术在当前先进制程芯片制造中金属薄膜生长的具体应用，以及选择它们的原因。
# 先进制程中主流金属薄膜沉积设备的应用现状

在微电子工艺中，薄膜沉积是半导体制造的三大核心步骤之一，负责介质层与金属层的生长 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。随着芯片制程不断向7纳米及以下（如3纳米FinFET工艺）发展，所需的薄膜沉积工序从早期的约40道增加到超过100道，涉及的薄膜材料种类也从6种增加到近20种，并且对薄膜颗粒的要求也从微米级提升到纳米级 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。这种复杂性和精密度的提升，对薄膜沉积技术提出了更高的要求，驱动了物理气相沉积（PVD）、化学气相沉积（CVD）和原子层沉积（ALD）等技术的快速发展和应用，使其成为先进制程中金属薄膜生长的核心技术 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)], [[4](https://manu56.magtech.com.cn/progchem/EN/lexeme/showArticleByLexeme.do?articleID=12954)]。

### 1. 物理气相沉积 (PVD) 在金属薄膜生长中的应用

PVD是一种通过物理方法将材料从源头蒸发或溅射到基底表面制备薄膜的技术，主要包括蒸发镀膜、溅射镀膜和离子镀等。PVD以其定向沉积的特性，特别适合沉积金属材料 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。在先进制程中，磁控溅射PVD因其卓越的沉积效率、大尺寸范围内的厚度控制和精确的成分控制等优势而占据主导地位 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://research.nus.edu.sg/research-facilities/files/2024/10/397.-Magnetron-Sputter-coater.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Magnetron Sputter Coater – Research Facilities
  </div>
</div>

在7nm及以下先进制程中，PVD设备主要应用于：

*   **金属互连层：** PVD广泛用于半导体制造中的金属互连层沉积，例如铝（Al）互连线的制备 [[2](https://amtdco.com/infodetail.aspx?PID=1093)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。对于先进工艺，PVD也被用于铜（Cu）互连的籽晶层沉积，为后续的电化学沉积铜提供晶种 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。北方华创的eVictor AX30 Al pad PVD系统已应用于Bond pad和Al interconnect工艺，并被应用于90-28nm制程产线，更先进制程正在加速验证 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。
*   **扩散阻挡层：** 在铜互连技术中，由于铜原子扩散速度快，易对器件造成“中毒”效应，因此必须在其周围沉积一层防扩散阻挡层。PVD设备被用于沉积铜互连的阻挡层和钨（W）栓塞的黏附层，如钽（Ta）、氮化钽（TaN）、钛（Ti）和氮化钛（TiN）薄膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。离子化PVD（Ionized-PVD）作为磁控溅射DCPVD的改进，能够通过控制金属离子的方向和能量，显著提高对高深宽比通孔和狭窄沟道的底部和侧壁覆盖能力 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
*   **金属硬掩膜：** PVD用于沉积金属硬掩膜，如氮化钛（TiN）硬掩膜，在IC制备流程的前段（FEOL）和后段工艺（BEOL）中发挥关键作用 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。北方华创的exiTin H630 TiN 金属硬掩膜PVD系统专门针对55-28nm制程的12寸晶圆制造，并已进入国际供应链体系 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。
*   **其他金属薄膜：** PVD技术可以沉积多种金属靶材，如钽（Ta）、铝（Al）、铜（Cu）、钛（Ti）等，以及TiN、TaN、AlN等金属化合物薄膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.appliedmaterials.com/content/dam/site/prod-tech/semi/img/axcela-pvd.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Axcela PVD
  </div>
</div>

尽管PVD设备复杂且昂贵，并需要高真空环境，但其在低温下沉积高质量薄膜、高附着力和均匀性等优点使其在半导体制造中，特别是在主干金属层和关键阻挡层的制备上，仍然是不可或缺的 [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。

### 2. 化学气相沉积 (CVD) 在金属薄膜生长中的应用

CVD技术通过化学气相反应在硅片衬底上沉积薄膜材料，种类繁多，通常具有较好的沉积覆盖性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。在先进制程中，CVD在特定金属薄膜领域也有关键应用。

*   **钨（W）填充：** 在先进逻辑芯片的接触孔填充和3D NAND中的字线及插塞结构中，钨（W）被广泛用作导电材料。早期的金属CVD（MCVD）曾是钨填充接触孔和存储器字线的主流选择，对于较厚的金属薄膜沉积仍有优势。然而，在14nm及以后的先进制程中，由于对高深宽比结构填充能力和薄膜质量的更高要求，原子层沉积（ALD）技术正逐渐取代CVD，尽管ALD效率相对较低 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。中微公司的LPCVD设备已用于先进逻辑器件的钨（W）CVD接触孔填充，以及64层和128层3D NAND中的多个关键应用，目前处于客户端验证阶段 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/micromachines/micromachines-15-00441/article_deploy/html/images/micromachines-15-00441-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Fabrication of Tungsten Oxide Nanowalls through HFCVD for ...
  </div>
</div>

*   **低压化学气相沉积 (LPCVD)：** LPCVD通过在低压环境下精确调控化学反应，能够制备出高质量、均匀的薄膜。在金属薄膜相关的应用中，如上述的钨（W）CVD填充。此外，国产LPCVD设备在氮化硅等介质层沉积方面也有进展，间接支持了整体芯片结构中的金属层集成 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。
*   **等离子体增强化学气相沉积 (PECVD)：** PECVD借助等离子体在相对较低的反应温度下形成高密度、高性能的薄膜，通常用于含有金属或其他对温度敏感的结构上生长薄膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。尽管PECVD主要用于沉积介质绝缘层和半导体材料，但其低温沉积的优势也可能间接支持金属层间的介质填充，例如沉积Low-K材料、硬掩膜等，这些介质层对于稳定金属互连至关重要 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。

CVD技术因其良好的台阶覆盖性和生产效率，在全球薄膜沉积设备市场中占据重要份额，尤其在介质层和部分金属层的沉积中发挥着不可替代的作用 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。

### 3. 原子层沉积 (ALD) 在金属薄膜生长中的应用 (7nm及以下)

ALD是一种基于自限性表面反应的薄膜沉积技术，其核心优势在于能够实现原子层级精确控制薄膜厚度（0.07-0.1nm）、组分和结构 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。这赋予了ALD优异的均匀性、致密性、无孔洞以及在高深宽比结构中的保形性（阶梯覆盖能力强）等特点 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。这些特性使其在半导体先进制程（如7nm及以下），特别是在复杂形貌和高深宽比沟槽表面的薄膜沉积方面，具有显著优势 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-09-02388/article_deploy/html/images/applsci-09-02388-g001.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Atomic Layer Deposition (ALD) of Metal Gates for CMOS
  </div>
</div>

在7nm及以下先进制程中，ALD技术在金属薄膜及相关应用中的具体体现：

*   **High-K栅介质层与金属栅（Metal Gate）：** 在45nm甚至28nm以下制程中，传统SiO2栅介质层因厚度缩小会导致量子隧穿效应和漏电流问题。为了解决这一问题，引入了High-K介电材料（如Al2O3、HfO2、TiO2、ZrO2、Ta2O5），其厚度通常小于10nm [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。ALD是制备这些超薄High-K介质的理想技术。同时，High-K材料与传统多晶硅栅极兼容性不佳，需要用金属栅（Metal Gate）替代。由于金属栅极需要沉积在多晶硅沟槽内部或复杂的FinFET结构中，对台阶覆盖率要求极高，ALD（特别是等离子体增强原子层沉积PEALD）是生长金属纳米薄膜（如TiN、TaN、W等）以形成金属栅的理想技术 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [source]1, [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。微导纳米的TALD产品已在逻辑芯片High-K栅介质层领域实现产业化应用 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.mdpi.com/applsci/applsci-07-01047/article_deploy/html/images/applsci-07-01047-g002.png" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    The Challenges of Advanced CMOS Process from 2D to 3D
  </div>
</div>

*   **铜互连扩散阻挡层：** 铜（Cu）因其优异的导电性在250nm及以下制程中广泛应用于互连技术。然而，铜扩散速度快，易使器件“中毒”，因此在镀铜前必须沉积防扩散阻挡层 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。ALD技术能够在深宽比超过100:1的沟槽中仍能沉积具有良好保形性、均匀性和防扩散特性的超薄阻挡层（如TiN、TaN），这是ALD在先进互连中的关键应用 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。
*   **钨（W）ALD及氮化钛（TiN）ALD：** 随着结构尺寸的进一步缩小，ALD在金属填充方面的优势愈发突出。中微公司正在研发ALD钨设备，可用于高端存储芯片，其氮化钛（TiN）ALD设备也进入实验室和测试阶段，以满足更高深宽比结构的材料填充需求 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
*   **微型电容器：** 在DRAM等存储器中，随着存储容量增大，单个电容器尺寸持续减小，沟槽深宽比增加，ALD技术凭借其膜厚精确控制、大面积均匀性和高台阶覆盖率，能够很好地满足这些高深宽比电容介质层（如Al2O3）的沉积要求 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。

ALD技术能够满足28nm以下甚至7nm以下工艺中对更薄膜层和更复杂3D立体结构表面均匀镀膜的需求，未来在薄膜沉积环节的市场占有率将持续提高 [source]1。

### 4. 先进制程中主流金属薄膜沉积设备的应用总结

下表总结了物理气相沉积（PVD）、化学气相沉积（CVD）和原子层沉积（ALD）这三类主流设备在先进制程芯片制造中金属薄膜生长的具体应用：

| 沉积技术 | 主要沉积金属/化合物薄膜种类 | 典型应用及在芯片结构中的功能和位置 | 为什么选择它们？（优势） |
| :------- | :-------------------------- | :--------------------------------- | :----------------------------------------------- |
| **PVD**  | 铝（Al）、铜（Cu）籽晶层、钛（Ti）、氮化钛（TiN）、钽（Ta）、氮化钽（TaN）、铝氮化物（AlN）等 | **金属互连层：** Al互连线；Cu互连的籽晶层。<br>**扩散阻挡层：** Cu互连的Ta/TaN阻挡层，W栓塞的Ti/TiN黏附层。<br>**金属硬掩膜：** TiN硬掩膜（FEOL/BEOL）。 | 高沉积效率、精确成分控制、膜层致密、高附着力、均匀性好；离子化PVD改善高深宽比覆盖能力 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。 |
| **CVD**  | 钨（W）、氮化硅（SiN）等（在金属层间介质填充或作为硬掩膜） | **钨（W）填充：** 接触孔、3D NAND字线和插塞填充（尤其对较厚薄膜）。<br>**介质层与硬掩膜：** PECVD沉积Low-K介质层或硬掩膜，间接支持金属层间的隔离和结构形成 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。 | 良好的台阶覆盖性（特定CVD）、生产效率较高、适应性强；可用于复杂结构填充（相对PVD） [source]0。 |
| **ALD**  | High-K介电材料（Al2O3、HfO2、TiO2等）、金属栅极（TiN、TaN、W）、铜（Cu）互连阻挡层（TiN、TaN）、钨（W） | **High-K栅介质层与金属栅：** 45nm及以下制程中的High-K介电材料（超薄、高K值），以及与High-K兼容的金属栅极材料（高保形性） [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。<br>**铜互连扩散阻挡层：** 用于深宽比极高的沟槽中，防止Cu扩散 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。<br>**高深宽比结构填充：** W ALD、TiN ALD用于高端存储芯片和逻辑芯片中复杂高深宽比结构的填充 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。 | 原子层级膜厚控制、优异的均匀性、极高的保形性和致密性（无针孔）、低温沉积；是7nm及以下先进制程中实现超薄膜和复杂三维结构填充的关键技术 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。 |

总体而言，在7nm及以下先进制程的金属薄膜生长中，PVD继续在各类金属层和硬掩膜沉积中发挥重要作用，并不断提升其在深宽比结构中的沉积能力。CVD（特别是LPCVD）在特定金属（如钨）的填充方面仍有应用，而ALD技术则因其原子级精确控制、高保形性和高深宽比填充能力而日益重要，尤其是在High-K/金属栅、铜扩散阻挡层等关键应用中不可替代。这三类技术协同作用，共同满足了先进制程对金属薄膜越来越严苛的要求 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。
# 先进制程选择PVD、CVD和ALD进行金属薄膜生长的原因

在微电子制造，特别是7nm及以下等先进制程中，薄膜沉积是与光刻、刻蚀并列的三大核心工艺之一。随着芯片制程的不断缩小，对薄膜的厚度控制、均匀性、致密性、阶梯覆盖率、纯度、电阻率以及应力等性能提出了前所未有的高要求。同时，芯片结构的日益复杂化（如FinFET、Gate-All-Around纳米线/片等三维结构）以及新型材料的应用（如High-K介电材料、金属栅等），使得对沉积工艺的温度预算、对下层结构的损伤控制、与各种材料的兼容性等工艺要求也更加严苛 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[8](https://pdf.dfcfw.com/pdf/H3_AP202310111601216108_1.pdf)]。

在此背景下，物理气相沉积（PVD）、化学气相沉积（CVD）和原子层沉积（ALD）凭借其独特的优势和不断进步的技术，成为先进制程中金属薄膜生长的首选设备。而电子束蒸发和分子束外延设备则因其固有的技术局限性，在主流金属薄膜沉积中未被广泛采用。

### 1. 物理气相沉积 (PVD)

PVD是一种利用物理方法将材料从源头蒸发或溅射到基底表面形成薄膜的技术，主要包括磁控溅射PVD。其在先进制程中被广泛选择用于金属薄膜生长，主要原因在于其优异的薄膜性能和工艺优势，尤其适合定向沉积金属材料 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。

*   **薄膜性能：**
    *   **致密性和高附着力：** PVD薄膜通常具有良好的致密性和优异的附着力，这对于后续工艺的稳定性和器件的可靠性至关重要 [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。
    *   **均匀性和成分控制：** 磁控溅射PVD能够实现大尺寸晶圆上的沉积厚度控制和精确的成分控制，确保薄膜在整个晶圆上的均匀性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
    *   **电阻率和纯度：** 能够沉积高纯度的金属薄膜，有助于保持较低的电阻率，满足高性能互连的需求 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
    *   **应力控制：** 通过优化工艺参数，PVD能够制备具有可控应力的薄膜，减少对器件结构的潜在损伤。
*   **工艺兼容性：**
    *   **低温沉积：** PVD可在相对较低的温度下进行薄膜沉积 [[2](https://amtdco.com/infodetail.aspx?PID=1093)]，这对于避免损伤已形成的热敏下层结构至关重要，符合先进制程的低热预算要求。
    *   **损伤控制：** 尽管存在离子轰击，但现代PVD技术（如离子化PVD）能够控制金属离子的方向和能量，在一定程度上减少对基底的损伤，并提高对高深宽比结构的底部覆盖能力 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
    *   **高真空环境：** 在高真空环境下进行，有助于减少薄膜中的杂质含量，提高纯度 [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.appliedmaterials.com/content/dam/site/prod-tech/semi/img/axcela-pvd.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Metals Deposition
  </div>
</div>
*图1. 现代PVD沉积系统，展示其用于金属沉积的能力。*

*   **满足新型材料需求：**
    *   **金属互连层：** PVD是沉积铝（Al）互连的关键技术 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)], [source]5。
    *   **扩散阻挡层和籽晶层：** 在铜（Cu）互连工艺中，PVD用于沉积钽（Ta）、氮化钽（TaN）等作为铜的扩散阻挡层以及铜籽晶层，防止铜原子扩散到硅衬底，同时为后续电镀铜提供生长基础 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。离子化PVD尤其适用于高深宽比通孔和狭窄沟道的底部覆盖 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
    *   **金属硬掩膜：** PVD广泛应用于沉积氮化钛（TiN）等金属硬掩膜，在刻蚀过程中保护下层结构 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。
    *   **其他金属薄膜：** 能够沉积包括钽（Ta）、铝（Al）、铜（Cu）、钛（Ti）等多种金属以及TiN、TaN、AlN等金属化合物薄膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。

### 2. 化学气相沉积 (CVD)

CVD技术通过化学气相反应在衬底表面沉积薄膜材料，其在先进制程中主要凭借其优异的阶梯覆盖率和填充能力在特定金属薄膜生长中占据一席之地 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。

*   **薄膜性能：**
    *   **良好均匀性：** CVD能够实现良好的薄膜厚度均匀性。
    *   **优异的阶梯覆盖性：** CVD（特别是低压化学气相沉积LPCVD）的沉积覆盖性较好，能够有效地填充深孔和高深宽比结构 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。对于较厚的金属薄膜沉积，CVD仍是重要的选择。
    *   **可控电阻率和纯度：** 通过精确控制反应气体组分和工艺参数，可以制备满足要求的金属薄膜。
*   **工艺兼容性：**
    *   **温度敏感性与损伤控制：** 尽管传统热CVD温度较高，但LPCVD和等离子体增强化学气相沉积（PECVD）能在相对较低的温度下进行。PECVD通过等离子体活化前驱体，在更低的反应温度下形成高性能薄膜，这对于含有金属或其他对温度敏感的结构尤为重要，有助于控制对下层结构的损伤 [source]0。
    *   **满足填充要求：** CVD技术，特别是针对高深宽比结构的填充，能够实现良好的孔洞填充，减少空隙和缺陷。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://wevolver-project-images.s3.us-west-1.amazonaws.com/0.8mioxuyz35bUntitleddesign.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    PVD vs CVD: Mastering Advanced Thin Film Deposition Techniques
  </div>
</div>
*图2. PVD与CVD工艺对比图，展示其基本原理差异。*

*   **满足新型材料需求：**
    *   **钨（W）填充：** CVD在钨（W）金属薄膜的填充中扮演着关键角色，尤其是在高深宽比的接触孔和存储器字线填充方面。例如，中微公司的LPCVD设备已用于先进逻辑器件的钨CVD接触孔填充，以及3D NAND中的字线沉积 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
    *   **硬掩膜与介质层：** 虽然PECVD主要用于沉积介质绝缘层，但其低温优势也使其能够用于沉积某些金属层间的介质，或作为硬掩膜支持金属层刻蚀。

### 3. 原子层沉积 (ALD)

ALD是一种基于自限性表面反应的薄膜沉积技术，因其原子层级的精确控制能力和优异的保形性，在7nm及以下先进制程中，特别是处理复杂形貌和高深宽比沟槽表面时，表现出显著优势，并日益变得不可或缺 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。

*   **薄膜性能：**
    *   **原子层级膜厚控制：** ALD能够实现0.07-0.1nm的原子层级精确厚度控制 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]，这对于制备超薄膜（如High-K介质层和金属栅）至关重要。
    *   **卓越的均匀性和三维共形性：** ALD的最大优势之一是其优异的均匀性和高保形性（阶梯覆盖能力强），即使在深宽比超过100:1的复杂三维结构中，也能实现均匀、致密的薄膜沉积，无孔洞，保证了器件性能的一致性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。这对于FinFET、3D NAND等先进结构尤为关键。
    *   **致密性和低缺陷率：** ALD薄膜通常非常致密、无针孔，有效降低了缺陷率，从而提高了器件的可靠性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [source]1。
    *   **纯度与电阻率：** 能够沉积高纯度的金属和金属化合物薄膜，确保所需的电学性能。
    *   **低应力：** ALD薄膜的应力通常较低，对下层结构影响小。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://pub.mdpi-res.com/applsci/applsci-09-02388/article_deploy/html/images/applsci-09-02388-g001.png?1561092123" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Atomic Layer Deposition (ALD) of Metal Gates for CMOS
  </div>
</div>
*图3. ALD用于CMOS金属栅沉积的示意图，展示其在高深宽比结构中的填充能力。*

*   **工艺兼容性：**
    *   **低温沉积：** ALD可以在相对较低的温度下进行沉积 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [source]1，这大大降低了热预算，避免了对已集成器件的热损伤，对于多层互连和敏感材料尤其重要。
    *   **损伤控制：** 与PVD的物理轰击和部分CVD的等离子体损伤相比，热ALD通过自限性化学反应进行，对下层结构几乎没有损伤，保证了界面的高质量。
*   **满足新型材料需求：**
    *   **High-K栅介质层与金属栅：** 在45nm甚至更小制程中，ALD是制备超薄High-K介电材料（如Al2O3、HfO2等）的理想技术。同时，ALD（特别是PEALD）是生长金属栅（如TiN、TaN等）纳米薄膜的理想技术，因为金属栅沉积在复杂沟槽内部，对台阶覆盖率要求极高 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [source]1, [source]5。
    *   **铜互连扩散阻挡层：** 由于铜的快速扩散特性，ALD技术被用于沉积超薄、高保形且有效的防扩散阻挡层（如TiN、TaN），即使在深宽比超过100:1的沟槽中也能表现出色，是先进互连中的关键应用 [source]1。
    *   **钨（W）ALD和氮化钛（TiN）ALD：** 随着制程缩小，ALD钨正逐渐取代MCVD用于填充接触孔和存储器字线，中微公司等正在研发相关设备。ALD氮化钛也正满足更高深宽比结构的材料填充需求 [source]0。
    *   **微型电容器：** 在DRAM等存储器中，ALD凭借其膜厚精确控制、大面积均匀性和高台阶覆盖率，满足了微型电容器高深宽比沟槽的填充要求 [source]1。

### 4. 电子束蒸发和分子束外延设备未广泛采用的原因

尽管电子束蒸发（E-beam Evaporation）和分子束外延（MBE）在特定领域有其应用，但在先进制程芯片的通用金属薄膜生长中并未被广泛采用，主要原因在于它们难以满足现代芯片工艺对薄膜性能、工艺兼容性和生产效率的严苛要求 [[9](https://zhuanlan.zhihu.com/p/671632123)]。

*   **电子束蒸发设备：**
    *   **薄膜性能局限：** 电子束蒸发是一种指向性沉积方法，在ULSI工艺中，尤其是在制造复杂的通孔、接触孔等高深宽比结构时，其台阶覆盖率极差，无法有效地实现孔内的金属均匀覆盖和填充 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [source]9, [source]10。它一般只适用于平面的膜层制备，与先进芯片的复杂三维结构需求不符 [source]9。
    *   **工艺兼容性问题：** 高能离子的轰击会引起衬底损伤 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]，这在对器件完整性要求极高的先进制程中是不可接受的，可能影响器件性能和良率。
    *   **应用局限：** 目前主要应用于LED的电极制作等特定场景 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]，而非主流芯片金属互连。

*   **分子束外延（MBE）设备：**
    *   **主要用途差异：** MBE主要用于生长高质量的单晶半导体薄膜（如硅、SiGe、GaAs等），以形成具有特定晶体结构和电学性能的半导体层 [source]10。它并非主流的通用金属薄膜（如互连线、阻挡层）沉积方法，因为这些金属层通常不需要单晶结构，并且对沉积速率和成本有更高的要求。
    *   **高成本和低效率：** MBE作为一种高度精确的单原子层级生长技术，通常伴随着极高的设备成本和较慢的沉积速率 [source]4。对于需要大规模、快速沉积的多晶金属薄膜，MBE的效率远低于磁控溅射PVD和部分CVD方法。
    *   **复杂性和操作难度：** MBE对真空环境、温度控制和材料纯度有极其严苛的要求，设备和操作复杂，不适合大规模工业化生产中对通用金属层的需求。

### 5. 总结比较

下表对比了PVD、CVD和ALD在先进制程金属薄膜生长中的关键特性、优缺点及其在满足工艺要求方面的表现。

| 技术类型   | 典型应用金属/化合物       | 膜厚控制与均匀性             | 阶梯覆盖率与填充能力 | 热预算与损伤控制       | 主要优势                                                                   | 局限性                                     |
| :--------- | :------------------------ | :--------------------------- | :------------------- | :--------------------- | :------------------------------------------------------------------------- | :----------------------------------------- |
| **PVD**    | Al, Cu, Ta, Ti, TiN, TaN | 大尺寸晶圆上良好厚度控制和均匀性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)] | 相对较差（定向沉积） [source]0 | 低温，高真空 [[2](https://amtdco.com/infodetail.aspx?PID=1093)] | 沉积效率高，大尺寸适用；精确成分控制；薄膜致密，附着力好 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)] | 复杂高深宽比结构覆盖性差；设备昂贵 [[2](https://amtdco.com/infodetail.aspx?PID=1093)] |
| **CVD**    | W, TiN                    | 良好均匀性                   | 优异（可填充深孔） [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)] | 可调（LPCVD/PECVD较低） [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)] | 良好阶梯覆盖和填充能力；可大批量生产；化学反应多样 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]             | 部分工艺温度高；前驱体选择；可能产生颗粒 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)] |
| **ALD**    | TiN, TaN, W, Al2O3, HfO2 | 原子层级精确控制，极高均匀性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)] | 卓越（高保形性，无针孔） [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)] | 低温，无损伤或极低损伤 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)] | 原子层级控制；超高保形性；致密无针孔；适用于极高深宽比结构和热敏感材料 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)] | 沉积速率慢；前驱体选择少；设备成本高 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)] |
| **电子束蒸发** | Al (LED电极)              | 膜厚精确控制                 | 极差（指向性） [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)] | 低温                   | 蒸发难熔金属；高纯度 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]                                         | 衬底损伤；无法填充高深宽比结构；适用于平面膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[9](https://zhuanlan.zhihu.com/p/671632123)], [[10](https://zhuanlan.zhihu.com/p/521919587)] |
| **分子束外延** | Si, SiGe, GaAs (半导体)   | 原子层级控制，极高均匀性     | 通常不用于填充结构   | 低温，超高真空         | 高质量单晶生长；缺陷密度极低；精确控制组分 [[10](https://zhuanlan.zhihu.com/p/521919587)]                    | 成本极高；沉积速率极慢；主要用于半导体材料生长，非通用金属薄膜 |

综上所述，在当前先进制程的芯片工艺中，PVD、CVD和ALD设备的选择是基于它们在薄膜性能、工艺兼容性和满足新型材料需求方面的综合考量。PVD在各类金属层的快速沉积和硬掩膜中仍发挥核心作用，CVD则凭借其填充能力在钨等特定金属的生长中不可替代。而ALD技术，因其原子层级的精确控制、卓越的三维共形性和低温无损伤特性，正日益成为7nm及以下先进制程中High-K/金属栅、超薄扩散阻挡层及复杂高深宽比结构填充的必然选择，并主导着未来金属薄膜沉积技术的发展方向。
# 电子束蒸发设备和分子束外延设备在先进制程中的应用局限性

在微电子工艺中，金属薄膜的生长是半导体制造的关键步骤之一，与光刻和刻蚀并列为三大核心工序。随着芯片制程不断向7纳米及以下（如3纳米FinFET工艺）发展，所需的薄膜沉积工序从90纳米CMOS的约40道增加到超过100道，薄膜材料种类也从6种增加到近20种，对薄膜的厚度、精度、均匀性和台阶覆盖率提出了前所未有的高要求。在这一背景下，选择合适的薄膜沉积设备对于实现高性能、高良率的先进制程芯片至关重要。目前主流的金属薄膜沉积技术主要集中于物理气相沉积（PVD）、化学气相沉积（CVD）和原子层沉积（ALD）。本节将考察电子束蒸发设备和分子束外延设备在先进制程芯片金属薄膜生长中是否有特定的应用场景，并详细分析其为何在主流金属薄膜沉积中不被广泛采用，包括它们各自的技术局限性与主流技术相比的劣势。

### 电子束蒸发设备的应用及局限性

电子束蒸发（Electron Beam Evaporation, EBE）是一种物理气相沉积（PVD）技术，其基本原理是利用高能电子束作为加热源，将真空腔室内的固体靶材加热至蒸发或升华，然后蒸发的原子或分子凝结沉积到放置在腔室内的基底表面，形成薄膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://pub.mdpi-res.com/coatings/coatings-13-00505/article_deploy/html/images/coatings-13-00505-g003.png?1677251629" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Thin Film Deposition Techniques in Surface Engineering ...
  </div>
</div>

**1. 应用方面：**
电子束蒸发能够产生极高的能量密度，因此可以蒸发一些熔点较高的金属或化合物，并制备出高纯度的薄膜。它还可以实现较快的沉积速率和对膜厚的精确控制 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[9](https://zhuanlan.zhihu.com/p/671632123)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。在超大规模集成电路（ULSI）的早期发展中，电子束蒸发曾被用于金属薄膜的沉积 [[9](https://zhuanlan.zhihu.com/p/671632123)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。然而，在当前的先进制程中，电子束蒸发设备的主要应用场景已转向特定领域，例如LED制造中的电极制备 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。

**2. 未广泛采用的原因及技术局限性：**
尽管电子束蒸发具有蒸发难熔金属和高纯度沉积的优点，但其在先进制程芯片的金属薄膜生长中并未被广泛采用，主要原因在于其固有的技术局限性，这些局限性与先进制程对薄膜的苛刻要求相悖：

*   **衬底损伤：** 电子束蒸发过程中，高能离子的轰击可能对敏感的衬底造成损伤 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。在器件结构日益微缩和精密的先进制程中，任何形式的衬底损伤都可能严重影响器件的性能和可靠性。
*   **台阶覆盖率差和深孔填充能力不足：** 电子束蒸发属于一种典型的指向性沉积方法 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。这意味着蒸发出的粒子沿着近似直线路径飞行并沉积。在先进制程芯片中，互连线、通孔和接触孔等结构具有极高的深宽比（如深宽比可达100:1），且形状日益复杂。电子束蒸发在这种高深宽比的沟槽和孔洞中无法实现良好的台阶覆盖，导致薄膜在侧壁和底部沉积不均匀，甚至形成空洞，无法满足后续工艺对填充完整性的要求 [[9](https://zhuanlan.zhihu.com/p/671632123)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。
*   **适用于平面膜制备的局限性：** 该方法通常更适用于平坦表面的薄膜制备 [[9](https://zhuanlan.zhihu.com/p/671632123)]。然而，先进制程芯片的结构已从二维平面向三维立体化发展，对薄膜在复杂三维结构上的共形性（Conformality）和填充能力提出了极高要求，这使得电子束蒸发难以胜任。

### 分子束外延设备的应用及局限性

分子束外延（Molecular Beam Epitaxy, MBE）是外延（Epitaxy, EPI）技术的一种。外延是指在单晶衬底上生长一层具有相同晶向的单晶薄膜材料 [[10](https://zhuanlan.zhihu.com/p/521919587)]。外延技术在半导体制造中主要用于在硅衬底上生长高纯度、低缺陷密度的单晶层，以改善器件的电学性能，例如在器件的源、漏和栅极区域沉积外延硅可以减小接触电阻，提高芯片运行速度 [[10](https://zhuanlan.zhihu.com/p/521919587)]。

<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://omo-oss-image.thefastimg.com/portal-saas/pg2024090313222616725/cms/image/40be4d3d-62d6-4382-8b0d-7f78dcba979.jpeg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    MBE Molecular Beam Epitaxy Equipment-Pengcheng Semiconductor ...
  </div>
</div>

**1. 应用方面：**
分子束外延技术能够实现原子层级的精确控制，生长出高质量的单晶半导体薄膜，如硅（Si）、硅锗（SiGe）、砷化镓（GaAs）和氮化镓（GaN）等。这些高质量的半导体层对于制造高性能的逻辑器件、射频器件、光电器件和量子器件至关重要。

**2. 未广泛采用的原因及技术局限性：**
尽管分子束外延在生长高质量单晶半导体薄膜方面具有独特优势，但它并非先进制程芯片中通用“金属薄膜生长”的主流选择，原因如下：

*   **主要用途差异：** 分子束外延的核心目的在于生长具有特定晶体结构的单晶半导体层，而非用于沉积构成互连线或阻挡层的多晶或非晶态金属薄膜。芯片中的金属互连层（如铜、铝）和阻挡层（如TiN、TaN）通常不需要单晶结构，它们的关键性能在于导电性、阻挡扩散能力和与介质层的兼容性。因此，分子束外延的优势并未体现在主流金属互连的需求上。
*   **高成本和低效率：** 分子束外延是一种对真空环境、温度控制和材料纯度要求极其苛刻的技术。其设备非常昂贵，且沉积速率相对较慢，难以满足大规模工业化生产中对通用金属薄膜的效率要求 [[4](https://manu56.magtech.com.cn/progchem/EN/lexeme/showArticleByLexeme.do?articleID=12954)]提及新兴技术昂贵且加工时间长。对于需要快速、大规模沉积的多晶金属薄膜，其生产效率远低于磁控溅射PVD和部分CVD方法。
*   **复杂性和操作难度：** 分子束外延设备和操作过程复杂，维护成本高昂。这使其在追求成本效益和高吞吐量的芯片制造中缺乏竞争力，尤其是在沉积非晶或多晶金属层时，其复杂性带来的收益不足以弥补其劣势。

### 主流薄膜沉积技术与电子束蒸发和分子束外延的对比

下表对比了电子束蒸发、分子束外延以及目前在先进制程中广泛使用的薄膜沉积技术在金属薄膜生长中的特点：

| 技术类型             | 沉积原理             | 主要应用材料          | 优点                                                                                     | 缺点/局限性                                                                                                   | 在先进制程中的主要作用/地位                                                                                        |
| :------------------- | :------------------- | :-------------------- | :--------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------- |
| **电子束蒸发 (EBE)** | 物理蒸发             | 金属                  | 高纯度、膜厚精确控制、可蒸发难熔金属                                                     | **高能离子轰击导致衬底损伤；台阶覆盖率差，无法有效填充高深宽比结构中的孔洞；主要适用于平面膜**                        | 仅限于特定领域（如LED电极），不适用于先进芯片复杂三维结构的金属互连和填充                                          |
| **分子束外延 (MBE)** | 单晶生长             | 半导体材料 (Si, SiGe, GaAs) | 单晶质量高、缺陷密度低、原子层级精确控制                                                 | **生产成本高、沉积速率慢、设备复杂；主要用于半导体层生长，不适用于主流金属薄膜**                                    | 用于高性能器件中的单晶半导体外延层生长，而非主流金属互连或阻挡层生长                                               |
| **磁控溅射PVD**      | 物理溅射             | 铜、铝、钛、钽、TiN、TaN | 膜层致密、结合力好、均匀性高、沉积效率高、大尺寸范围沉积厚度控制 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)] | 在极高深宽比结构中台阶覆盖能力相对ALD和部分CVD较弱                                                            | 主流金属薄膜沉积技术，广泛用于金属互连层、扩散阻挡层（如Ti/TiN、Ta/TaN）、硬掩膜（如TiN） [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)] |
| **化学气相沉积 (CVD)** | 化学气相反应         | 钨、介质材料          | 膜厚均匀性好、台阶覆盖性好（尤其是LPCVD/PECVD）、生产效率高                              | 工艺参数敏感；部分工艺（如PECVD）台阶覆盖率不如ALD                                                              | 用于钨（W）填充（尤其在存储器中），沉积介质层和硬掩膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]                                                |
| **原子层沉积 (ALD)**   | 原子层级自限性表面反应 | High-K介质、金属、TiN、TaN | 原子层级膜厚控制、优异的均匀性、致密性、高深宽比结构的超高保形性 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)] | 沉积速率慢、前驱体选择和工艺控制复杂、成本高 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]                                            | 先进制程的关键技术，用于High-K栅介质、金属栅、铜互连扩散阻挡层、高深宽比结构的填充 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]       |

综上所述，电子束蒸发设备和分子束外延设备虽然在各自的特定领域（如LED电极制备、单晶半导体材料生长）具有不可替代的优势，但由于其固有的技术局限性——电子束蒸发存在衬底损伤和差的台阶覆盖率问题，不适合复杂三维金属结构的填充；分子束外延则侧重于单晶半导体材料而非通用金属薄膜的生长，且成本高、效率低——使得它们在当前和未来的先进制程芯片“金属薄膜生长”这一主流应用中不被广泛采用。相反，磁控溅射PVD、CVD以及ALD技术凭借其在沉积效率、薄膜质量、特别是高深宽比结构填充和共形性方面的优势，占据了先进制程芯片金属薄膜沉积的主导地位。
# 结论

在当前先进制程芯片制造（7nm及以下）中，薄膜沉积技术作为半导体制造的三大核心步骤之一，其重要性日益凸显。随着芯片线宽的不断缩小，对薄膜的厚度、精度、均匀性和台阶覆盖率提出了前所未有的高要求。面对日益复杂的3D结构和更多层数的薄膜需求，多种金属薄膜生长设备被运用和优化，以满足这些严苛的工艺挑战。

目前，在先进制程芯片工艺中，金属薄膜的生长主要运用到物理气相沉积（PVD）、化学气相沉积（CVD）和原子层沉积（ALD）这三类设备。

### 1. 主流金属薄膜生长设备的运用与选择

#### 1.1 物理气相沉积 (PVD)
PVD是一种通过物理方法将材料从源头蒸发或溅射到基底表面制备薄膜的技术。在金属薄膜PVD中，磁控溅射PVD占据主导地位，因其具有极佳的沉积效率、大尺寸范围的沉积厚度控制和精确的成分控制等优势 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
*   **沉积金属薄膜：** PVD设备主要用于沉积**金属互连层**（如铝Al、铜Cu）、**扩散阻挡层**（如用于钨栓塞的黏附层以及铜互连的阻挡层和籽晶层，通常是TiN、TaN）、**金属硬掩膜**（如氮化钛TiN）以及其他**金属靶材**（如钽Ta、钛Ti）。 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]
*   **选择原因：** 尽管PVD设备复杂且昂贵，并需要高真空环境，但其在低温下沉积高质量薄膜、高附着力和均匀性等优点使其在半导体制造中不可或缺 [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。离子化PVD（Ionized-PVD）的出现进一步提升了对高深宽比通孔和狭窄沟道的台阶底部覆盖能力 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。

#### 1.2 化学气相沉积 (CVD)
CVD技术通过化学气相反应在硅片衬底上沉积薄膜材料，其沉积覆盖性较好，尤其适合沉积介质材料，但在特定金属薄膜领域也有重要应用。
*   **沉积金属薄膜：** 主要应用于**钨（W）填充**，尤其是在接触孔和存储器的字线填充中。低压化学气相沉积（LPCVD）在低压环境下精确调控化学反应，可用于制备高质量、均匀的钨薄膜 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。等离子体增强化学气相沉积（PECVD）通常用于含有金属或其他对温度敏感的结构上生长薄膜，其低温沉积的优势也可能间接支持金属层间的介质填充 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。
*   **选择原因：** CVD技术能够提供良好的膜层均匀性和台阶覆盖性，对于需要填充复杂三维结构的金属材料（如钨插塞）是有效的选择。PECVD通过等离子体辅助，可在较低温度下实现高质量薄膜沉积，减少对敏感结构的损伤 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://wevolver-project-images.s3.us-west-1.amazonaws.com/0.8mioxuyz35bUntitleddesign.jpg" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    PVD vs CVD comparison
  </div>
</div>

#### 1.3 原子层沉积 (ALD)
ALD是一种基于自限性表面反应的薄膜沉积技术，能够实现原子层级精确控制薄膜厚度、组分和结构，具有优异的均匀性、致密性、无孔洞以及高深宽比结构的保形性。这些优势使其在半导体先进制程（如7nm及以下）中具有显著优势 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[2](https://amtdco.com/infodetail.aspx?PID=1093)]。
*   **沉积金属薄膜：** 在7nm及以下先进制程中，ALD技术在**High-K栅介质层与金属栅**（如Al2O3、HfO2等High-K材料及金属栅薄膜）的制备中至关重要 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)], [[5](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)]。此外，ALD是沉积**铜互连扩散阻挡层**（如TiN、TaN）的关键技术，能够在深宽比超过100:1的沟槽中沉积保形薄膜 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。**钨（W）ALD**也正在研发中，以满足更高深宽比结构的材料填充需求 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)]。
*   **选择原因：** ALD能够满足28nm以下工艺中对更薄膜层和更3D立体结构表面均匀镀膜的需求，其原子层级的精确控制、优异的台阶覆盖能力和良好的膜质量，使其在多维复杂结构和超薄膜沉积方面几乎不可替代 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://www.atomiclayerdeposition.com/storage/app/2147/JMIDCXNgc9KdHTcW17H9k8QMixqsWtBzxEkoPAGHAM2PYlC6.webp" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Atomic Layer Deposition
  </div>
</div>

### 2. 电子束蒸发设备和分子束外延设备在先进制程芯片金属薄膜生长中未被广泛采用的原因

尽管存在多种薄膜沉积技术，但电子束蒸发设备和分子束外延设备在先进制程芯片的“通用”金属薄膜生长中并未得到广泛应用，主要原因在于其技术局限性和应用侧重点的不同。

#### 2.1 电子束蒸发设备 (Electron Beam Evaporation)
*   **应用及优点：** 电子束蒸发作为一种PVD技术，能够获得极高的能量密度，蒸发难熔金属或化合物，并制备高纯度薄膜，同时实现快速蒸发和精确控制膜厚 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[9](https://zhuanlan.zhihu.com/p/671632123)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。目前主要应用于LED的电极制作等特定领域 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。
*   **未广泛采用的原因：** 在先进制程芯片制造中，电子束蒸发存在以下局限：
    *   **衬底损伤：** 高能离子的轰击会引起衬底损伤，这在对器件完整性要求极高的先进工艺中是不可接受的 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。
    *   **台阶覆盖率差和无法填充深孔：** 电子束蒸发是一种指向性沉积方法，在ULSI工艺中，尤其是在制造复杂的通孔、接触孔等高深宽比结构时，其无法有效实现孔内的金属覆盖，难以满足先进芯片对三维共形性和填充能力的需求 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[9](https://zhuanlan.zhihu.com/p/671632123)], [[10](https://zhuanlan.zhihu.com/p/521919587)]。
    *   **平面膜制备的局限性：** 该方法一般只适用于平面的膜层制备，与先进芯片的复杂三维结构不符 [[9](https://zhuanlan.zhihu.com/p/671632123)]。

#### 2.2 分子束外延设备 (Molecular Beam Epitaxy, MBE)
*   **应用及优点：** 分子束外延（MBE）是外延（EPI）技术的一种，主要用于在单晶衬底上生长一层与衬底具有相同晶向的单晶薄膜材料 [[10](https://zhuanlan.zhihu.com/p/521919587)]。它旨在生长高纯度、低缺陷密度的单晶半导体薄膜（如硅、SiGe、GaAs、GaN等），以改善器件性能，而非通用金属层 [[10](https://zhuanlan.zhihu.com/p/521919587)]。
*   **未广泛采用的原因：** 尽管在高质量单晶半导体生长方面有其独特优势，但分子束外延不适用于先进制程芯片的**主流金属薄膜**生长，原因如下：
    *   **主要用途差异：** MBE的核心是生长具有特定晶体结构和电学性能的单晶半导体层，这与多晶或非晶态的金属互连线、阻挡层等通用金属薄膜的需求不同。
    *   **高成本和低效率：** MBE设备造价极高，并且沉积速率相对较慢，对于需要大规模、快速沉积的多晶金属薄膜，其生产效率和成本效益远低于PVD和CVD等主流方法。
    *   **复杂性和操作难度：** MBE对真空环境、温度控制和材料纯度有极其严苛的要求，设备和操作复杂，不适合大规模工业化生产中对通用金属层的需求。

### 3. 先进制程芯片金属薄膜生长设备对比总结

| 技术类型 | 沉积原理 | 主要应用材料（先进制程） | 主要优点 | 主要局限性 | 在先进制程中的地位 |
| :------- | :------- | :----------------------- | :------- | :--------- | :----------------- |
| **PVD (磁控溅射)** | 物理溅射 | Al, Cu互连；TiN, TaN扩散阻挡层/硬掩膜；Ta, Ti等金属 | 膜层致密、结合力好、沉积效率高、均匀性好；低温沉积 | 台阶覆盖能力相对较弱（尤其是在高深宽比结构中） | 主流金属薄膜沉积技术，应用广泛 |
| **CVD (LPCVD, PECVD)** | 化学反应 | W填充（接触孔、字线）；间接支持金属层间介质填充 | 膜厚均匀性好、台阶覆盖性好（LPCVD）；生产效率高；可实现低温沉积（PECVD） | 工艺参数敏感；部分工艺台阶覆盖率差 | 介质层和部分金属层（如W）的核心技术 |
| **ALD** | 原子层级化学反应 | High-K介质/金属栅（Al2O3, HfO2, TiN, TaN）；Cu扩散阻挡层；W填充 | 原子层级膜厚控制、优异的均匀性和三维保形性、致密无针孔；低温沉积 | 沉积速率慢、前驱体选择和工艺控制复杂、成本高 | 先进制程（7nm及以下）的关键技术，日益重要 |
| **电子束蒸发** | 物理蒸发 | 特定金属薄膜（如LED电极）；不适用于主流互连 | 高纯度、膜厚精确控制、蒸发难熔金属 | 高能离子轰击导致衬底损伤；无法填充高深宽比结构；适用于平面膜 | 在先进芯片主流金属薄膜沉积中未广泛应用 |
| **分子束外延** | 单晶生长 | 高质量单晶半导体薄膜（如Si, SiGe, GaAs） | 单晶质量高、缺陷密度低、精确控制层厚和组分 | 生产成本高、沉积速率慢、设备复杂；主要用于半导体层而非通用金属层 | 用于高性能器件中的半导体外延层，不适用于主流金属互连或阻挡层生长 |
<div style="text-align:center; margin-top:24px; margin-bottom:30px;">
  <img src="https://vaccoat.com/wp-content/uploads/Vac-Deposition-Concepts-and-Methods-scaled.webp" style="max-width:720px; height:auto; display:block; margin: 0 auto 12px auto;">
  <div style="text-align:center; margin-top:8px; color: #888; font-size: 15px;">
    Comparison of deposition techniques
  </div>
</div>

### 4. 展望未来技术发展趋势

未来，随着芯片制程不断向3nm甚至更小节点发展，对薄膜沉积技术的要求将更加严苛：
1.  **ALD技术的关键性增强：** 针对更薄膜层和更复杂的3D立体结构（如GAA架构），ALD技术凭借其原子层级精确控制和优异的保形性，将在薄膜沉积环节的市场占有率持续提高 [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。
2.  **PVD技术的持续创新：** PVD设备将继续在各类金属层和硬掩膜沉积中发挥作用，并不断提升其在极高深宽比结构中的沉积能力，以适应复杂的器件结构需求。
3.  **异构集成和新材料挑战：** 随着异构集成（Heterogeneous Integration）的兴起，可能需要沉积更多种类、更复杂的新型金属材料和介质材料，这将驱动薄膜沉积设备向更多样化、更精确的方向发展。
4.  **国产化替代加速：** 中国半导体设备厂商（如北方华创、拓荆科技、微导纳米、中微公司）正在积极进行国产替代，在PVD、CVD和ALD等领域取得了显著进展，有望在先进薄膜沉积设备方面填补国内空白并走向国际市场 [[0](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)], [[1](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)]。

综上所述，在先进制程芯片的金属薄膜生长中，PVD、CVD和ALD设备是不可或缺的核心工具。它们各自发挥优势，协同满足了芯片制造对薄膜性能的严苛要求。而电子束蒸发和分子束外延设备则因其固有的局限性和应用侧重点不同，并未在主流金属薄膜沉积中广泛采用。未来，随着技术进步和产业需求升级，薄膜沉积技术将持续向更高精度、更复杂结构填充能力和更高效率方向演进。


# References

- [新能源重卡行业——定义与分类](https://pdf.dfcfw.com/pdf/H3_AP202406241636834646_1.pdf)
- [光大证券-半导体设备行业跟踪报告：半导体制造技术进步，原子层沉积(ALD)技术是关键-230206....](https://pdf.dfcfw.com/pdf/H3_AP202302071582835023_1.pdf)
- [PVD、ALD、LPCVD、PECVD 四种薄膜沉积技术介绍_行业资讯_新闻资讯_Showerhea...](https://amtdco.com/infodetail.aspx?PID=1093)
- [2021年全球及中国半导体薄膜沉积设备行业市场现状分析，国产替代高景气「图」_华经情报网_华经产业研...](https://www.huaon.com/channel/trend/803205.html)
- [制备固体氧化物燃料电池中电解质薄膜的电泳沉积法](https://manu56.magtech.com.cn/progchem/EN/lexeme/showArticleByLexeme.do?articleID=12954)
- [2022年薄膜设备市场份额及发展现状研究 薄膜设备行业下游导入持续取得新进展 - 报告精读 - 未来...](https://www.vzkoo.com/read/20220628498ce3db43a516e17b34d057.html)
- [基于搅拌摩擦的金属固相增材制造研究进展](https://jme.biam.ac.cn/CN/10.11868/j.issn.1001-4381.2021.000741)
- [从太平洋到喜马拉雅的沉积学新航程](http://www.cjxb.ac.cn/cn/article/doi/10.14027/j.issn.1000-0550.2023.005?viewType=HTML)
- [平安证券-半导体&电子行业：薄膜沉积设备颇具市场活力，国产化替代正当-231011.pdf](https://pdf.dfcfw.com/pdf/H3_AP202310111601216108_1.pdf)
- [薄膜沉积技术基本情况及对比](https://zhuanlan.zhihu.com/p/671632123)
- [芯片制造的核心工艺：一文看懂薄膜沉积](https://zhuanlan.zhihu.com/p/521919587)
