## Introduction

Chinese painting, as a significant component of traditional East Asian art, embodies rich visual semantics, symbolic abstraction, and unique structural composition rules. Unlike Western paintings that emphasize perspective realism, Chinese painting relies heavily on brushstroke representation, hierarchical composition, and semantic abstraction, posing distinctive challenges for computer vision analysis.

This repository aims to systematically organize and review existing research at the intersection of Chinese painting and computer vision. We structure the literature from low-level visual feature extraction to high-level visual–semantic grounding, covering representative works in both traditional methods and modern deep learning approaches. Additionally, we collect relevant datasets to facilitate further research in this emerging field.

We hope this survey can serve as a useful resource for researchers interested in digital humanities, computational aesthetics, and cross-domain visual understanding.

## Menu

- [Papers](#papers)
- [Datasets](#datasets)

## Papers<a id="papers"></a>

### 1. Form Response: Hierarchical Paradigms for Visual–Semantic Grounding

#### 1.1 Foundation: Primitive Extraction and Structural Encoding

- **中国山水画基本元素的自动分类算法研究（Research on Automatic Classification Algorithms for Basic Elements in Chinese Landscape Painting）** [[paper\]](https://d.wanfangdata.com.cn/thesis/Y876906)
  **Authors:** Wu Haifeng
  **Introduction:** This paper proposes a reliable automatic classification method for five basic elements of landscape paintings (branches, moss dots, figures, houses, seals) with targeted feature extraction and a dual-level decision tree classifier, aiming to improve the existing computer-aided Chinese painting authentication platform by providing objective quantitative indicators and enhancing detail comparison/retrieval functions, addressing the subjectivity of traditional expert-based forgery identification that hinders Chinese painting’s international development.

- **利用拓片恢复汉画像的浮雕效果（Restoration of Han Dynasty Brick and Stone Relief from Rubbing Images）**[Journal of Computer-Aided Design and Computer Graphics 2011] [[paper\]](https://d.wanfangdata.com.cn/thesis/Y876906)

  **Authors:** Wang Song, Li Zhuwen, Yu, Jinhui
  **Introduction:** A method to recover 3D relief surfaces from Han portrait rubbings (which lack such effect) is proposed, involving dividing relief surfaces into low-frequency (estimated via edge detection, blur analysis, prior-based interpolation) and high-frequency (estimated with minimal interaction) components, whose weighted superposition yields the final relief height, validated effectively by examples.

- **Sketch Tokens: A Learned Mid-level Representation for Contour and Object Detection**[CVPR 2013] [[paper\]](https://ieeexplore.ieee.org/document/6619250)

  **Authors:** Lim Joseph J., Zitnick C. Lawrence, Dollár, Piotr
  **Introduction:** This paper proposes a novel approach to learn and detect mid-level contour-based features called sketch tokens (via clustering hand-drawn contour patches and using a random forest classifier for efficient detection), which achieves state-of-the-art results in top-down contour detection (over 200x faster than competitors) and improves bottom-up pedestrian/object detection accuracy on INRIA/PASCAL datasets by complementing low-level features like gradient histograms.

- **Art2Contour: Salient Contour Detection in Artworks Using Generative Adversarial Networks**[ICIP 2020] [[paper]](https://ieeexplore.ieee.org/document/9191117)

  **Authors:** Sindel Aline, Maier Andreas, Christlein Vincent

  **Introduction:** To facilitate the comparison of artworks (where artists/workshops often reuse/amend motifs), this paper proposes a supervised GAN-based approach for salient contour extraction (reducing artworks to key lines/boundaries) that combines multiple regression task losses, and using a self-created high-resolution artwork dataset with annotated ground truth, it is shown to outperform competing methods both visually and quantitatively in contour detection on prints and paintings.

- **Modelling traditional Chinese paintings for content-based image classification and retrieval**[MULMM 2004] [[paper]](https://ieeexplore.ieee.org/document/1264994)

  **Authors:** Danging Zhang, Pham B., Yuefeng Li

  **Introduction:** This paper presents early results and a framework of applying CBIR to traditional Chinese paintings (motivated by aiding art historians' research, advancing CBIR techniques in this specific domain, and exploring high-dimensional data clustering), examining the suitability of existing CBIR proposals/algorithms and proposing a research agenda for Chinese paintings classification and retrieval, given that CBIR's key problems (feature extraction and similarity measure) are domain-specific.

- **Fast Accurate and Automatic Brushstroke Extraction**[ACM Trans. Multimedia Comput. Commun. Appl. 2021] [[paper]](https://dl.acm.org/doi/10.1145/3429742)

  **Authors:**Fu, Yunfei; Yu, Hongchuan; Yeh, Chih-Kuo; Lee, Tong-Yee; Zhang, Jian J 

  **Introduction:** Brushstrokes, as artists' "handwriting" in paintings, are crucial for style learning, painting simulation and authentication. Existing methods face challenges like inefficient extraction of interleaved brushstrokes, neglected soft transitions and reliance on manual annotation. This paper proposes DStroke, a deep neural network-based algorithm, enabling fully automatic, fast and accurate brushstroke extraction with restored soft transitions, outperforming existing methods in experiments.

- **Automatic extraction of brushstroke orientation from paintings**[Mach. Vis. Appl. 2009] [[paper]](https://link.springer.com/article/10.1007/s00138-007-0098-7)

  **Authors:** Berezhnoy, Igor E.; Postma, Eric O.; van den Herik, H. Jaap

  **Introduction:**Brushstroke orientation is a key spatial characteristic for painting analysis, so this paper proposes the POET technique based on a circular filter and dedicated orientation extraction phase, which achieves human-level performance in automatically extracting brushstroke orientation from digital paintings to assist art experts.

- **Research on quantifying color of HSV in extraction of middle-level semantic objects of traditional Chinese painting images**[Proc. 2nd Int. Conf. Comput. Sci. Netw. Technol. 2012] [[paper]](https://ieeexplore.ieee.org/document/6525881)

  **Authors:** Liu, Hongzhe; Liang, Ye; Xu, Guangmei

  **Introduction:**For extracting scripts (black ink) and seals (red) in traditional Chinese paintings, this paper proposes an HSV color quantifying model based on the paintings’ characteristics, analyzes results under different quantifying values, and achieves satisfactory extraction effects to support accurate extraction of the two semantic objects.

- **A novel algorithm for extraction of the scripts part in traditional Chinese painting images**[Proc. 2nd Int. Conf. Softw. Technol. Eng. 2010] [[paper]](https://ieeexplore.ieee.org/document/5608756)

  **Authors:** HONG BAO；YE LIANG；HONG-ZHE LIU ；De Xu

  **Introduction:** As the scripts part of traditional Chinese paintings has important semantics, and few popular image processing techniques are applied in its extraction, this paper proposes a simple yet efficient novel algorithm based on the color and structure features of Chinese characters, with satisfactory results.

- **Object Extraction in Chinese Painting Base on Visual Saliency**[] [[paper]](https://ieeexplore.ieee.org/document/7469181)

  **Authors:** Hu, Zhengkun and Wang, Tingmei

  **Introduction:**  To address the challenge of object extraction in traditional Chinese paintings (featuring abstract form, implicit expression, and limited fixed colors) that general image processing algorithms cannot handle, this paper proposes a novel, simple, and efficient method based on visual saliency, which generates full-resolution saliency maps and achieves complete object extraction in important regions through experiments.

- **Image Classification Based on Sparse Coding and Multi-Scale Spatial Latent Semantic Analysis**[J. Comput. Res. Dev. 2014] [[paper]](https://link.springer.com/article/10.1186/s13640-019-0425-8)

  **Authors:** Zhao, Zhongqiu；Ji, Haifeng ；Gao, Jun；Hu, Donghui ； Wu, Xindong

  **Introduction:**To address the loss of spatial information and insufficient discriminability in traditional sparse coding for image classification, this paper proposes a method integrating spatial pyramid matching, sparse coding, and PLSA model: it extracts spatial information via multi-scale image segmentation, forms co-occurrence matrices through feature soft quantization, mines local latent semantics, and achieves higher classification accuracy than existing methods like ScSPM.

- **国画的艺术目标分割及深度学习与分类（Learning Artistic Objects for Improved Classification of Chinese Paintings）**[J. Image Graph. 2018] [[paper]](https://www.cjig.cn/zh/article/doi/10.11834/jig.170545/)

  **Authors:** Sheng, Jiachuan; Li, Yuzhi

  **Introduction:** To address the limitations of direct feature extraction from entire Chinese paintings and susceptibility to noise, this paper proposes a framework integrating SLIC superpixel segmentation, MSRMAO interactive artistic object extraction, O-CNN feature description (fine-tuned VGG-F model), and SVM-based fusion, achieving 89% average accuracy in classifying 10 artists’ works and outperforming MHMM and Fusion methods.

#### 1.2 Integration: Mid-Level Fusion and Semantic Composition

- **Monte Carlo Convex Hull Model for classification of traditional Chinese paintings**[Neurocomputing 2016] [[paper]](https://www.sciencedirect.com/science/article/abs/pii/S0925231215011601)

  **Authors:**  Meijun Sun，Dong Zhang ，Zheng Wang ，Jinchang Ren，Jesse S. Jin

  **Introduction:** To address the challenge of characterizing artistic styles in traditional Chinese paintings, this paper proposes an integrated feature-based descriptor with an infusion factor and Monte Carlo Convex Hull (MCCH) feature selection model, combined with SVM, outperforming existing techniques in classification precision and recall.

- **Recognition of Chinese artists via windowed and entropy balanced fusion in classification of their authored ink and wash paintings (IWPs)**[Pattern Recognit. 2014] [[paper]](https://www.sciencedirect.com/science/article/abs/pii/S0031320313003385?via%3Dihub)

  **Authors:** Jiachuan Sheng，Jianmin Jiang

  **Introduction:** To address the difficulty of classifying Chinese ink-wash paintings due to similar content, this paper extracts histogram-based local and global features to characterize artistic styles, uses neural networks for classification, and proposes a windowed entropy-balanced fusion scheme, outperforming existing benchmark techniques.

- **Modelling traditional Chinese paintings for content-based image classification and retrieval**[Proc. 10th Int. Multimed. Modelling Conf. 2004]] [[paper]](https://ieeexplore.ieee.org/document/1264994)

  **Authors:** Danging Zhang and Pham, B. and Yuefeng Li

  **Introduction:** To support art historians' research on oriental paintings and advance CBIR techniques, this paper proposes a framework for modelling traditional Chinese paintings, examines the suitability of existing CBIR algorithms, and sets a research agenda for their classification and retrieval based on automatically extracted visual features.

- **Automatic traditional Chinese painting classification: A benchmarking analysis** [Comput. Intell. 2020] [[paper\]](https://onlinelibrary.wiley.com/doi/abs/10.1111/coin.12328)

  **Authors:** Sze-Teng Liong, Yen-Chang Huang, Shumeng Li, Zhongkai Huang, Jingyang Ma, Yee Siang Gan

  **Introduction:** To provide a comprehensive benchmark for traditional Chinese painting classification, this paper conducts a systematic comparative analysis of multiple classic machine learning and deep learning algorithms, evaluating their performance based on texture, color, and shape features, and offering valuable references for subsequent related research.

- **Image Classification Based on Sparse Coding and Multi-Scale Spatial Latent Semantic Analysis**[J. Comput. Res. Dev. 2014] [[paper]](https://link.springer.com/article/10.1186/s13640-019-0425-8)

  **Authors:** Zhao, Zhongqiu；Ji, Haifeng ；Gao, Jun；Hu, Donghui ； Wu, Xindong

  **Introduction:**To address the loss of spatial information and insufficient discriminability in traditional sparse coding for image classification, this paper proposes a method integrating spatial pyramid matching, sparse coding, and PLSA model: it extracts spatial information via multi-scale image segmentation, forms co-occurrence matrices through feature soft quantization, mines local latent semantics, and achieves higher classification accuracy than existing methods like ScSPM.

- **Element Identification and Feature Extraction of Chinese Painting Based on Computer Vision and CAD** [Comput.-Aided Des. Appl. 2023] [[paper\]](https://cad-journal.net/files/vol_21/CAD_21(S14)_2024_220-236.pdf)

  **Authors:** Bo Ning, Zichao Xing

  **Introduction (English):** To address the difficulty of accurate identification and feature extraction of Chinese painting elements, this paper proposes a method integrating computer vision and CAD technology, realizing effective recognition of core elements and precise extraction of their features, which provides technical support for the digital preservation and intelligent analysis of Chinese paintings.

- **Painting Element Segmentation Algorithm Based on Deep Network** [Proc. Photonics & Electromagnetics Res. Symp. (PIERS) 2021] [[paper\]](https://ieeexplore.ieee.org/document/9694935)

  **Authors:** Song Ran, Lan Lin

  **Introduction:** To solve the problems of low accuracy and noise sensitivity in traditional ancient painting element segmentation, this paper proposes a method combining data enhancement, U-Net/IndexNet models and guided filtering, which effectively overcomes over-fitting caused by small sample size and optimizes segmentation results.

- **The Elements Extraction on Traditional Chinese Paintings Based on Object Detection** [ - 2019] [[paper\]](https://dl.acm.org/doi/10.1145/3375959.3375980)

  **Authors:** Qingyu Meng, Kaiyue Li, Mingquan Zhou, Huanhuan Zhang

  **Introduction:** To address the inefficiency and subjectivity of manual extraction of traditional Chinese painting elements, this paper proposes an extraction method based on object detection technology, realizing automatic and accurate identification and extraction of core elements in Chinese paintings, and improving the efficiency of digital processing of traditional Chinese paintings.

- **中国画分类的改进嵌入式学习算法（Improved Embedded Learning for Classification of Chinese Paintings）** [J. Comput.-Aided Des. Comput. Graph. 2018] [[paper\]](https://www.jcad.cn/article/doi/10.3724/SP.J.1089.2018.16539)

  **Authors:** Yuzhi Li, Jiachuan Sheng, Bin Hua

  **Introduction (English):** To address the limitation that existing Chinese painting classification ignores inter-painting relationships and feature importance, this paper proposes an improved embedded learning algorithm: it extracts features via fine-tuning the pre-trained VGG-F model, integrates mutual information into embedded learning, and uses SVM for classification, achieving 86% average accuracy on 10 artists’ works with better robustness.

- **Feature Extraction and Recognition Based on Integrated Material Painting Images** [Automatic Control Comput. Sci. 2025] [[paper\]](https://link.springer.com/article/10.3103/S014641162570052X)

  **Authors:** Ying Cheng, Hongwei Li, Tao Meng, Lu Bai, Yan Li

  **Introduction (English):** To improve the accuracy and robustness of feature extraction and classification for Chinese painting images, this paper proposes a method integrating multi-color gamut texture analysis and block color feature extraction, enhanced by multi-resolution gray-level co-occurrence matrix technology. Experiments show average accuracy and recall are 12.2% and 14% higher than traditional methods, with better noise resistance (7% and 7.5% accuracy/recall decrease under 30dB noise).

#### 1.3 Emergence: Deep Hierarchical Representation Learning

- **Automatic traditional Chinese painting classification: A benchmarking analysis** [Comput. Intell. 2020] [[paper\]](https://onlinelibrary.wiley.com/doi/abs/10.1111/coin.12328)

  **Authors:** Sze-Teng Liong, Yen-Chang Huang, Shumeng Li, Zhongkai Huang, Jingyang Ma, Yee Siang Gan

  **Introduction:** To provide a comprehensive benchmark for traditional Chinese painting classification, this paper conducts a systematic comparative analysis of multiple classic machine learning and deep learning algorithms, evaluating their performance based on texture, color, and shape features, and offering valuable references for subsequent related research.

- **DeepPainter: Painter Classification Using Deep Convolutional Autoencoders** [CoRR 2017] [[paper\]](https://arxiv.org/abs/1711.08763)

  **Authors:** Eli David, Nathan S. Netanyahu

  **Introduction (English):** To address the reliance on manual feature extraction in traditional painter classification, this paper proposes a DeepPainter approach based on deep convolutional autoencoders, operating directly on raw pixels without preprocessing. It initializes a supervised CNN via the pre-trained autoencoder, achieving 96.52% accuracy in 3-painter classification (63% error rate reduction vs. previous state-of-the-art).

- **Three-dimensional reconstruction image generation of traditional Chinese painting elements** [Eng. Appl. Artif. Intell. 2025] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0952197625014198)

  **Authors:** Qiyao Hu, Jingyu Wang, Xianlin Peng, Tengfei Li, Rui Cao

  **Introduction (English):** To address the lack of 3D datasets for traditional Chinese paintings and the challenge of single-view 3D reconstruction, this paper proposes the TCPE-3D framework, integrating the OTX-MVG multi-view synthesis module, NeRF synthesis module, and mesh generation module. It constructs the 3DTCP dataset, solves the Janus problem, and achieves high-quality 3D reconstruction of Chinese painting elements with better visualization results than state-of-the-art methods.

- **BPA-SAM: A Prompt Enhancement Method for SAM Using Bounding Boxes in Gongbi Painting Datasets** [J. Graph. (China) 2025] [[paper\]](10.11996/JG.j.2095-302X.2025020322)

  **Authors:** Tiansheng Zhang, Minfeng Zhu, Yiwen Ren, Chenhan Wang, Lidong Zhang, Wei Zhang, Wei Chen

  **Introduction (English):** To improve the segmentation accuracy of Gongbi painting elements using the Segment Anything Model (SAM), this paper proposes the BPA-SAM prompt enhancement method. It leverages bounding box prompts tailored to Gongbi painting datasets, enhancing the model’s ability to capture fine-grained details of traditional Chinese realistic painting elements, and achieves effective segmentation performance as verified by experiments on relevant datasets.

- **Ancient Painting to Natural Image: A New Solution for Painting Processing** [arXiv:1901.00224 [cs.CV] 2019] [[paper\]](https://arxiv.org/abs/1901.00224)

  **Authors:** Tingting Qiao, Weijing Zhang, Miao Zhang, Zixuan Ma, Duanqing Xu

  **Introduction (English):** To address the lack of large-scale annotated datasets for ancient Chinese painting processing, this paper proposes a Domain Style Transfer Network (DSTN) that converts ancient flower, bird, and landscape paintings to photo-realistic natural images. With a compound loss ensuring preserved color composition and content, the transferred images outperform state-of-the-art methods in human perceptual tests and downstream image processing tasks.

- **Interactively transforming chinese ink paintings into realistic images using a border enhance generative adversarial network** [Multimed. Tools Appl. 2023] [[paper\]](https://link.springer.com/article/10.1007/s11042-022-13684-4)

  **Authors:** Chieh-Yu Chung, Szu-Hao Huang

  **Introduction (English):** To address the lack of research on transforming Chinese ink paintings into realistic images with user interaction, this paper proposes a border enhance GAN (generative adversarial network) by combining cycle-consistent GAN, pix2pix, and a label function. It enhances border details of ink paintings (with low-quality texture and border features) and generates more accurate realistic images, enabling interactive selection of geologic styles for an immersive experience.

- **Multimodal Fusion for Traditional Chinese Painting Generation** [Adv. Multimed. Inf. Process. – PCM 2018] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-030-00764-5_3)

  **Authors:** Sanbi Luo, Si Liu, Jizhong Han, Tao Guo

  **Introduction (English):** To address the challenge of AI-generated traditional Chinese paintings with creativity, this paper proposes a multimodal fusion framework integrating suitable networks for generating different painting elements. It adopts a divide-and-conquer strategy to handle large images under limited GPU resources, enabling automatic generation of complete traditional Chinese paintings in minutes.

#### 1.4 Conceptualization: Knowledge-Grounded Controllable Understanding

- **ContextNet: representation and exploration for painting classification and retrieval in context** [Int. J. Multimed. Info. Retr. 2020] [[paper\]](https://link.springer.com/article/10.1007/s13735-019-00189-4)

  **Authors:** Noa Garcia, Benjamin Renoust, Yuta Nakashima

  **Introduction (English):** To address the limitation that standard CNNs fail to capture subtle relationships between artistic attributes, this paper proposes ContextNet with two modalities: one based on multitask learning (capturing visual attribute relationships) and another on knowledge graphs (encoding non-visual attribute connections). It enhances visual representations, improving painting classification accuracy by up to 7.3% and cross-modal retrieval performance by 37.24% compared to baselines.

- **Leveraging Knowledge Graphs and Deep Learning for automatic art analysis** [Knowl.-Based Syst. 2022] [[paper\]](https://www.sciencedirect.com/science/article/pii/S0950705122004105)

  **Authors:** Giovanna Castellano, Vincenzo Digeno, Giovanni Sansaro, Gennaro Vessio

  **Introduction (English):** To address the limitation that existing art analysis systems rely solely on visual features, metadata, and textual comments, this paper constructs an artistic Knowledge Graph (KG) integrating WikiArt and DBpedia, and proposes a KG-enabled fine art classification method. It extracts embeddings from the KG as "contextual" knowledge and injects them into a Deep Learning model, achieving encouraging results in artwork attribute prediction and bridging the gap between Humanities and Computer Science.

- **Object-Based Visual Sentiment Concept Analysis and Application** [Proc. 22nd ACM Int. Conf. Multimedia 2014] [[paper\]](https://dl.acm.org/doi/10.1145/2647868.2654935)

  **Authors:** Tao Chen, Felix X. Yu, Jiawei Chen, Yin Cui, Yan-Ying Chen, Shih-Fu Chang

  **Introduction (English):** To address the lack of fine-grained analysis in traditional visual sentiment research, this paper proposes an object-based visual sentiment concept analysis framework. It extracts sentiment-related concepts from image objects, builds a sentiment concept hierarchy, and integrates multi-modal features to predict image sentiment. Experiments show the method outperforms state-of-the-art approaches in sentiment classification and retrieval tasks.

- **Diversified Visual Attention Networks for Fine-Grained Object Classification** [IEEE Trans. Multimed. 2017] [[paper\]](https://ieeexplore.ieee.org/document/7807286)

  **Authors:** Bo Zhao, Xiao Wu, Jiashi Feng, Qiang Peng, Shuicheng Yan

  **Introduction (English):** To address the challenge of capturing discriminative local details in fine-grained object classification, this paper proposes a Diversified Visual Attention Network (DVAN). It integrates multiple attention mechanisms to generate diverse and complementary attention maps, enhancing the model’s ability to focus on subtle distinguishing features. Experiments on benchmark datasets (CUB-200-2011, Stanford Cars, FGVC-Aircraft) show DVAN outperforms state-of-the-art methods with improved classification accuracy and robustness.

- **On Using Histograms of Local Invariant Features for Image Retrieval** [Tech. Rep. 2006] [[paper\]](https://lmb.informatik.uni-freiburg.de/people/halawani/mva05.pdf)

  **Authors:** Alaa Halawani, Hans Burkhardt

  **Introduction (English):** To improve the effectiveness of image retrieval by preserving local structure and ensuring Euclidean motion invariance, this paper proposes methods for constructing histograms from local invariant features (computed around salient points) using Haar integrals with nonlinear kernel functions. It compares different histogram construction approaches on a 15,000-image database, verifying their performance in image retrieval tasks.

- **On the accuracy of the Sobel edge detector** [Image Vis. Comput. 1983] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/0262885683900069)

  **Authors:** J Kittler

  **Introduction (English):** To evaluate the accuracy of the Sobel edge detector, this paper conducts a systematic analysis of its performance in edge localization. It quantifies the detector’s positional error under different noise conditions and edge configurations, providing theoretical and experimental foundations for the rational use of the Sobel operator in image processing tasks.

  **Introduction (中文):** 为评估 Sobel 边缘检测器的准确性，本文对其边缘定位性能进行了系统分析，量化了该检测器在不同噪声条件和边缘配置下的位置误差，为图像处理任务中合理使用 Sobel 算子提供了理论与实验依据。

- **Edge Boxes: Locating Object Proposals from Edges** [Comput. Vis. – ECCV 2014] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-319-10602-1_26)

  **Authors:** C. Lawrence Zitnick, Piotr Dollár

  **Introduction (English):** To improve the efficiency and accuracy of object detection, this paper proposes Edge Boxes, a method for generating object proposals from edges. It uses the number of fully contained contours in a bounding box as an objectness score, enabling fast evaluation of millions of candidates and returning top-scoring proposals. Experiments show 96% object recall at 0.5 overlap threshold with 1000 proposals, running in 0.25 seconds.

- **Oriented edge forests for boundary detection** [IEEE Conf. Comput. Vis. Pattern Recognit. (CVPR) 2015] [[paper\]](https://ieeexplore.ieee.org/document/7298782)

  **Authors:** Sam Hallman, Charless C. Fowlkes

  **Introduction (English):** To address the inefficiency of structured forest models and the limitation of simple gradients in boundary detection, this paper proposes an oriented edge forest model. It combines local edge orientation-based training example clustering and scale-dependent probability calibration, outperforming benchmarks on BSDS500 with 10x faster training and lower memory usage.

- **Learning to detect natural image boundaries using local brightness, color, and texture cues** [IEEE Trans. Pattern Anal. Mach. Intell. 2004] [[paper\]](https://ieeexplore.ieee.org/document/1273918)

  **Authors:** D.R. Martin, C.C. Fowlkes, J. Malik

  **Introduction (English):** To improve the accuracy of natural image boundary detection, this paper proposes a method leveraging local brightness, color, and texture cues. It formulates feature responses to boundary-related changes and uses a classifier trained on human-labeled ground truth to combine cues optimally, outperforming existing approaches with a linear model and explicit texture treatment.

### 2. Attribute Assignment: Semantic Conditioning and Appearance Control

#### 2.1 Perception-Oriented Modeling of Artistic Emotion and Aesthetics

- **SCEP—A New Image Dimensional Emotion Recognition Model Based on Spatial and Channel-Wise Attention Mechanisms** [IEEE Access 2021] [[paper\]](https://ieeexplore.ieee.org/document/9348893)

  **Authors:** Bo Li, Hui Ren, Xuekun Jiang, Fang Miao, Feng Feng, Libiao Jin

  **Introduction (English):** To address the limitation that existing image emotion recognition models fail to fully capture discriminative emotional features, this paper proposes the SCEP model integrating spatial and channel-wise attention mechanisms. It enhances the extraction of emotion-related spatial regions and channel features, optimizes feature representation via a multi-scale fusion strategy, and achieves superior performance on the GEMEP-FERA, AffectNet, and CK+ datasets compared to state-of-the-art methods.

- **Image Retrieval by Emotional Semantics: A Study of Emotional Space and Feature Extraction** [IEEE Int. Conf. Syst. Man Cybern. 2006] [[paper\]](https://ieeexplore.ieee.org/document/4274431)

  **Authors:** Wei-ning Wang, Ying-lin Yu, Sheng-ming Jiang

  **Introduction (English):** To address the gap between low-level image features and high-level emotional semantics in retrieval systems, this paper constructs a three-dimensional emotional factor space using 12 pairs of emotional words. It designs three novel features (luminance-warm-cool fuzzy histogram, saturation-warm-cool fuzzy histogram with color contrast, luminance contrast with edge sharpness) and uses SVM regression to predict emotional factors, enabling effective emotion-based image retrieval.

- **Interpretable aesthetic features for affective image classification** [IEEE Int. Conf. Image Process. (ICIP) 2013] [[paper\]](https://ieeexplore.ieee.org/document/6738665)

  **Authors:** Xiaohui Wang, Jia Jia, Jiaming Yin, Lianhong Cai

  **Introduction (English):** To address the poor interpretability of traditional visual features and low classification accuracy in affective image analysis, this paper proposes interpretable aesthetic features inspired by art theories. These intuitive and discriminative features not only improve classification accuracy compared to state-of-the-art methods but also explain why images convey specific emotions.

- **Exploring Principles-of-Art Features For Image Emotion Recognition** [Proc. 22nd ACM Int. Conf. Multimedia 2014] [[paper\]](https://dl.acm.org/doi/10.1145/2647868.2654930)

  **Authors:** Sicheng Zhao, Yue Gao, Xiaolei Jiang, Hongxun Yao, Tat-Seng Chua, Xiaoshuai Sun

  **Introduction (English):** To bridge the gap between low-level visual features and high-level emotional semantics in image emotion recognition, this paper explores principles-of-art features derived from art theory (e.g., balance, rhythm, proportion, emphasis). It integrates these domain-specific features with traditional visual features, enhancing the model’s ability to capture emotion-conveying cues. Experiments on benchmark datasets demonstrate superior performance compared to state-of-the-art methods, validating the effectiveness of art-inspired features.

- **Exploring Discriminative Representations for Image Emotion Recognition With CNNs** [IEEE Trans. Multimed. 2020] [[paper\]](https://ieeexplore.ieee.org/document/8764506)

  **Authors:** Wei Zhang, Xuanyu He, Weizhi Lu

  **Introduction (English):** To address the limitation that existing CNN models for image emotion recognition ignore low-level style features (color, texture, shape) vital for evoking emotions, this paper proposes a novel CNN model. It integrates high-layer content information and low-layer style information, and designs a loss function incorporating emotion labeling quality to handle label uncertainty, achieving more discriminative representations for emotion recognition.

- **ColorNetVis: An Interactive Color Network Analysis System for Exploring the Color Composition of Traditional Chinese Painting** [IEEE Trans. Vis. Comput. Graph. 2024] [[paper\]](https://ieeexplore.ieee.org/document/10499893)

  **Authors:** Xiaojiao Chen, Qinghua Liu, Yonghao Chen, Ruihan Wang, Yang You, Wanxin Deng, Chen Wei, Wang Xiaosong

  **Introduction (English):** To address the inefficiency of manual color relationship analysis in traditional Chinese paintings, this paper proposes ColorNetVis, an interactive color network analysis system. It builds a bipartite network between colors and paintings via color difference measurement, projects it into a one-mode color network, and integrates multi-view visualization tools to help researchers efficiently explore color composition and potential relationships.

- **Feature Extraction and Classification Algorithms for Chinese Paintings（中国画的特征提取与分类算法研究）** [Master's Thesis, Xi'an Univ. Archit. Technol. 2018] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=lSOmZDqoX8OOrDLPi1pLFdubhQlsQHQ-J7BwJ1u4pBqxyWLJ09sV4X_Yi3WKRwWTCE2-IPjqCgeFfCT_kvRNX2L4EpxM_IAMzk_Yb0XjfB0VQP8cpIgxy4Yzt7kDT4n2CKZ0nUt2br2a3vkBlq8shDgml_z3BovFwwBSyinWguTQowllF0dHbsrV0SMKc1Mv&uniplatform=NZKPT&language=CHS)

  **Author:** Jing Wang

  **Introduction (English):** Focusing on the challenges of feature extraction and classification in Chinese paintings, this master's thesis investigates effective algorithms for capturing unique artistic features (e.g., brushwork, ink wash, composition) of Chinese paintings. It compares and optimizes traditional machine learning and deep learning-based classification methods, aiming to improve the accuracy and robustness of Chinese painting classification tasks.

- **Content-Based Identifying and Classifying Traditional Chinese Painting Images** [IEEE Congr. Image Signal Process. 2008] [[paper\]](https://ieeexplore.ieee.org/document/4566716)

  **Authors:** Guanming Lu, Zhong Gao, Danni Qin, Xin Zhao, Mengjue Liu

  **Introduction (English):** To address the need for effective identification and classification of digitalized traditional Chinese painting (TCP) images, this paper proposes a content-based scheme. It extracts chromatic and textural features to represent TCP visual content, and uses four classifiers to learn styles, art movements, and painter characteristics, achieving over 85% accuracy in related classification tasks.

#### 2.2 Physics-Based Simulation and Material-Oriented Stylization

- **Computer‐generated Chinese color ink paintings** [J. Chin. Inst. Eng. 2006] [[paper\]](https://www.tandfonline.com/doi/abs/10.1080/02533839.2006.9671203)

  **Authors:** Der‐Lor Way, Wei‐Jin Lin, Zen‐Chung Shih

  **Introduction (English):** To simulate the unique artistic effects of Chinese color ink paintings via computer, this paper proposes a generation method integrating traditional painting techniques and digital processing. It models key elements such as ink wash diffusion, brushwork texture, and color blending, and uses image synthesis algorithms to reproduce the aesthetic characteristics of Chinese color ink paintings, achieving vivid and authentic computer-generated results.

- **Physical-based Model of Ink Diffusion in Chinese Paintings** [Int. Conf. Cent. Eur. Comput. Graph. Vis. 2003] [[paper\]](https://www.researchgate.net/publication/221546314_Physical-based_Model_of_Ink_Diffusion_in_Chinese_Paintings)

  **Authors:** Der-Lor Way, Sheng-Wen Huang, Zen-Chung Shih

  **Introduction (English):** Given the scarcity of research on Chinese ink painting (a three-thousand-year-old non-photorealistic art) and the challenge of simulating complex ink behavior, this paper proposes a physics-based ink diffusion method based on observation and analysis. It can simulate various tone expressions on different paper types, elucidate the mixing effect of strokes from different brushes, and validate the results through comparison with real ink paintings.

- **Diffusion rendering of black ink paintings using new paper and ink models** [Comput. Graph. 2001] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0097849300001321)

  **Author:** Jintae Lee

  **Introduction (English):** To address the challenge of simulating realistic ink diffusion effects in oriental black ink paintings, this paper proposes a novel rendering method based on improved paper and ink models. It constructs fiber mesh paper models (random or uniform) to mimic different paper textures, designs elastic bristle/brush models to generate authentic strokes, and simulates ink diffusion dynamics. The method enables real-time dynamic rendering of ink spreading, reflecting both local temporal variations and global gray tone changes of the paper.

- **Computer-generated watercolor** [Proc. 24th Annu. Conf. Comput. Graph. Interact. Tech. (SIGGRAPH) 1997] [[paper\]](https://dl.acm.org/doi/10.1145/258734.258896)

  **Authors:** Cassidy J. Curtis, Sean E. Anderson, Joshua E. Seims, Kurt W. Fleischer, David H. Salesin

  **Introduction (English):** To automatically simulate the diverse artistic effects of watercolor, this paper proposes a watercolor model based on an ordered set of translucent glazes. Each glaze is independently created via a shallow-water fluid simulation, and the Kubelka-Munk compositing model is adopted to simulate the optical effect of superimposed glazes. The method is applied to three scenarios: interactive watercolor painting systems, automatic image "watercolorization," and non-photorealistic rendering of 3D scenes.

- **A diffusion model for computer animation of diffuse ink painting** [Proc. Comput. Animation'95 1995] [[paper\]](https://ieeexplore.ieee.org/document/393542)

  **Authors:** T.L. Kunii, G.V. Nosovskij, T. Hayashi

  **Introduction (English):** To realize computer animation of diffuse ink painting with realistic ink spreading effects, this paper proposes a specialized diffusion model. It models the dynamic process of ink diffusion on paper, capturing the temporal evolution of ink tones and spreading ranges. The model enables smooth and natural animation of ink diffusion, providing a technical solution for dynamic simulation of traditional ink painting art.

- **A model based technique for realistic oriental painting** [10th Pac. Conf. Comput. Graph. Appl. 2002] [[paper\]](https://ieeexplore.ieee.org/document/1167898)

  **Authors:** Young Jung Yu, Young Bok Lee, Hwan Gue Cho, Do Hoon Lee

  **Introduction (English):** To generate realistic oriental paintings with authentic diffusion and stroke effects, this paper proposes a model-based technique. It includes a local equilibrium model (LEM) for efficient calculation of water and ink movement, a fiber mesh paper model with three-layer cell structure (supporting overlapped strokes), and a brush model capable of shading effects, enhancing the realism of computer-generated oriental paintings.

- **Non-photorealistic rendering of ink painting style diffusion** [IEEE Int. Conf. Granular Comput. 2009] [[paper\]](https://ieeexplore.ieee.org/document/5255155)

  **Author:** Tianding Chen

  **Introduction (English):** To achieve non-photorealistic rendering (NPR) that reproduces the unique diffusion style of ink paintings, this paper proposes a targeted rendering method. It focuses on simulating the natural spreading and blending characteristics of ink in traditional ink paintings, integrating granular computing principles to optimize the diffusion effect simulation. The method effectively captures the artistic charm of ink diffusion, providing a new approach for ink painting-style NPR.

- **Real-time image-based Chinese ink painting rendering** [Multimedia Tools Appl. 2014] [[paper\]](https://link.springer.com/article/10.1007/s11042-012-1126-9)

  **Authors:** Lixing Dong, Shufang Lu, Xiaogang Jin

  **Introduction (English):** To address the trade-off between realism and efficiency in Chinese ink painting rendering, this paper proposes a real-time image-based method. It extracts structural and tonal features from input images, simulates key ink painting effects (e.g., ink diffusion, dry brush texture, and hierarchical ink wash) via lightweight algorithms, and achieves real-time rendering without compromising the artistic authenticity of traditional Chinese ink paintings.

- **Simulating Aging and Reverse-Aging Phenomena of Traditional Chinese Paintings** [Proc. Annu. Conf. Jpn. Soc. Artif. Intell. (JSAI) 2012] [[paper\]](https://www.jstage.jst.go.jp/article/pjsai/JSAI2012/0/JSAI2012_4M1IOS3c5/_article/-char/ja/)

  **Authors:** Lieu-Hen Chen, Meng-Feng Tsai, Chien-Hui Hsu, Yu-Sheng Chen

  **Introduction (English):** Conventional image processing techniques for simulating painting aging and restoration are overly simplistic, failing to consider storage conditions, pigment/surface material status, and historical color trends. This leads to unrealistic results in both aging simulation of contemporary works and reverse-aging (restoration) of old paintings. To address this, the paper proposes a knowledge-based approach: it discovers color fading knowledge over time by collecting, categorizing, and analyzing paintings from different eras, and tracks relationships between color distribution histograms, painting subjects, creation dynasties, and pigment properties. The prototype system enables simulation of both aging and reverse-aging processes, with initial results verifying its potential for realistic aging effects on traditional Chinese paintings.

#### 2.3 Generative Stylization and Cross-Domain Transfer of Color Semantics

- **TCPColor：基于文本到图像生成模型的中国画配色方案推荐系统** [图学学报 2025] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=lSOmZDqoX8PnWbwCvdy1TWMbZz6m5n8g6cpXJe-77YoT86k49cdnO5uuaB_KNe8afekAqu7SeFowDKI7UJj2-K76w6goI3RZOMlEfd82VAMv2q8TdZoKBW9-vjGyOsxg21bwTABzC3PCjZRY0_Z1PnG4sL66GBNGluwW5OHeP-ln07z807j3XQ==&uniplatform=NZKPT&language=CHS)

  **Authors:** 张迪（Zhang Di）, 张文安（Zhang Wenan）, 姜智德（Jiang Zhide）, 吴爱霞（Wu Aixia）, 孔浩（Kong Hao）, 郭显（Guo Xian）, 陈为（Chen Wei）

  **Introduction (English):** Aiming at the difficulty of matching color schemes with artistic themes and styles in traditional Chinese painting creation, this paper proposes TCPColor, a color scheme recommendation system based on text-to-image generation models. The system extracts and organizes color features from classic Chinese painting works by leveraging the semantic understanding and color modeling capabilities of text-to-image models, and provides personalized color scheme recommendations according to user-specified themes, styles, or scenes. Experimental results demonstrate that the system can generate color schemes consistent with the artistic characteristics of traditional Chinese paintings, offering effective support for Chinese painting creation and digital restoration.

- **Detail-Preserving CycleGAN-AdaIN Framework for Image-to-Ink Painting Translation** [IEEE Access 2020] [[paper\]](https://ieeexplore.ieee.org/document/9142197)

  **Authors:** Fengquan Zhang, Huaming Gao, Yuping Lai

  **Introduction (English):** To address the loss of image details and insufficient artistic authenticity in existing image-to-ink painting translation methods, this paper proposes a detail-preserving framework integrating CycleGAN and AdaIN. It introduces AdaIN to align style features while retaining content details, optimizes the cycle consistency loss to enhance translation stability, and designs a detail-preserving loss to emphasize texture and structural information. The method achieves high-quality ink painting translation with both authentic artistic style and intact input image details.

- **Contour-enhanced CycleGAN framework for style transfer from scenery photos to Chinese landscape paintings** [Neural Comput. Appl. 2022] [[paper\]](https://link.springer.com/article/10.1007/s00521-022-07432-w)

  **Authors:** Xianlin Peng, Shenglin Peng, Qiyao Hu, Jinye Peng, Jiaxin Wang, Xinyu Liu, Jianping Fan

  **Introduction (English):** To address the lack of distinct contours and insufficient artistic style authenticity in style transfer from scenery photos to Chinese landscape paintings, this paper proposes a contour-enhanced CycleGAN framework. It integrates a contour extraction module to emphasize the structural contours of Chinese landscape paintings, optimizes the generator and discriminator architectures to capture style features such as brushwork and ink wash, and introduces a contour consistency loss to maintain contour integrity during transfer. Experiments show the method generates Chinese landscape paintings with clear contours, authentic artistic style, and natural integration of photo content and painting style.

- **SRAGAN: Saliency Regularized and Attended Generative Adversarial Network for Chinese Ink-wash Painting Style Transfer** [arXiv 2025] [[paper\]](https://arxiv.org/abs/2404.15743)

  **Authors:** Xiang Gao, Yuqi Zhang

  **Introduction (English):** To address the issues of unbalanced style-content integration and neglect of salient regions in Chinese ink-wash painting style transfer, this paper proposes SRAGAN, a saliency-regularized and attended GAN. It introduces a saliency detection module to identify key content regions, designs an attention mechanism to focus on style feature alignment in salient areas, and adds a saliency regularization loss to preserve the structural integrity of important content. The method achieves high-quality style transfer that balances ink-wash artistic characteristics with content saliency, generating natural and authentic Chinese ink-wash paintings.

- **ChipGAN: A Generative Adversarial Network for Chinese Ink Wash Painting Style Transfer** [Proc. 26th ACM Int. Conf. Multimed. 2018] [[paper\]](https://dl.acm.org/doi/10.1145/3240508.3240655)

  **Authors:** Bin He, Feng Gao, Daiqian Ma, Boxin Shi, Ling-Yu Duan

  **Introduction (English):** To address the challenge of capturing the unique artistic characteristics (e.g., dry/wet brushwork, ink diffusion, and sparse composition) of Chinese ink wash paintings in style transfer, this paper proposes ChipGAN. It designs a two-stage generation framework: the first stage generates a base ink wash painting via a global style transfer module, and the second stage refines local details using a chip-based enhancement module to simulate realistic brush textures and ink gradations. The method effectively reproduces the artistic essence of Chinese ink wash paintings, achieving high-quality style transfer from natural images to ink wash art.

- **Fast Style Transfer for Chinese Traditional Ink Painting** [IEEE Int. Conf. Electron. Inf. Emerg. Commun. (ICEIEC) 2019] [[paper\]](https://ieeexplore.ieee.org/document/8784632)

  **Authors:** Renjie Zhou, Jeong Hoon Han, Hyeon Seok Yang, Woojin Jeong, Young Shik Moon

  **Introduction (English):** To address the inefficiency of existing style transfer methods for Chinese traditional ink painting, this paper proposes a fast style transfer approach. It optimizes the network architecture by simplifying feature extraction layers and adopting lightweight normalization modules, enabling real-time style transfer while preserving core ink painting characteristics (e.g., ink gradation, brush texture). The method balances efficiency and artistic quality, providing a practical solution for real-time ink painting style conversion applications.

- **Image-Based Rendering for Ink Painting** [IEEE Int. Conf. Syst. Man Cybern. 2013] [[paper\]](https://ieeexplore.ieee.org/document/6722427)

  **Authors:** Lingyu Liang, Lianwen Jin

  **Introduction (English):** To realize realistic ink painting rendering from input images, this paper proposes an image-based method integrating artistic feature extraction and style simulation. It extracts structural contours and tonal information from images, models key ink painting effects (e.g., ink wash gradation, brushstroke texture) via adaptive filtering and texture mapping, and achieves natural integration of image content with ink painting artistic style. The method provides an efficient and practical approach for ink painting-style image generation.

- **State of the "Art": A Taxonomy of Artistic Stylization Techniques for Images and Video** [IEEE Trans. Vis. Comput. Graph. 2013] [[paper\]](https://ieeexplore.ieee.org/document/6243138)

  **Authors:** Jan Eric Kyprianidis, John Collomosse, Tinghuai Wang, Tobias Isenberg

  **Introduction (English):** To systematically summarize the progress of artistic stylization techniques for images and video, this paper presents a comprehensive taxonomy. It classifies existing methods into multiple categories (e.g., image filtering, texture synthesis, shape-based methods, deep learning-based approaches) based on technical principles and artistic goals, analyzes the advantages, limitations, and application scenarios of each category, and discusses key challenges such as style authenticity, real-time performance, and content-style balance. The taxonomy provides a structured overview of the field, serving as a reference for researchers and guiding future developments in artistic stylization.

- **Enhancing Digital Chinese Painting in Interior Design with Deep Learning and Virtual Reality** [CAD Comput. Graph. (CADAPS) 2024] [[paper\]](https://cad-journal.net/files/vol_21/CAD_21(S16)_2024_163-177.pdf)

  **Authors:** Ye Ping, He Jie

  **Introduction (English):** To explore the application value of digital Chinese painting in interior design, this paper first clarifies the internal connection between interior space art and the aesthetic spirit of Chinese painting artistic conception, laying a theoretical foundation for modern indoor space atmosphere construction. It combines deep learning to analyze the application of Chinese painting in interior design, comprehensively considers equipment and software selection based on system construction goals (including hardware platform, software platform, and development tools), and constructs an interior design system based on deep learning. Research shows that Chinese painting can play an important role in interior design, effectively improving design effects, and deep learning serves as an effective evaluation method for this application.

#### 2.4 Restoration and Enhancement Guided by Color Semantics

- **Computer-Aided Rendering of Chinese Meticulous Figure Paintings** [J. Comput. Aided Des. Comput. Graph. 2015] [[paper\]](https://www.jcad.cn/en/article/id/cc99922c-42bf-4006-92f3-c78a871b1c4a)

  **Authors:** Ding Xiaoqiang, Hu Taocheng, Peng Ren, Yu Jinhui

  **Introduction (English):** Chinese meticulous figure painting is a traditional art form characterized by fine detail depiction, but manual coloring is tedious and time-consuming. To address this, this paper proposes a computer-aided rendering algorithm that accelerates the coloring process while retaining the artistic style of meticulous figure paintings. The method first interactively extracts contour lines and segments regions (face, hair, limbs, clothes). For the face, interactive auxiliary lines specify light/dark areas, and an iterative dampened-spring diffuser generates grayscale shading. For limbs and clothes, an automatic shading rendering method is adopted. For hair, hand-drawn lines are treated as high-frequency components, smoothed with a Gaussian filter to obtain low-frequency components, and blended for the final effect. Small parts (e.g., headwear) are processed via simple interactions. Experimental results show satisfactory rendering effects consistent with manual works.

- **ConvSRGAN: super-resolution inpainting of traditional Chinese paintings** [Heritage Sci. 2024] [[paper\]](https://www.nature.com/articles/s40494-024-01279-1)

  **Authors:** Qiyao Hu, Xianlin Peng, Tengfei Li, Xiang Zhang, Jiangpeng Wang, Jinye Peng

  **Introduction (English):** Traditional Chinese paintings (TCPs) often suffer from degradation (e.g., blurring, noise, missing regions) due to aging and improper preservation, posing challenges to cultural heritage protection. To address the dual demands of super-resolution (SR) and inpainting for degraded TCPs, this paper proposes ConvSRGAN, a specialized framework integrating convolution neural networks and generative adversarial networks. It designs a multi-scale feature fusion module to enhance detail recovery, adopts a hybrid loss function (including perceptual loss and adversarial loss) to preserve TCP artistic styles (e.g., brushwork, ink wash), and realizes simultaneous SR and inpainting. Experimental results on degraded TCP datasets demonstrate that the method outperforms existing approaches in both visual quality and quantitative metrics, effectively restoring degraded TCPs while retaining their inherent artistic characteristics.

- **Virtual restoration of ancient Chinese paintings using color contrast enhancement and lacuna texture synthesis** [IEEE Trans. Image Process. 2004] [[paper\]](https://ieeexplore.ieee.org/document/1278364)

  **Authors:** SooChang Pei, YiChong Zeng, ChingHua Chang

  **Introduction (English):** Ancient Chinese paintings are prone to color fading, contrast reduction, and lacuna (missing region) formation due to aging and environmental factors, threatening cultural heritage preservation. To address these issues, this paper proposes a virtual restoration method integrating color contrast enhancement and lacuna texture synthesis. It first applies a adaptive color contrast enhancement algorithm to recover faded colors and improve visual clarity. For lacuna regions, a texture synthesis technique based on neighboring valid texture information is adopted to fill missing areas naturally, ensuring consistency with surrounding artistic styles (e.g., brushwork, color tone). The method achieves effective virtual restoration of degraded ancient Chinese paintings, preserving their historical and artistic value.

- **Image Recovery for Ancient Chinese Paintings** [Int. J. Signal Process. Image Process. Pattern Recognit. 2013] [[paper\]](https://www.researchgate.net/publication/269585792_Image_Recovery_for_Ancient_Chinese_Paintings)

  **Authors:** Fan Guo, Jin Tang, Hui Peng

  **Introduction (English):** Ancient Chinese paintings suffer from degradation due to pigment fading and paper aging, affecting their visual quality and cultural value. To address this, this paper proposes a new virtual recovery method for electronic versions of ancient Chinese paintings. The method first uses a guided filter to enhance the original image. Then, a novel bi-extracting method is adopted to separate semi-transparent strokes (foreground) from the painting background: saliency detection and pseudo-alpha matting generate two independent maps, which are fused to represent the foreground strokes. Finally, the ancient painting image is recovered by adjusting the background color. Experiments on various ancient Chinese paintings verify the robustness and accuracy of the proposed method.

- **MCCFNet: Multi-channel Color Fusion Network For Cognitive Classification of Traditional Chinese Paintings** [Cogn. Comput. 2023] [[paper\]](https://link.springer.com/article/10.1007/s12559-023-10172-1)

  **Authors:** Jing Geng, Xin Zhang, Yijun Yan, Meijun Sun, Huiyuan Zhang, Maher Assaad, Jinchang Ren, Xiaoquan Li

  **Introduction (English):** Cognitive classification of traditional Chinese paintings (TCPs) is crucial for cultural heritage management and artistic research, but existing methods often ignore the unique color characteristics and multi-dimensional semantic information of TCPs. To address this, this paper proposes MCCFNet, a multi-channel color fusion network. It designs a multi-channel color feature extraction module to capture color information from different color spaces (e.g., RGB, HSV, Lab), integrates a cross-attention fusion mechanism to enhance the interaction between color features and semantic features, and adopts a hierarchical classification strategy to realize fine-grained classification of TCPs (e.g., style, theme, dynasty). Experiments on TCP datasets demonstrate that the method outperforms existing classification models in accuracy and robustness, providing an effective solution for cognitive classification of TCPs.

- **Supervised Heterogeneous Sparse Feature Selection for Classification and Prediction of Chinese Paintings** [J. Comput. Aided Des. Comput. Graph. 2013] [[paper\]](https://www.jcad.cn/article/id/ae57289e-7ce1-4dfd-9ad8-02e3bfd57d51)

  **Authors:** Wang Zheng, Sun Meijun, Han Yahong, Zhang Dong

  **Introduction (English):** Classification and prediction of Chinese paintings rely on effective feature extraction from heterogeneous data (e.g., texture, color, shape, semantic information), but existing methods suffer from redundant features and low computational efficiency. To address this, this paper proposes a supervised heterogeneous sparse feature selection method. It integrates multiple heterogeneous features of Chinese paintings, introduces a sparse regularization term to select discriminative features while eliminating redundancy, and leverages supervised information to enhance the correlation between selected features and classification/prediction tasks (e.g., style identification, author attribution). Experimental results show that the method improves classification and prediction accuracy while reducing feature dimensionality, providing an efficient feature selection solution for Chinese painting analysis.

- **Intelligent Classification Method of Basic Elements of Chinese Ink Painting Based on a Convolution Neural Network** [IEEE Int. Conf. Ind. Appl. Artif. Intell. (IAAI) 2021] [[paper\]](https://ieeexplore.ieee.org/document/9699884?denied=)

  **Author:** Liu Yang

  **Introduction (English):** The basic elements of Chinese ink painting (e.g., lines, dots, strokes, textures) are the core of its artistic expression, and their accurate classification is crucial for style analysis and digital creation. To address the inefficiency and subjectivity of manual classification, this paper proposes an intelligent classification method based on a convolution neural network (CNN). It constructs a dataset of basic ink painting elements, designs a lightweight CNN architecture to extract discriminative features (e.g., shape, texture, structural characteristics) of elements, and optimizes the network with transfer learning to improve classification accuracy with limited data. Experimental results demonstrate that the method achieves high-precision and efficient classification of basic ink painting elements, providing technical support for intelligent analysis and digital inheritance of Chinese ink painting.

- **The Application of Hyperpixel Segmentation Algorithm in Chinese Painting** [J. Radiat. Res. Appl. Sci. 2024] [[paper\]](https://www.sciencedirect.com/science/article/pii/S1687850724000888)

  **Author:** Xie Shupei

  **Introduction (English):** Segmentation of Chinese painting elements (e.g., figures, landscapes, brushstrokes) is a key step for digital analysis, restoration, and creation, but traditional pixel-level segmentation methods struggle with blurred boundaries and inconsistent texture integration. To address this, this paper proposes the application of a hyperpixel segmentation algorithm in Chinese painting. Hyperpixel segmentation groups adjacent pixels with similar features (color, texture, structure) into meaningful hyperpixel units, which better align with the artistic integrity of Chinese painting elements. The method enhances boundary accuracy and reduces segmentation noise, facilitating subsequent tasks such as element extraction, style analysis, and digital modification. Experimental results verify the effectiveness of hyperpixel segmentation in Chinese painting processing, providing a more refined tool for digital analysis of traditional Chinese art.

- **Edge-Aware Image Super-Resolution Using a Generative Adversarial Network** [SN Comput. Sci. 2023] [[paper\]](https://link.springer.com/article/10.1007/s42979-022-01561-8)

  **Authors:** Bishshoy Das, Sumantra Dutta Roy

  **Introduction (English):** Image super-resolution (SR) often suffers from edge blurring and detail loss, especially for images with complex structural features. To address this, this paper proposes an edge-aware GAN-based SR method. It integrates an edge detection module to extract and emphasize structural edge information, designs a generator with edge-preserving feature fusion blocks to enhance edge recovery, and adopts an adversarial loss combined with edge loss to optimize the network. The method achieves high-quality SR with sharp edges and rich details, outperforming traditional and mainstream GAN-based SR approaches in both visual quality and quantitative metrics (e.g., PSNR, SSIM). It provides an effective solution for edge-sensitive SR tasks, such as cultural heritage image restoration (including Chinese paintings) and high-definition content generation.

- **Virtual Restoration of Stains on Ancient Paintings with Maximum Noise Fraction Transformation Based on Hyperspectral Imaging** [J. Cult. Heritage 2018] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S1296207417305708)

  **Authors:** Miaole Hou, Pingping Zhou, Shuqiang Lv, Yungang Hu, Xuesheng Zhao, Wangting Wu, Haiping He, Songnian Li, Li Tan

  **Introduction (English):** Stains on ancient paintings (e.g., mold, dust, watermarks) severely affect their visual quality and cultural value, but traditional restoration methods are often invasive or ineffective for subtle stains. To address this, this paper proposes a virtual restoration method for stains on ancient paintings based on hyperspectral imaging and maximum noise fraction (MNF) transformation. Hyperspectral imaging captures rich spectral information to distinguish stains from the original painting layers, while MNF transformation effectively separates noise (stain-related components) from useful signals (painting content). The method achieves non-invasive and precise stain removal, preserving the original texture, color, and artistic details of ancient paintings. Experiments on stained ancient painting samples demonstrate the method's effectiveness and robustness, providing a reliable technical tool for cultural heritage preservation.

### 3. Spatial Governance: Relational Modeling and Layout Reasoning

#### 3.1 Foundation: Geometric and Semantic Parsing of Visual Scenes

- **Simulation of Chinese Ink-Wash Painting Based on Landscapes and Trees** [Int. Symp. Plant Growth Model. Appl. 2006] [[paper\]](https://ieeexplore.ieee.org/document/4548391)

  **Authors:** Xunxiang Li, Yu Li

  **Introduction (English):** Simulating the artistic characteristics of Chinese ink-wash landscape paintings (e.g., tree modeling, ink wash gradation, sparse composition) is a key task in digital art. To address the lack of realism in traditional geometric modeling-based simulation methods, this paper proposes a specialized simulation approach for landscape and tree elements in Chinese ink-wash painting. It integrates natural growth rules of trees with artistic expression of ink-wash painting, designs a parametric model to generate tree structures (trunks, branches, leaves) consistent with ink-wash brushwork, and simulates ink diffusion and dry/wet brush effects via texture synthesis and alpha blending. The method realizes realistic simulation of ink-wash landscape paintings, providing a technical foundation for digital creation and inheritance of Chinese ink-wash art.

- **A Depth-Estimation-Based Method for Multi-View Synthesis Applied to Chinese Landscape Paintings** [Appl. Soft Comput. 2025] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S1568494625011718)

  **Authors:** Xianlin Peng, Wanlin Zhou, Qiyao Hu, Tengfei Li, Dong Zhang, Rui Cao

  **Introduction (English):** Chinese landscape paintings often convey implicit spatial depth through artistic techniques (e.g., layer composition, perspective processing), but multi-view synthesis for such paintings remains challenging due to the lack of explicit depth information. To address this, this paper proposes a depth-estimation-based multi-view synthesis method. It first designs a depth estimation network specialized for Chinese landscape paintings, which infers spatial depth from artistic features (e.g., ink wash gradation, object overlapping, size variation). Then, a multi-view generation module uses the estimated depth map to synthesize realistic multi-angle views while preserving the original artistic style and spatial logic. Experimental results demonstrate that the method generates natural and consistent multi-view images of Chinese landscape paintings, providing a new technical approach for digital display, virtual appreciation, and cultural heritage dissemination.

- **Video-based Running Water Animation in Chinese Painting Style** [Sci. China Ser. F: Inf. Sci. 2009] [[paper\]](https://link.springer.com/article/10.1007/s11432-009-0035-7)

  **Authors:** Zhang SongHai, Chen Tao, Zhang YiFei, Hu ShiMin, Ralph Martin

  **Introduction (English):** Animating natural elements like running water in Chinese painting style is crucial for dynamic digital expression of traditional art, but existing methods struggle to balance fluid motion realism with ink-wash artistic characteristics. To address this, this paper proposes a video-based running water animation method. It extracts motion features of real running water from video footage, models fluid dynamics combined with Chinese painting brushwork rules, and adopts texture synthesis and ink diffusion simulation to render water flows with ink-wash style (e.g., light/dark ink gradation, dynamic brush strokes). The method realizes vivid running water animation consistent with Chinese painting aesthetics, providing a technical solution for dynamic digital creation of traditional Chinese art.

#### 3.2 Representation: Modeling Relational Priors and Scene Graphs

- **Improved Watershed Image Segmentation Method Based on Adaptive Structural Elements** [J. Harbin Inst. Technol. 2023] [[paper\]](https://hit.alljournals.cn/html/hitxb_cn/2023/5/20230507.html)

  **Authors:** Chao Fang, Xiaopeng Wang, Baomin Li, Weiwei Fan

  **Introduction (English):** Image segmentation is a key link between image processing and analysis, but traditional watershed segmentation methods are prone to over-segmentation and edge information loss due to noise interference. To address these issues, this paper proposes an improved watershed segmentation method based on adaptive structural elements. First, adaptive structural elements with variable shapes are constructed using local density, symmetry, and boundary features of adjacent pixels, ensuring consistency with target shapes. Second, these elements are used to compute the morphological gradient, improving edge positioning accuracy. The gradient image is modified via L0 norm gradient minimization and morphological open-close hybrid reconstruction to reduce invalid local minima and suppress over-segmentation. Finally, watershed segmentation is performed on the modified gradient image. Experiments show the method effectively restrains over-segmentation, enhances edge positioning accuracy, and achieves high-precision image segmentation, which can be applied to target extraction and analysis of Chinese paintings.

- **CCLAP: Controllable Chinese Landscape Painting Generation via Latent Diffusion Model** [arXiv 2023] [[paper\]](https://arxiv.org/abs/2304.04156)

  **Authors:** Zhongqi Wang, Jie Zhang, Zhilong Ji, Jinfeng Bai, Shiguang Shan

  **Introduction (English):** Controllable generation of Chinese landscape paintings (CLPs) is challenging due to their unique artistic characteristics (e.g., ink wash gradation, freehand brushwork, spatial composition) and the need for fine-grained control over creative elements. To address this, this paper proposes CCLAP, a controllable generation method based on latent diffusion models (LDMs). It introduces a CLP-specific latent space optimization to capture artistic style features, designs multi-modal control modules (e.g., sketch, text, color palette) to enable precise control over composition, content, and style, and integrates a style consistency constraint to preserve the inherent aesthetic of CLPs. Experimental results demonstrate that CCLAP generates high-quality, stylistically consistent CLPs with flexible controllability, providing a new tool for digital creation and cultural heritage inheritance of Chinese landscape painting.

- **A Generative Approach to Chinese Shanshui Painting** [IEEE Comput. Graph. Appl. 2017] [[paper\]](https://ieeexplore.ieee.org/document/7819408)

  **Author:** Shi Weili

  **Introduction (English):** Chinese shanshui (landscape) painting features unique artistic expressions (e.g., freehand brushwork, layered composition, ink wash gradation), making generative modeling a significant challenge. To address this, this paper proposes a generative approach tailored for Chinese shanshui painting. It integrates artistic rules of shanshui painting (e.g., spatial layout principles, brushstroke techniques) with procedural generation algorithms, designs a hierarchical modeling framework to generate core elements (mountains, rivers, trees, pavilions) sequentially, and simulates ink diffusion and texture variation via parameterized models. The method realizes automatic generation of shanshui paintings with authentic artistic style, providing a practical tool for digital creation and art education.

- **Measuring and Evaluating the Visual Complexity of Chinese Ink Paintings** [Comput. J. 2021] [[paper\]](https://academic.oup.com/comjnl/article-abstract/65/8/1964/6278154?redirectedFrom=fulltext)

  **Authors:** Zhen-Bao Fan, Yi-Na Li, Kang Zhang, Jinhui Yu, Mao Lin Huang

  **Introduction (English):** Visual complexity is a key aesthetic attribute of Chinese ink paintings, influencing artistic appreciation and digital analysis, but systematic measurement and evaluation methods are lacking. To address this, this paper proposes a quantitative framework for measuring the visual complexity of Chinese ink paintings. It extracts multi-dimensional features (e.g., brushstroke density, texture variation, spatial composition, ink wash gradation) that reflect visual complexity, designs a weighted evaluation model to integrate these features, and validates the framework through subjective user experiments and objective statistical analysis. The method achieves consistent and reliable evaluation of visual complexity, providing a theoretical basis and technical tool for aesthetic research, digital classification, and creative guidance of Chinese ink paintings.

- **Knowledge Association and Semantic Description of "Meta-Painting" Works: A Case Study of Ming Dynasty "Meta-Painting"** [Library J. 2023] [[paper\]](https://lib.cqvip.com/Qikan/Article/Detail?id=7111374495)

  **Authors:** Zang Zhidong, Sui Chenglong, Cheng Jiejing

  **Introduction (English):** "Meta-painting" is a special artistic form that reflects on painting itself through artistic expression, and the Ming Dynasty meta-painting works have important academic value in art history research. However, existing research lacks systematic knowledge association and standardized semantic description, which hinders the in-depth excavation of their cultural connotations. To address this, this paper takes Ming Dynasty meta-painting as the research object, constructs a knowledge association framework covering artistic elements, historical context, and academic comments, and establishes a semantic description system based on metadata standards. Through case analysis, the method realizes the structured organization and effective expression of meta-painting knowledge, providing a theoretical reference and technical support for the digital management, academic research, and cultural inheritance of traditional Chinese meta-painting works.

#### 3.3 Reasoning: Knowledge-Informed Spatial Logic and Function

- **A Virtual Restoration Network of Ancient Murals via Global–Local Feature Extraction and Structural Information Guidance** [Heritage Sci. 2023] [[paper\]](https://www.nature.com/articles/s40494-023-01109-w)

  **Authors:** Ge Hao, Yu Ying, Zhang Le

  **Introduction (English):** Ancient murals are valuable cultural heritage but suffer from degradation (e.g., cracks, fading, missing regions) due to natural and human factors. Traditional virtual restoration methods often fail to balance global style consistency and local detail fidelity. To address this, this paper proposes a virtual restoration network for ancient murals. It designs a global–local feature extraction module to capture overall artistic style (e.g., color tone, brushwork) and local texture details simultaneously, integrates structural information guidance (e.g., edge, contour) to maintain the mural's inherent structural logic, and adopts a hybrid loss function to optimize both visual quality and historical authenticity. Experimental results on degraded mural datasets demonstrate that the method outperforms existing approaches in restoration effect, preserving the mural's cultural and artistic value while achieving natural and consistent restoration.

- **Traditional Landscape Painting and Art Image Restoration Methods Based on Structural Information Guidance** [J. Intell. Syst. 2024] [[paper\]](https://www.degruyterbrill.com/document/doi/10.1515/jisys-2024-0058/html?srsltid=AfmBOoor9RbxscNLZS3CJ_HseXBTxnqUJLRMBxsyQAPpKQ1yMkzL5Qc9)

  **Author:** Yao Zhimin

  **Introduction (English):** Traditional landscape paintings (including Chinese landscape paintings) are prone to structural damage (e.g., contour blurring, shape distortion) and detail loss due to aging and preservation issues, affecting their artistic and historical value. Existing restoration methods often focus on texture and color recovery while ignoring structural integrity. To address this, this paper proposes an art image restoration method for traditional landscape paintings based on structural information guidance. It first extracts structural features (e.g., contours, spatial layout, brushstroke logic) of landscape paintings via edge detection and structural analysis, then designs a guided restoration framework that uses structural information to constrain texture and color recovery, ensuring consistency between restored details and the original structural logic. Experimental results show the method effectively restores structural integrity and detail fidelity of traditional landscape paintings, providing a reliable technical approach for cultural heritage protection.

- **Sgrgan: Sketch-Guided Restoration for Traditional Chinese Landscape Paintings** [Heritage Sci. 2024] [[paper\]](https://www.nature.com/articles/s40494-024-01253-x)

  **Authors:** Qiyao Hu, Weilu Huang, Yinyin Luo, Rui Cao, Xianlin Peng, Jinye Peng, Jianping Fan

  **Introduction (English):** Traditional Chinese landscape paintings (TCLPs) often suffer from degradation (e.g., blurring, noise, missing regions) due to aging and improper preservation, and existing restoration methods lack effective structural constraint, leading to inconsistent restoration of artistic elements (e.g., mountains, trees, brushstrokes). To address this, this paper proposes Sgrgan, a sketch-guided restoration framework for TCLPs. It first extracts structural sketches from degraded TCLPs (or uses user-provided sketches) to capture core structural information (e.g., contour, spatial layout, brushstroke direction). Then, a sketch-guided generator integrates sketch features with image features to constrain restoration, ensuring consistency between restored content and original structure. A hybrid loss function (adversarial loss, perceptual loss, sketch consistency loss) is adopted to preserve TCLP artistic styles (e.g., ink wash gradation, texture) while maintaining structural integrity. Experimental results on degraded TCLP datasets demonstrate that Sgrgan outperforms existing methods in visual quality and structural consistency, effectively restoring degraded TCLPs while retaining their inherent artistic value.

- **High-Resolution Restoration of Ancient Chinese Paintings Based on Line Structure Decomposition** [J. Comput. Aided Des. Comput. Graph. 2018] [[paper\]](https://www.researchgate.net/publication/328487848_Repairing_High-Definition_Ancient_Paintings_Based_on_Decomposition_of_Curves)

  **Authors:** Ma Wei, Long Qingqing, Qin Yue, Xu Shibiao, Zhang Xiaopeng

  **Introduction (English):** High-resolution ancient Chinese paintings often suffer from line structure damage (e.g., blurring, breakage, fading) due to aging, which severely affects their artistic expression and historical value. Existing high-resolution restoration methods fail to fully consider the unique line structure characteristics of Chinese paintings, leading to unsatisfactory restoration effects. To address this, this paper proposes a high-resolution restoration method for ancient Chinese paintings based on line structure decomposition. It first decomposes the painting into line structure layers and texture color layers, extracts and repairs damaged line structures using curve fitting and shape optimization techniques, and then fuses the repaired line structures with the texture color layers to generate high-resolution restored images. The method effectively preserves the integrity and authenticity of the line structures of ancient Chinese paintings while improving the clarity and quality of the restored images. Experimental results demonstrate the effectiveness and superiority of the proposed method in high-resolution restoration of ancient Chinese paintings.

#### 3.4 Synthesis: Computational Aesthetics and Goal-Directed Layout Generation

- **Progressive Artistic Aesthetic Enhancement for Chinese Ink Painting Style Transfer** [InBook 2024] [[paper\]](https://ebooks.iospress.nl/doi/10.3233/FAIA240557)

  **Author:** Chihan Huang

  **Introduction (English):** Chinese ink painting style transfer aims to render content images with the unique artistic characteristics of ink painting (e.g., ink wash gradation, freehand brushwork, sparse composition), but existing methods often lack sufficient aesthetic enhancement and fail to capture the subtle artistic nuances. To address this, this paper proposes a progressive artistic aesthetic enhancement method for Chinese ink painting style transfer. It designs a multi-stage progressive framework: first extracting content and style features, then iteratively enhancing artistic elements (e.g., brushstroke texture, ink diffusion, spatial layout) based on aesthetic rules of Chinese ink painting, and finally optimizing the overall visual harmony. The method integrates aesthetic evaluation metrics to guide the enhancement process, ensuring the transferred images not only retain content integrity but also possess authentic ink painting aesthetic qualities. Experimental results demonstrate that the method outperforms existing style transfer approaches in artistic expression and aesthetic satisfaction, providing a more refined tool for digital creation of Chinese ink painting style.

- **Hierarchical Painter: Chinese Landscape Painting Restoration with Fine-Grained Styles** [Vis. Intell. 2023] [[paper\]](https://link.springer.com/article/10.1007/s44267-023-00021-y)

  **Authors:** Zhekai Xu, Haohong Shang, Shaoze Yang, Ruiqi Xu, Yichao Yan, Yixuan Li, Jiawei Huang, Howard C. Yang, Jianjun Zhou

  **Introduction (English):** Chinese landscape paintings feature diverse fine-grained styles (e.g., Northern/Southern School, freehand/meticulous brushwork) that are critical to their artistic value, but existing restoration methods often ignore style granularity, leading to inconsistent style expression in restored regions. To address this, this paper proposes Hierarchical Painter, a restoration method for Chinese landscape paintings with fine-grained style awareness. It constructs a hierarchical style feature extraction framework to capture both global style categories and local fine-grained style details (e.g., brushstroke thickness, ink concentration). A style-aware restoration generator uses these hierarchical features to constrain the restoration process, ensuring that restored regions match the original fine-grained style. Additionally, a style consistency loss is designed to maintain style uniformity across the entire painting. Experimental results demonstrate that Hierarchical Painter achieves high-fidelity restoration while preserving fine-grained style characteristics, outperforming existing methods in style consistency and artistic authenticity.

- **Traditional Chinese Painting Instance Segmentation Algorithm Based on Integrating Spatial Structure Characteristics** [J. China Univ. Posts Telecommun. 2025] [[paper\]](https://jcupt.bupt.edu.cn/EN/10.19682/j.cnki.1005-8885.2025.0015)

  **Authors:** Diao Haiyang, Hou Xiaogang, Li Huabiao, Yang Jiaxin

  **Introduction (English):** Instance segmentation of Traditional Chinese Paintings (TCPs) is essential for digital analysis and creative applications, but existing algorithms struggle to capture the unique spatial structure characteristics of TCPs (e.g., scattered composition, flexible brushstroke layout, implicit spatial hierarchy), leading to inaccurate instance localization and ambiguous boundaries. To address this, this paper proposes an instance segmentation algorithm for TCPs by integrating spatial structure characteristics. It designs a spatial structure feature extraction module to capture hierarchical spatial relationships (e.g., foreground-background layout, inter-instance overlapping logic) and structural constraints of TCP elements (e.g., strokes, objects). The module fuses spatial structure features with appearance features (color, texture) to enhance instance discriminability. A refined segmentation head with boundary-aware loss is adopted to optimize edge precision and instance consistency. Experimental results on TCP datasets demonstrate that the method outperforms mainstream instance segmentation algorithms in segmentation accuracy and structural coherence, providing effective technical support for TCP digital analysis, element extraction, and style reconstruction.

- **DRANet: A Semantic Segmentation Network for Chinese Landscape Paintings** [Digit. Signal Process. 2024] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S1051200424000526)

  **Authors:** QiYao Hu, Wanlin Zhou, Xianlin Peng, Xiang Zhang, Penglin Xie, Yuzhe Liu, Jinye Peng, Jianping Fan

  **Introduction (English):** Semantic segmentation of Chinese landscape paintings (CLPs) is critical for digital analysis, restoration, and creation, but existing semantic segmentation networks fail to account for CLPs' unique artistic characteristics (e.g., abstract brushwork, ink wash gradation, implicit semantic boundaries). This leads to low segmentation accuracy and ambiguous semantic classification of core elements (mountains, rivers, trees, pavilions). To address this, this paper proposes DRANet, a specialized semantic segmentation network for CLPs. It designs a dual-branch feature extraction module to capture both appearance features (color, texture) and structural features (brushstroke direction, spatial layout) of CLPs. A semantic relation attention module is integrated to model contextual dependencies between CLP elements, enhancing semantic discriminability. Additionally, a boundary refinement loss is adopted to optimize semantic boundary clarity. Experimental results on CLP datasets demonstrate that DRANet outperforms mainstream semantic segmentation networks in segmentation precision and semantic consistency, providing a reliable technical tool for CLP digital processing and cultural heritage protection.

- **A Novel Automatic Image Segmentation Method for Chinese Literati Paintings Using Multi-View Fuzzy Clustering Technology** [Multimedia Syst. 2020] [[paper\]](https://link.springer.com/article/10.1007/s00530-019-00627-7)

  **Authors:** Zhang Jie, Zhou Yintao, Xia Kaijian, Jiang Yizhang, Liu Yuan

  **Introduction (English):** Chinese literati paintings feature unique artistic characteristics (e.g., freehand brushwork, sparse composition, ink wash gradation) and implicit semantic boundaries, making automatic image segmentation a challenging task. Traditional segmentation methods rely on single-view features, leading to insufficient feature representation and inaccurate segmentation of literati painting elements. To address this, this paper proposes a novel automatic segmentation method using multi-view fuzzy clustering technology. It extracts multi-view features (color, texture, structural shape) from Chinese literati paintings to comprehensively characterize image content, designs a weighted feature fusion strategy to balance the contribution of different views, and applies fuzzy clustering to achieve automatic segmentation of artistic elements (e.g., figures, landscapes, calligraphy). The method effectively handles the ambiguity and abstraction of literati paintings, improving segmentation accuracy and semantic consistency. Experimental results demonstrate the superiority of the proposed method over traditional single-view clustering and mainstream segmentation algorithms, providing a technical foundation for digital analysis and inheritance of Chinese literati paintings.

- **Special Perceptual Parsing for Chinese Landscape Painting Scene Understanding: A Semantic Segmentation Approach** [Neural Comput. Appl. 2023] [[paper\]](https://link.springer.com/article/10.1007/s00521-023-09343-w)

  **Authors:** Yang Rui, Yang Honghong, Zhao Min, Jia Ru, Wu Xiaojun, Zhang Yumei

  **Introduction (English):** Scene understanding of Chinese landscape paintings (CLPs) relies on accurate semantic segmentation of artistic elements, but CLPs' unique perceptual characteristics (e.g., abstract brushwork, ink wash gradation, implicit spatial relationships) pose challenges to mainstream semantic segmentation methods, leading to poor parsing of artistic semantics. To address this, this paper proposes a special perceptual parsing approach for CLP scene understanding. It designs a CLP-specific semantic segmentation network that integrates perceptual feature enhancement modules to capture artistic texture (e.g., dry/wet brush strokes) and semantic context (e.g., element co-occurrence rules). A multi-scale feature fusion strategy is adopted to handle the scale variation of CLP elements, and a perceptual consistency loss is introduced to align segmentation results with human artistic perception. Experimental results on CLP datasets demonstrate that the method outperforms mainstream semantic segmentation approaches in semantic parsing accuracy and perceptual consistency, enabling effective scene understanding for CLP digital analysis, restoration, and creative applications.

- **An Image Segmentation Method for Chinese Paintings by Combining Deformable Models with Graph Cuts** [HCI 2011, LNCS 6761] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-642-21602-2_62)

  **Authors:** Ning He, Ke Lu

  **Introduction (English):** Image segmentation of Traditional Chinese Paintings (TCPs) is crucial for element extraction and digital analysis, but existing graph-based methods often require trimap inputs, are time-consuming, or only rely on color information. To address these issues, this paper proposes a fast segmentation method combining deformable models and graph cuts. First, it integrates deformable model information and explicit edge information into a graph cuts optimization framework to roughly segment TCPs into foreground and background. Then, belief propagation (BP) is used to estimate opacity values of boundary pixels. Finally, texture information is introduced by constructing co-occurrence matrices of TCP images. Experiments show the method is efficient and effective for TCP segmentation, overcoming the limitations of traditional graph-based approaches.

### 4. Structural Brushwork: Structure-Preserving Stroke Modeling

#### 4.1 Physically-Based Modeling of Brush–Ink–Paper Dynamics

- **Hairy Brushes** [SIGGRAPH Comput. Graph. 1986] [[paper\]](https://dl.acm.org/doi/10.1145/15886.15911)

  **Author:** Steve Strassmann

  **Introduction (English):** To solve the problem that traditional digital modeling fails to simulate natural brush strokes, this paper proposes the "hairy brush" model. It represents brushes as discrete flexible bristles with physical properties, simulates dynamic interactions between bristles, ink, and canvas, and generates realistic and varied strokes. This work lays a foundation for digital painting brush simulation and influences non-photorealistic rendering research, including Chinese ink wash brushwork simulation.

- **Simulating Oriental Black-Ink Painting** [IEEE Comput. Graph. Appl. 1999] [[paper\]](https://ieeexplore.ieee.org/document/761553)

  **Author:** J. Lee

  **Introduction (English):** Traditional oriental black-ink painting simulation often relies on spline curve editing, resulting in unnatural strokes. To address this, this paper proposes an interactive modeling algorithm for "soft brushes" that respond elastically to pressure. The model supports brush resizing, and selection of color, texture, and bristle type, generating 3D visual effects through elastic bristle deformation—key for authentic black-ink painting. It enables users to create strokes via natural brush movement, avoiding unnatural editing and enhancing the realism of simulated oriental black-ink art.

- **Diffusion rendering of black ink paintings using new paper and ink models** [Comput. Graph. 2001] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0097849300001321)

  **Author:** Jintae Lee

  **Introduction (English):** To address the challenge of simulating realistic ink diffusion effects in oriental black ink paintings, this paper proposes a novel rendering method based on improved paper and ink models. It constructs fiber mesh paper models (random or uniform) to mimic different paper textures, designs elastic bristle/brush models to generate authentic strokes, and simulates ink diffusion dynamics. The method enables real-time dynamic rendering of ink spreading, reflecting both local temporal variations and global gray tone changes of the paper.

- **An Efficient Physically-Based Model for Chinese Brush** [FAW 2007, LNCS 4613] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-540-73814-5_25)

  **Authors:** Bendu Bai, Kam-Wah Wong, Yanning Zhang

  **Introduction (English):** Conventional Chinese brush simulation relies on bristle-level modeling, leading to high complexity. To address this, this paper proposes an efficient physically-based model. Instead of simulating individual bristles, it uses points to represent the entire brush bundle and a spring network to calculate brush deflection based on internal and external forces. The model captures real brush deformation during interaction with virtual paper, achieving effective and efficient simulation of Chinese brush painting.

- **The Droplet Virtual Brush for Chinese Calligraphic Character Modeling** [WACV 2002] [[paper\]](https://ieeexplore.ieee.org/document/1182203/)

  **Authors:** Xiaofeng Mi, Jie Xu, Min Tang, Jinxiang Dong

  **Introduction (English):** Traditional Chinese calligraphy simulation faces challenges like poor expressive ability of curve-offset methods and complex evaluation of stroke areas in physical solid-model brushes. To solve these, this paper proposes a droplet-based virtual brush model. It uses droplet operations to generate vivid character outlines with clear geometric information, enabling accurate outline retrieval. The model can express various Chinese brush styles simply, overcoming the limitations of previous methods and simplifying stroke area computation.

- **"Nijimi" Rendering Algorithm for Creating Quality Black Ink Paintings** [CGI 2003] [[paper\]](https://ieeexplore.ieee.org/document/1214460)

  **Authors:** Q. Guo, T.L. Kunii

  **Introduction (English):** Simulating the "Nijimi" (ink diffusion) effect is key to authentic Chinese black ink paintings, but existing methods struggle to replicate its natural gradation. This paper proposes a "Nijimi" rendering algorithm that models ink diffusion based on paper texture and ink concentration. It simulates the physical process of ink spreading on porous paper, generating soft, gradual tonal transitions characteristic of "Nijimi". The algorithm enhances the realism of digital black ink paintings by capturing the subtle interplay between ink and paper.

- **Physical-based Model of Ink Diffusion in Chinese Paintings** [Int. Conf. Cent. Eur. Comput. Graph. Vis. 2003] [[paper\]](https://www.researchgate.net/publication/221546314_Physical-based_Model_of_Ink_Diffusion_in_Chinese_Paintings)

  **Authors:** Der-Lor Way, Sheng-Wen Huang, Zen-Chung Shih

  **Introduction (English):** Given the scarcity of research on Chinese ink painting (a three-thousand-year-old non-photorealistic art) and the challenge of simulating complex ink behavior, this paper proposes a physics-based ink diffusion method based on observation and analysis. It can simulate various tone expressions on different paper types, elucidate the mixing effect of strokes from different brushes, and validate the results through comparison with real ink paintings

- **MoXi: Real-Time Ink Dispersion in Absorbent Paper** [ACM Trans. Graph. 2005] [[paper\]](https://dl.acm.org/doi/10.1145/1073204.1073221)

  **Authors:** Nelson S.-H. Chu, Chiew-Lan Tai

  **Introduction (English):** Realistic simulation of ink dispersion on absorbent paper is critical for digital Chinese ink painting but faces challenges of high computational cost and unrealistic effects. This paper proposes MoXi, a physically-based method using the lattice Boltzmann equation to model fluid flow in porous media (paper) in real time. It unifies spontaneous shape evolution and porous media flow simulation, coupling physics with implicit modeling and image-based rendering to generate realistic ink dispersion effects, including complex flow patterns and artistic textures.

- **On the Effects of Haptic Display in Brush and Ink Simulation for Chinese Painting and Calligraphy** [PG 2002] [[paper\]](https://ieeexplore.ieee.org/document/1167892)

  **Authors:** Jeng-sheng Yeh, Ting-yu Lien, Ming Ouhyoung

  **Introduction (English):** Traditional Chinese painting/calligraphy simulation lacks haptic feedback, reducing user immersion. This paper explores integrating haptic display into brush-ink simulation, mapping brush-paper interaction forces (e.g., friction, pressure) to haptic feedback. The system enhances realism by enabling users to perceive physical resistance during virtual painting, addressing the immersion gap in existing simulations.

- **The Synthesis of Rock Textures in Chinese Landscape Painting** [Computer Graphics Forum 2001] [[paper\]](https://onlinelibrary.wiley.com/doi/abs/10.1111/1467-8659.00505)

  **Authors:** Der-Lor Way, Zen-Chung Shih

  **Introduction (English):** Rock textures are crucial in Chinese landscape painting, conveying mountain orientation and atmosphere, with core strokes like hemp-fiber (for gentle slopes) and axe-cut (for hard surfaces). This paper proposes a novel synthesis method for rock textures. Users only need to specify contours and parameters, and the method completes the entire painting process automatically. It is applicable for interactive creation by artists and automated natural scene rendering.

- **Real-time Painting with an Expressive Virtual Chinese Brush** [IEEE Comput. Graph. Appl. 2004] [[paper\]](https://ieeexplore.ieee.org/document/1333630)

  **Authors:** N.S.H. Chu, Chiew-Lan Tai

  **Introduction (English):** Existing digital tools poorly support expressive Chinese brushwork due to inadequate real-time delicate deformation simulation. This paper proposes an efficient 3D deformable virtual Chinese brush model, which simulates realistic bristle behavior via 6-degree-of-freedom input and enables real-time rendering of dynamic brushstrokes on consumer hardware, supporting digital Eastern brush creation and related applications.

- **Intrinsic Feature Preserved Chinese-Painting Style Rendering for 3D Models** [J. Comput. Aided Des. Comput. Graph. 2012] [[paper\]](https://www.jcad.cn/en/article/id/c04e969a-4166-40e0-8b0e-b2c682702698)

  **Authors:** Ji Zhongping, Wang Yigang, Fang Meie, Gao Cheng

  **Introduction (English):** Existing 3D model Chinese-painting style rendering often neglects 3D shape intrinsic features. This paper proposes a non-photorealistic rendering method: calculate and non-linearly transform surface mean curvatures, map them to materials, render to texture via frame buffer object, and apply GPU-based post-processing. Users can adjust light and thresholds for real-time effect editing, achieving efficient and robust rendering while preserving 3D model intrinsic features.

- **Ink Wash Painting Style Rendering With Physically-based Ink Dispersion Model** [J. Phys. Conf. Ser. 2018] [[paper\]](https://iopscience.iop.org/article/10.1088/1742-6596/1004/1/012026)

  **Authors:** Wang Yifan, Li Weiran, Zhu Qing

  **Introduction (English):** For real-time ink wash style rendering of 3D scenes, this paper proposes a GPU-based method. It calculates vertex curvature to render 3D model ink properties, caches them to a paper structure, and simulates ink dispersion via a porous media theory-based model, finally converting ink properties to pixel colors. The method achieves better visual quality than previous approaches.

- **Virtual Hairy Brush for Digital Painting and Calligraphy** [Science in China Ser. F 2005] [[paper\]](https://www.researchgate.net/publication/277373114_Virtual_hairy_brush_for_digital_painting_and_calligraphy)

  **Author:** Songhua Xu

  **Introduction (English):** Existing virtual brush systems struggle to balance user-friendliness, expressiveness, and real-time performance for digital Chinese painting/calligraphy. This paper proposes a novel virtual hairy brush framework based on solid modeling: it uses "writing primitives" (hair clusters) instead of individual bristles to reduce simulation complexity, models brush deformation and ink deposition dynamically, and develops an interactive prototype system. The system enables real-time creation of high-quality digital paintings/calligraphy, addressing the trade-off between realism and efficiency.

#### 4.2 Stroke Structure as Semantic and Visual Primitives

- **Categorizing Traditional Chinese Painting Images** [LNCS 3331, 2004] [[paper\]](https://www.researchgate.net/publication/225138214_Categorizing_Traditional_Chinese_Painting_Images)

  **Authors:** Shuqiang Jiang, Tiejun Huang

  **Introduction (English):** Automatic categorization of Traditional Chinese Painting (TCP) images is essential for digital archiving and retrieval, but TCPs' artistic characteristics (e.g., ink wash textures, abstract brushwork) challenge conventional image classification methods. This paper proposes a categorization approach leveraging TCP-specific features (e.g., ink gradation, brush stroke patterns) and machine learning techniques. It extracts discriminative visual features tailored to TCP styles and trains a classifier to distinguish between major categories (e.g., landscape, figure, flower-and-bird paintings), achieving effective automatic categorization.

- **An Effective Method to Detect and Categorize Digitized Traditional Chinese Paintings** [Pattern Recognit. Lett. 2006] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0167865505003211)

  **Authors:** Shuqiang Jiang, Qingming Huang, Qixiang Ye, Wen Gao

  **Introduction (English):** Digitized Traditional Chinese Paintings (TCPs) need effective detection and categorization for retrieval, but distinguishing TCPs from general images and classifying Gongbi/Xieyi styles is challenging. This paper proposes a two-step method: first use C4.5 decision tree + autocorrelation features to detect TCPs, then combine edge-size histogram, color features, and autocorrelation textures with SVM to categorize into Gongbi/Xieyi. It achieves high accuracy with low computation cost.

- **Style-based Classification of Chinese Ink and Wash Paintings** [Opt. Eng. 2013] [[paper\]](https://ui.adsabs.harvard.edu/abs/2013OptEn..52i3101S/abstract)

  **Authors:** Jiachuan Sheng, Jianmin Jiang

  **Introduction (English):** Automated author-style classification of digitized Chinese ink and wash paintings (IWPs) is vital for management, but IWPs’ lack of color/tones limits traditional image processing methods. This paper proposes a style-based algorithm: it uses edge detection to locate local regions and extract stroke-based histogram features reflecting artist styles. Parallel neural networks process these features, with information entropy-balanced fusion integrating global and local cues for final classification, achieving good performance.

- **An Effective Approach to Identify Digitized IWPs (Ink and Wash Paintings)** [CISP 2012] [[paper\]](https://ieeexplore.ieee.org/document/6469719)

  **Author:** JiaChuan Sheng

  **Introduction (English):** Content-based methods fail to identify digitized ink and wash paintings (IWPs) due to their lack of color/tones and reliance on stylistic strokes. This paper proposes a style-based identification algorithm: it uses edge detection to locate local regions and extract histogram features from painting strokes, then feeds these features into a neural network for automatic classification. Experiments show good performance, supporting computerized analysis and management of IWPs.

- **Studying Digital Imagery of Ancient Paintings by Mixtures of Stochastic Models** [IEEE Trans. Image Process. 2004] [[paper\]](https://ieeexplore.ieee.org/document/1278358/)

  **Authors:** Jia Li, J.Z. Wang

  **Introduction (English):** Analyzing digital imagery of ancient paintings (e.g., texture, brushwork, aging traces) is crucial for preservation and authentication, but their complex, stochastic artistic and degradation features challenge traditional analytical methods. This paper proposes a framework using mixtures of stochastic models to model the multi-scale, non-homogeneous characteristics of ancient painting imagery. It decomposes image features into stochastic components, captures subtle patterns (e.g., brush stroke randomness, aging texture variations), and enables quantitative analysis, supporting tasks like authenticity verification and restoration assessment.

- **Rhythmic Brushstrokes Distinguish van Gogh from His Contemporaries: Findings via Automated Brushstroke Extraction** [IEEE Trans. Pattern Anal. Mach. Intell. 2012] [[paper\]](https://ieeexplore.ieee.org/document/6042878)

  **Authors:** Jia Li, Lei Yao, Ella Hendriks, James Z. Wang

  **Introduction (English):** Authenticating van Gogh’s works relies on identifying his unique brushstroke style, but manual analysis is subjective and inefficient. This paper proposes an automated brushstroke extraction method integrating edge detection and clustering-based segmentation. It statistically analyzes massive extracted brushstrokes, confirming van Gogh’s brushstrokes are highly rhythmic (regular shapes, tight arrangement, repetitive patterns) — a key trait distinguishing him from contemporaries and consistent across his French periods.

- **MTFFNet: A Multi-task Feature Fusion Framework for Chinese Painting Classification** [Cogn. Comput. 2021] [[paper\]](https://link.springer.com/article/10.1007/s12559-021-09896-9)

  **Authors:** Wei Jiang, Xiaoyu Wang, Jinchang Ren, Sen Li, Meijun Sun, Zheng Wang, Jesse S. Jin

  **Introduction (English):** Classifying traditional Chinese paintings by artist style is challenging due to the difficulty of fusing semantic and brush stroke features. This paper proposes MTFFNet, a multi-task feature fusion framework with DenseNet as the backbone. It has two branches: one extracts RGB-based semantic/color features, and the other extracts brush stroke/texture features via gray-level co-occurrence matrix (GLCM). The fused features are fed into a multi-kernel SVM classifier, achieving higher accuracy and better generalization than state-of-the-art methods.

- **Fine-Art Painting Classification via Two-Channel Dual Path Networks** [Int. J. Mach. Learn. Cybern. 2020] [[paper\]](https://link.springer.com/article/10.1007/s13042-019-00963-0)

  **Authors:** Sheng-hua Zhong, Xingsheng Huang, Zhijiao Xiao

  **Introduction (English):** Fine-art painting classification requires capturing both global semantic and local stylistic features, but single-path networks struggle to balance the two. This paper proposes a two-channel dual path network (DPN): one channel processes RGB images to extract global content/semantic features, the other processes gray-level images to capture local texture/stylistic features. Dual path fusion integrates multi-scale features, enhancing discriminability. Experiments on fine-art datasets (including Chinese paintings) show higher classification accuracy than traditional CNNs and single-channel models.

- **DCT–CNN-based Classification Method for the Gongbi and Xieyi Techniques of Chinese Ink-Wash Paintings** [Neurocomputing 2019] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0925231218313201)

  **Authors:** Wei Jiang, Zheng Wang, Jesse S. Jin, Yahong Han, Meijun Sun

  **Introduction (English):** Classifying Gongbi and Xieyi Chinese ink-wash paintings (IWPs) is challenging due to similar content and the need for effective brushstroke feature extraction. This paper proposes a DCT-CNN framework: it uses Sobel edge detection to extract brushstrokes, applies discrete cosine transformation (DCT) to reduce data dimensionality, and feeds selected DCT coefficients into a CNN for automatic feature extraction. A hybrid CNN-SVM model is adopted for classification, achieving competitive performance on a 1400-IWP dataset while reducing computational complexity.

- **Multi-Instance Learning Algorithm Based on LSTM for Chinese Painting Image Classification** [IEEE Access 2020] [[paper\]](https://ieeexplore.ieee.org/abstract/document/9210099)

  **Authors:** Daxiang Li, Yue Zhang

  **Introduction (English):** Chinese painting classification faces challenges from abstract brushwork and ambiguous content boundaries. This paper proposes a multi-instance learning (MIL) algorithm based on LSTM: divide paintings into image patches (instances), extract features via CNN, input instance features into LSTM to model inter-instance contextual relationships, and use MIL to handle label ambiguity. Experiments show improved classification accuracy for styles/themes compared to traditional methods.

- **中国传统水墨画的计算机分类与算法研究（Computer Classification and Algorithm Research of Traditional Chinese Ink Wash Paintings）** [Ph.D. Thesis, Tianjin University, 2013] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=lSOmZDqoX8PdzE63QXO2Jeo-8auKJHUexUMAyg3QFcsKvy59OXjWjGLORLyEYOxqQ9b7ZZsrASOglqzYNGpasimZ4QOb94OyhuwWxhPCCUx06pFujc0kjKA_46RH2VDU3GgwDOcWmx3Qqi373AswMRHgdTb2H5ZH9pfl7oGjOmCUIOtSKcmm1Q==&uniplatform=NZKPT&language=CHS)

  **Author:** Sheng Jiachuan

  **Introduction (English):** To solve the poor adaptability of traditional methods to colorless, brushstroke-dependent Chinese ink wash paintings (IWPs), this thesis proposes style-feature-based classification algorithms. It extracts brushstroke features via edge detection and histogram techniques, fuses neural networks and information entropy, and addresses author identification and Gongbi/Xieyi style distinction, constructing a classification framework tailored for digital IWPs.

- **Study on the Emotional Image of Calligraphy Strokes based on Sentiment Analysis** [2020 5th International Conference on Communication, Image and Signal Processing (CCISP)] [[paper\]](https://ieeexplore.ieee.org/document/9273474)

  **Authors:** Yingying Pan, Ruimin Lyu, Qinyan Nie, Lei Meng

  **Introduction (English):** Traditional research on calligraphy strokes' emotional meaning relies on personal experience, lacking public perception data. This study designs an aesthetic-engineering integrated experiment: participants write articles after feeling 12 famous calligraphers' typical strokes, then sentiment analysis, quantitative analysis and visualization are used to reveal the public's subjective emotional image of the strokes.

- **基于表现手法的国画分类方法研究（Research on Classification Methods of Chinese Paintings Based on Expression Techniques）**[[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=lSOmZDqoX8MKfDAWIjg-UH-TzEYh2_Y91noCHVrTo3RpiwlMIBPmc4ZymDwt1Nl_dil0DQCT8ktvB7TjXBF0Ae86nLRouhVH6pE7nOyM6zK9h4n8RHAyA7tBRN84DYlqrqNbC3L6PPNmAiEsIY_gETKirnIjNBBGhtFpt5VWKCh3P99UA7gmqg==&uniplatform=NZKPT&language=CHS)

  **Authors:** Gao Feng, Nie Jie, Huang Lei, Duan Lingyu, Li Xiaoming

  **Introduction (English):** Focusing on the classification of Chinese paintings based on expression techniques (Gongbi and Xieyi), this paper proposes a targeted classification method. It extracts discriminative features related to painting techniques, such as brushstroke texture and line characteristics, and builds an effective classification model. The study aims to solve the problem of low accuracy in traditional methods caused by the abstract nature of Chinese painting techniques, providing technical support for the automatic classification and management of Chinese paintings.

#### 4.3 Stylized Structure Generation with Structured Priors

- **From Writing to Painting: A Kinect-Based Cross-Modal Chinese Painting Generation System** [Proceedings of the 22nd ACM International Conference on Multimedia, 2014] [[paper\]](https://dl.acm.org/doi/10.1145/2647868.2654911)

  **Authors:** LI Jiajia, Grace Ngai, Stephen C.F. Chan, Kien A. Hua, Hong Va Leong, Alvin Chan

  **Introduction (English):** This paper presents CalliPaint, a Kinect-based cross-modal system linking Chinese ink brush calligraphy and landscape painting. Based on metaphoric congruence, it maps the two modalities to enable intuitive creation: novice users can generate attractive landscape paintings through calligraphy writing. Evaluations show it offers a more enjoyable and easy-to-learn experience than general digital painting software.

- **Image-based synthesis of Chinese landscape painting** [Journal of Computer Science and Technology, 2003, 18(1): 22-28] [[paper\]](https://link.springer.com/article/10.1007/BF02946647)

  **Authors:** Yu JinHui, Luo GuoMing, Peng QunSheng

  **Introduction (English):** This paper proposes a new image-based framework for synthesizing Chinese landscape painting. It includes a preprocessing phase (collecting brush stroke texture primitives (BSTP) from hand-made paintings and constructing a control picture) and an on-line phase (synthesizing fog images and mapping multi-layer BSTP guided by the control picture, with shading pictures for complex shading). The synthesized paintings are more similar to hand-made works than previous modeling methods.

- **A novel method of converting photograph into Chinese ink painting** [IEEJ Trans. Electr. Electron. Eng., 2015, 10(3): 320-329] [[paper\]](https://onlinelibrary.wiley.com/doi/10.1002/tee.22088)

  **Authors:** Guo Fan, Peng Hui, Tang Jin

  **Introduction (English):** This paper presents a novel method to convert photographs into Chinese ink paintings. First, it estimates the Structure Description Map (SDM) of the photo to depict object appearance. A color transform algorithm is then proposed to adjust the color to meet traditional Chinese ink painting requirements. Qualitative evaluation shows the method produces aesthetically pleasing results with less user interaction and faster conversion speed compared to other approaches.

- **An Efficient Rendering Method of Wash-Ink Strokes and Its Applications** [J. Comput. Aided Des. Comput. Graph., 2014, 26(3): 356-363] [[paper\]](https://www.researchgate.net/publication/286979811_An_efficient_rendering_method_of_wash-ink_strokes_and_its_applications)

  **Authors:** Li Dajin, Bai Chengjie

  **Introduction (English):** To address the inefficiency of physical-based ink diffusion models, this paper proposes an image-based rendering method for Chinese wash-ink strokes. It divides strokes into three regions, generates diffused regions and irregular boundaries based on ink water ratio and paper properties, and adds luminance variation to simulate pigment granulation. The method is efficient and realistic, applicable to interactive painting systems, style transformation, and 3D scene rendering.

- **End-to-End Chinese Landscape Painting Creation Using Generative Adversarial Networks** [arXiv:2011.05552 [cs.CV], 2020] [[paper\]](https://arxiv.org/abs/2011.05552)

  **Author:** Alice Xue

  **Introduction (English):** Addressing the lack of originality in conditional input-dependent GAN-based art generation, this paper proposes SAPGAN (Sketch-And-Paint GAN), the first end-to-end model for Chinese landscape painting creation without conditional input. It consists of SketchGAN (generating edge maps) and PaintGAN (translating edges to paintings), trained on a new dataset of traditional Chinese landscape paintings. A Visual Turing Test with 242 participants shows 55% of SAPGAN’s outputs are mistaken for human works, outperforming baseline GANs.

- **Transform a Simple Sketch to a Chinese Painting by a Multiscale Deep Neural Network** [Algorithms, 2018, 11(1): 4] [[paper\]](https://www.mdpi.com/1999-4893/11/1/4)

  **Authors:** Daoyu Lin, Yang Wang, Guangluan Xu, Jun Li, Kun Fu

  **Introduction (English):** To address the limitation of deep learning-based image synthesis focusing on simple datasets, this paper proposes a multiscale deep neural network for converting sketches to Chinese paintings. It combines L1 loss and adversarial loss for training, enabling feed-forward controllable synthesis with both local details and global framework. The model can also serve as neural style transfer with an edge detector, and exhibits universality in image colorization and super-resolution.

- **Sketch to Chinese paintings: A three-stage progressive generation network via enhancing sketch** [J. Frankl. Inst., 2024, 361(18): 107246] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0016003224006677)

  **Authors:** Shuai Yang, Mengxue Wang, Jing Guo, Ze Gao, Yongzhen Ke, Fan Qin

  **Introduction (English):** Existing sketch-based Chinese painting generation models often rely on complete edge maps from mature paintings, leading to poor quality when using sparse-line user sketches. This paper proposes a three-stage progressive generation network: it first generates sketches with different line richness via reduction and enhancement networks, then uses three connected generative networks to progressively learn structure, color, and detail information. Experimental results show the model generates higher-quality Chinese paintings and has better generalization to user sketches.

- **Real-time Rendering of 3D Ink-wash Painting Based on Geometry Buffers** [J. Inst. Ind. Appl. Eng., 2017, 5: 65-70] [[paper\]](https://www.researchgate.net/publication/317281234_Real-time_Rendering_of_3D_Ink-wash_Painting_Based_on_Geometry_Buffers)

  **Authors:** Gua Yu, Naoki Ono, Kiichi Urahama

  **Introduction (English):** To achieve real-time rendering of 3D ink-wash painting effects, this paper proposes a method based on geometry buffers (G-buffers). It extracts depth, normal, and position information of 3D models via G-buffers, simulates ink diffusion and shading characteristics of traditional ink-wash paintings through shader programming, and realizes efficient real-time rendering without complex physical calculations. The method maintains the artistic style of ink-wash paintings while ensuring interactive frame rates.

- **The Synthesis of Rock Textures in Chinese Landscape Painting** [Computer Graphics Forum 2001] [[paper\]](https://onlinelibrary.wiley.com/doi/abs/10.1111/1467-8659.00505)

  **Authors:** Der-Lor Way, Zen-Chung Shih

  **Introduction (English):** Rock textures are crucial in Chinese landscape painting, conveying mountain orientation and atmosphere, with core strokes like hemp-fiber (for gentle slopes) and axe-cut (for hard surfaces). This paper proposes a novel synthesis method for rock textures. Users only need to specify contours and parameters, and the method completes the entire painting process automatically. It is applicable for interactive creation by artists and automated natural scene rendering.

- **Stroke-based real-time ink wash painting style rendering for geometric models** [SIGGRAPH Asia 2012 Technical Briefs, 2012] [[paper\]](https://dl.acm.org/doi/10.1145/2407746.2407765)

  **Authors:** Tian-Chen Xu, Li-Jie Yang, En-Hua Wu

  **Introduction (English):** This paper presents a stroke-based approach for real-time ink wash painting style rendering on geometric models. It creates a particle-based ink footprint model, extracts classified strokes using 3D model geometry information, and combines strokes with ink effects to generate immersive paintings. Leveraging GPU parallel processing, the method achieves real-time rendering on consumer-level PCs while retaining realistic Chinese ink wash characteristics.

- **Instance-Aware Coherent Video Style Transfer for Chinese Ink Wash Painting** [Proceedings of the Thirtieth International Joint Conference on Artificial Intelligence (IJCAI-21), 2021, pp. 823-829] [[paper\]](https://www.ijcai.org/proceedings/2021/114)

  **Authors:** Hao Liang, Shuai Yang, Wenjing Wang, Jiaying Liu

  **Introduction (English):** Existing fast video style transfer methods perform well on Western paintings but struggle with Chinese ink wash painting due to its unique techniques and aesthetics, leading to poor temporal consistency or loss of freehand brushstroke features. This paper proposes a novel framework: it uses multi-frame fusion (reference frame-based reordering and stylization) to enhance temporal coherence, and instance segmentation for adaptive background white space reservation and foreground feature extraction at proper scales. Experiments show superior performance in both temporal consistency and visual quality.

- **Generation of Aesthetic Chinese Flower Painting by Stroke-Based Stylization** [J. Comput. Aided Des. Comput. Graph., 2020, 32(11): 1721-1730] [[paper\]](https://www.jcad.cn/en/article/doi/10.3724/SP.J.1089.2020.18178)

  **Authors:** Yang Lijie, Xu Tianchen, Wu Enhua

  **Introduction (English):** To simplify the creation of aesthetic Chinese flower paintings, this paper proposes a stroke-based stylization tool. Unlike full-image style transfer methods, it focuses on detailed style features and user intent: correcting inaccurate user sketch strokes, selecting optimal style patterns for each skeletal stroke, and mapping patterns via shape calculation and texture synthesis. Experiments show the generated paintings match the specified style and meet aesthetic expectations, suitable for touch devices and art education.

- **Automatic Colorization of Chinese Ink Painting Combining Multi-Level Features and Generative Adversarial Networks** [Fractals, 2023, 31(6): 2340144] [[paper\]](https://www.worldscientific.com/doi/abs/10.1142/S0218348X23401448?srsltid=AfmBOoo_-HMCi2THdOZ4DufC2jSmp93i0WQmPQMNHJ_SsdqdwvaOpM2X)

  **Authors:** Bing Wu, Qingshuang Dong, Wenqi Sun

  **Introduction (English):** Traditional Chinese ink paintings are often black and white, while elaborate flower-and-bird ink paintings feature rich colors. Existing colorization algorithms fail to extract high-level semantic and low-level local features of ink paintings, leading to blurry borders and low color saturation. This paper proposes an automatic colorization method combining multi-level features (global + local) and GANs. Evaluations via PSNR, SSIM, colorfulness, and user studies show it outperforms previous methods in coloring accuracy, coherence, color richness, and overflow control.

- **High Relief from Brush Painting** [IEEE Trans. Vis. Comput. Graph., 2019, 25(9): 2763-2776] [[paper\]](https://ieeexplore.ieee.org/document/8419282)

  **Authors:** Yunfei Fu, Hongchuan Yu, Chih-Kuo Yeh, Jianjun Zhang, Tong-Yee Lee

  **Introduction (English):** Relief bridges 2D painting and 3D sculpture, but generating high relief from brush paintings remains unsolved. This paper proposes a novel approach: it extracts brushstrokes via layer decomposition (with ETF field and coherent lines) and modified MSERs (using opacity instead of intensity), then generates relief proxies for each stroke through inflation and displacement maps based on opacity. The method preserves brushstroke details and artistic style, and supports image editing applications. Experiments show it outperforms existing methods in extracting overlapped strokes and preserving fine details.

- **Attentional Wavelet Network for Traditional Chinese Painting Transfer** [2020 25th International Conference on Pattern Recognition (ICPR), 2021, pp. 3077-3083] [[paper\]](https://ieeexplore.ieee.org/document/9413063)

  **Authors:** Rui Wang, Huaibo Huang, Aihua Zheng, Ran He

  **Introduction (English):** Traditional Chinese paintings feature "Gongbi" (detailed portrayal) and "Xieyi" (conceptual expression), making photo-to-Chinese painting transfer challenging. This paper proposes an attentional wavelet network: it uses 2D Haar wavelet transform to extract high-level conception and local details, designs separate streams for high/low frequency processing, and adopts self-attention to supplement missing details. A new P2A Dataset (photos and Chinese paintings of famous mountains) is constructed. Experiments show the method outperforms state-of-the-art style transfer algorithms.

#### 4.4 Mapping Artistic Intent to Computational Execution

- **Virtual Hairy Brush for Digital Painting and Calligraphy** [Science in China Ser. F 2005] [[paper\]](https://www.researchgate.net/publication/277373114_Virtual_hairy_brush_for_digital_painting_and_calligraphy)

  **Author:** Songhua Xu

  **Introduction (English):** Existing virtual brush systems struggle to balance user-friendliness, expressiveness, and real-time performance for digital Chinese painting/calligraphy. This paper proposes a novel virtual hairy brush framework based on solid modeling: it uses "writing primitives" (hair clusters) instead of individual bristles to reduce simulation complexity, models brush deformation and ink deposition dynamically, and develops an interactive prototype system. The system enables real-time creation of high-quality digital paintings/calligraphy, addressing the trade-off between realism and efficiency.

- **Two Methods for Creating Chinese Painting** [Proc. of Pacific Graphics, 2002, pp. 403-412] [[paper\]](https://people.tamu.edu/~ergun/research/artisticdepiction/papers/pg02.pdf)

  **Authors:** Ching Chan, Ergun Akleman, Jianer Chen

  **Introduction (English):** This paper proposes two methods for creating realistic Chinese paintings. The first method leverages existing software packages to generate 3D Chinese painting animations. The second is an expressive painting tool that enables artists to interactively create 2D Chinese paintings.

- **Animating Strokes in Drawing Process of Chinese Ink Painting** [J. Comput. Aided Des. Comput. Graph., 2016, 28(5): 742-749] [[paper\]](https://www.jcad.cn/en/article/id/db8205ad-f7d8-42c1-a2b0-960b1cc20842)

  **Authors:** Yang Lijie, Xu Tianchen, Wu Enhua

  **Introduction (English):** To vividly simulate the real drawing process of Chinese ink painting, this paper proposes an animation tool based on reproducible brush strokes. Unlike previous methods that require manual input of brush trajectories, it first decomposes the input ink painting image into individual brush strokes, then automatically extracts brush trajectories using shape outline and skeleton information. A brush footprint model is built to constrain trajectory quality via parameters (location, size, orientation) and dynamically renders trajectories into strokes with a real-time model. The tool is valuable for ink painting appreciation, analysis, and art education.

- **Animating Chinese Paintings through Stroke-Based Decomposition** [ACM Trans. Graph., 2006, 25(2): 239–267] [[paper\]](https://dl.acm.org/doi/10.1145/1138450.1138454)

  **Authors:** Songhua Xu, Yingqing Xu, Sing Bing Kang, David H. Salesin, Yunhe Pan, Heung-Yeung Shum

  **Introduction (English):** This paper proposes a stroke-based decomposition method to animate traditional Chinese paintings. It first decomposes static Chinese paintings into individual brush strokes via image analysis and clustering, then infers the temporal order and dynamic parameters (e.g., speed, pressure) of strokes based on artistic rules. The strokes are replayed with dynamic rendering to simulate the realistic drawing process, preserving the artistic style and brushwork details of the original paintings. The method enables interactive animation of Chinese paintings for appreciation and education.

- **Animating Chinese Paintings through Stroke-Based Decomposition** [ACM Trans. Graph., 2006, 25(2): 239–267] [[paper\]](https://dl.acm.org/doi/10.1145/1138450.1138454)

  **Authors:** Songhua Xu, Yingqing Xu, Sing Bing Kang, David H. Salesin, Yunhe Pan, Heung-Yeung Shum

  **Introduction (English):** This paper presents a stroke-based decomposition approach for animating traditional Chinese paintings. It decomposes static Chinese paintings into individual brush strokes via image analysis and clustering, infers the temporal order and dynamic parameters (e.g., speed, pressure) of strokes based on artistic rules, and replays strokes with dynamic rendering to simulate the realistic drawing process. The method preserves the original artistic style and brushwork details, enabling interactive animation for Chinese painting appreciation and education.

- **From Writing to Painting: A Kinect-Based Cross-Modal Chinese Painting Generation System** [Proceedings of the 22nd ACM International Conference on Multimedia, 2014] [[paper\]](https://dl.acm.org/doi/10.1145/2647868.2654911)

  **Authors:** LI Jiajia, Grace Ngai, Stephen C.F. Chan, Kien A. Hua, Hong Va Leong, Alvin Chan

  **Introduction (English):** This paper presents CalliPaint, a Kinect-based cross-modal system linking Chinese ink brush calligraphy and landscape painting. Based on metaphoric congruence, it maps the two modalities to enable intuitive creation: novice users can generate attractive landscape paintings through calligraphy writing. Evaluations show it offers a more enjoyable and easy-to-learn experience than general digital painting software.

- **Study on the Emotional Image of Calligraphy Strokes based on Sentiment Analysis** [CCISP, 2020, pp. 264-269] [[paper\]](https://ieeexplore.ieee.org/document/9273474)

  **Authors:** Yingying Pan, Ruimin Lyu, Qinyan Nie, Lei Meng

  **Introduction (English):** Calligraphic strokes convey rich emotional information, but traditional research on their emotional image relies mostly on personal experience of calligraphers and theorists, lacking public perspective. This paper proposes an educational experiment integrating aesthetics with science and engineering: participants write articles based on feeling and imagining typical calligraphic strokes, then sentiment analysis, quantitative analysis, and data visualization are applied to the articles. The study reveals the rich subjective images of typical strokes from twelve famous historical calligraphers, with dual research and teaching value.

- **Easy Drawing: Generation of Artistic Chinese Flower Painting by Stroke-Based Stylization** [IEEE Access, 2019, 7: 35449-35456] [[paper\]](https://ieeexplore.ieee.org/abstract/document/8666126)

  **Authors:** Lijie Yang, Tianchen Xu, Jixiang Du, Enhua Wu

  **Introduction (English):** Creating high-quality Chinese flower paintings requires professional skills, while existing tools either demand accurate user inputs or only perform full-image style transfer. This paper proposes a photo-guided stroke-based stylization tool: it corrects user’s rough sketches via opposite-direction search, selects optimal style patterns through energy function minimization, and generates stylized strokes by calculating adaptive width (based on length and curvature) and synthesizing texture. The tool works well on touch devices, tolerates input errors, and produces aesthetically pleasing paintings, suitable for users without drawing experience.

- **Generation of Aesthetic Chinese Flower Painting by Stroke-Based Stylization** [J. Comput. Aided Des. Comput. Graph., 2020, 32(11): 1721-1730] [[paper\]](https://www.jcad.cn/en/article/doi/10.3724/SP.J.1089.2020.18178)

  **Authors:** Yang Lijie, Xu Tianchen, Wu Enhua

  **Introduction (English):** To simplify the creation of aesthetic Chinese flower paintings, this paper proposes a stroke-based stylization tool. Unlike full-image style transfer methods, it focuses on detailed style features and user intent: correcting inaccurate user sketch strokes, selecting optimal style patterns for each skeletal stroke, and mapping patterns via shape calculation and texture synthesis. Experiments show the generated paintings match the specified style and meet aesthetic expectations, suitable for touch devices and art education.

### 5. Generative Transmission: Exemplar Learning and Cross-Modal Generation

#### 5.1 Fidelity-Preserving Augmentation and Restoration

- **Learning a Deep Convolutional Network for Image Super-Resolution** [ECCV, 2014, pp. 184–199] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-319-10593-2_13)

  **Authors:** Chao Dong, Chen Change Loy, Kaiming He, Xiaoou Tang

  **Introduction (English):** This paper proposes a deep learning method for single image super-resolution (SR). It learns an end-to-end mapping between low and high-resolution images via a deep convolutional neural network (CNN), which takes low-resolution images as input and outputs high-resolution ones. Unlike traditional sparse-coding-based SR methods that handle components separately, this method jointly optimizes all layers. The lightweight CNN achieves state-of-the-art restoration quality and fast speed for practical online use.

- **Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network** [arXiv:1609.04802 [cs.CV], 2017] [[paper\]](https://arxiv.org/abs/1609.04802)

  **Authors:** Christian Ledig, Lucas Theis, Ferenc Huszar, Jose Caballero, Andrew Cunningham, Alejandro Acosta, Andrew Aitken, Alykhan Tejani, Johannes Totz, Zehan Wang, Wenzhe Shi

  **Introduction (English):** Existing super-resolution (SR) methods often produce over-smoothed results lacking photo-realism. This paper proposes SRGAN, a generative adversarial network (GAN) for photo-realistic single image SR. It introduces a perceptual loss combining adversarial loss (training the generator to fool a discriminator) and content loss (using VGG features to preserve structural similarity). SRGAN generates high-resolution images with finer textures and more realistic details than traditional methods, achieving state-of-the-art performance on benchmark datasets.

- **Details or Artifacts: A Locally Discriminative Learning Approach to Realistic Image Super-Resolution** [arXiv:2203.09195 [eess.IV], 2022] [[paper\]](https://arxiv.org/abs/2203.09195)

  **Authors:** Jie Liang, Hui Zeng, Lei Zhang

  **Introduction (English):** GAN-based single image super-resolution (SISR) often suffers from unstable training, leading to perceptual artifacts alongside generated details. This paper proposes a Locally Discriminative Learning (LDL) approach: it leverages differences in local statistics (e.g., residual variance) between artifacts and realistic details to train a discriminator that generates an artifact map. This map regularizes model training, enabling stable generation of realistic details while suppressing artifacts. LDL is lightweight, compatible with existing SISR methods, and achieves superior reconstruction accuracy and perceptual quality on synthetic and real-world datasets.

- **A diffusion probabilistic model for traditional Chinese landscape painting super-resolution** [Heritage Sci., 2024, 12(1): 4] [[paper\]](https://www.nature.com/articles/s40494-023-01123-y)

  **Authors:** Qiongshuai Lyu, Na Zhao, Yu Yang, Yuehong Gong, Jingli Gao

  **Introduction (English):** Traditional Chinese landscape paintings often suffer from low resolution during digital protection. This paper proposes CLDiff, a diffusion probabilistic model for super-resolution (SR) of such paintings. It uses a parameterized Markov chain to transform Gaussian noise into high-resolution paintings via iterative denoising, guided by low-resolution inputs. An attention module with an energy function is integrated into the U-Net backbone to enhance key feature capture. CLDiff avoids GAN-related issues (mode collapse, unstable training) and achieves clear ink textures, superior visual effects, and competitive performance on SR tasks.

- **A Single Historical Painting Super-Resolution via a Reference-Based Zero-Shot Network** [Int. J. Comput. Intell. Syst., 2021, 14(1): 1577-1588] [[paper\]](https://www.atlantis-press.com/journals/ijcis/125956410)

  **Authors:** Hongzhen Shi, Dan Xu, Hao Zhang, YingYing Yue

  **Introduction (English):** Learning-based single image super-resolution (SISR) is hard to apply to unique historical paintings due to the lack of ground truth and datasets. This paper proposes Ref-ZSSR, a reference-based zero-shot network for historical painting SISR. It extracts global and local multi-scale similar information from the painting itself to provide artistic style knowledge, enabling end-to-end synthesis of high-resolution images with sharp textures. Compared to ZSSR, Ref-ZSSR improves precision (≈4.68 dB for ×2 scale) and visual perception, and requires no external examples, making it applicable to various damaged cultural relics.

- **Unsupervised Single Image Super-Resolution Network (USISResNet) for Real-World Data Using Generative Adversarial Network** [CVPRW, 2020, pp. 1904-1913] [[paper\]](https://ieeexplore.ieee.org/document/9151093)

  **Authors:** Kalpesh Prajapati, Vishal Chudasama, Heena Patel, Kishor Upla, Raghavendra Ramachandra, Kiran Raja, Christoph Busch

  **Introduction (English):** Supervised SISR methods trained on synthetic LR images (e.g., bicubic downsampling) perform poorly on real-world data with unknown degradation. This paper proposes USISResNet, an unsupervised GAN-based network for real-world SISR. It introduces a Mean Opinion Score (MOS)-based loss function to enhance perceptual quality. Evaluated on NTIRE-2020 Real-world SR Challenge datasets, USISResNet demonstrates strong generalization and reliable accuracy on real-world LR images, outperforming state-of-the-art methods dependent on synthetic data.

- **Research on Super-Resolution Relationship Extraction and Reconstruction Methods for Images Based on Multimodal Graph Convolutional Networks** [Math. Probl. Eng., 2022, 2022: 1016112] [[paper\]](https://www.researchgate.net/publication/363473034_Research_on_Super-Resolution_Relationship_Extraction_and_Reconstruction_Methods_for_Images_Based_on_Multimodal_Graph_Convolutional_Networks)

  **Authors:** Jie Xiao

  **Introduction (English):** Traditional super-resolution (SR) methods struggle to capture complex structural relationships between image regions, leading to insufficient detail restoration. This paper proposes an SR method based on multimodal graph convolutional networks (MGCN). It constructs a graph structure using multimodal features (e.g., texture, edge, semantic) of low-resolution (LR) images, extracts intra-modal and inter-modal spatial relationships via graph convolution, and fuses these relationships to guide high-resolution (HR) image reconstruction. Experiments show the method effectively enhances structural coherence and detail richness, outperforming traditional CNN-based SR methods in both objective metrics (PSNR, SSIM) and subjective visual quality.

- **An Ancient Chinese Painting Restoration Method Based on Improved Generative Adversarial Network** [J. Phys.: Conf. Ser., 2022, 2400(1): 012005] [[paper\]](https://iopscience.iop.org/article/10.1088/1742-6596/2400/1/012005)

  **Authors:** Renquan Luo, Renze Luo, Liang Guo, Hong Yu

  **Introduction (English):**Aiming at the inefficiency and secondary damage risks of manual restoration for damaged ancient Chinese paintings, this paper proposes UGAN—an improved GAN-based model with U-Net generator and DCGR-Block. It enhances shallow/deep feature extraction, outperforming GLCIC by 8.14% (PSNR) and 4.79% (SSIM) on overall missing regions, and excels at high damage rates.

- **Computer-Aided Analysis of Seals in Ancient Chinese Paintings Based on Image Extraction and Restoration** [J. Comput. Aided Des. Comput. Graph., 2025, 37(2): 254-264] [[paper\]](https://www.jcad.cn/article/doi/10.3724/SP.J.1089.2023-00343)

  **Authors:** Lin Xinyi, Wu Hongjia, Yuan Zhiting, Zhang Hongxin, Chen Wei

  **Introduction (English):** Traditional manual seal analysis in ancient Chinese paintings is inefficient and labor-intensive. This study proposes an automatic extraction and restoration method for seals, constructs a dataset with 1,762 ancient paintings and their seals, and builds seal portraits using overall, local, and associated features. A visual analysis system enables multi-perspective presentation, significantly improving experts’ comparison efficiency, with effectiveness verified by case studies and positive expert feedback.

- **From Inpainting to Painting: Exploring Conservation of Chinese Paintings with Generative Artificial Intelligence** [Master's Thesis, Simon Fraser University, 2024] [[thesis\]](https://summit.sfu.ca/item/38702)

  **Author:** Shumeng Dai

  **Introduction (English):** Chinese painting conservation faces conflicts between minimal intervention/recognizability/reversibility principles and traditional pursuit of restoration completeness, plus the loss of historical artworks. This master’s thesis explores GenAI’s potential in virtual restoration and reconstruction, using Stable Diffusion to fill missing portions of Chinese paintings and recreate a lost work by Qing Dynasty artists. Results show GenAI aids virtual restoration, visualizes lost works in original styles, and provides insights for art conservation, exhibition, and research.

- **Material Classification Method of Traditional Chinese Painting Image Based on Prototypical Network** [npj Heritage Sci., 2025, 13(1): 377] [[paper\]](https://www.nature.com/articles/s40494-025-01949-8)

  **Authors:** Zhibin Su, Luyue Zhang, Jinyu Liu, Shuang Wang

  **Introduction (English):** Intelligent material classification of traditional Chinese paintings is critical for digital preservation but hindered by limited samples and weak feature representation. This paper proposes a framework based on a ResNet18-backed prototypical network, integrating cropping augmentation (for fine-grained details), multitask learning (joint material and dynasty classification), and ensemble voting. Experiments on a self-constructed dataset show 80% accuracy with 30 samples, outperforming comparative methods in few-shot scenarios.

- **Monte Carlo Convex Hull Model for Classification of Traditional Chinese Paintings** [Neurocomputing, 2016, 171: 788-797] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0925231215011601)

  **Authors:** Meijun Sun, Dong Zhang, Zheng Wang, Jinchang Ren, Jesse S. Jin

  **Introduction (English):** Classifying traditional Chinese paintings by artist style is challenging due to their unique brushwork-focused characteristics. This paper proposes an integrated artistic style descriptor with a Monte Carlo Convex Hull (MCCH) feature selection model and SVM classifier. It combines visual features (including composition and object features) and uses an infusion factor to optimize feature selection, enhancing discriminative power. Experiments on 180 paintings by 6 artists show the method outperforms existing techniques in precision and recall.

- **中国画分类的改进嵌入式学习算法（Improved Embedded Learning for Classification of Chinese Paintings）** [J. Comput.-Aided Des. Comput. Graph. 2018] [[paper\]](https://www.jcad.cn/article/doi/10.3724/SP.J.1089.2018.16539)

  **Authors:** Yuzhi Li, Jiachuan Sheng, Bin Hua

  **Introduction (English):** To address the limitation that existing Chinese painting classification ignores inter-painting relationships and feature importance, this paper proposes an improved embedded learning algorithm: it extracts features via fine-tuning the pre-trained VGG-F model, integrates mutual information into embedded learning, and uses SVM for classification, achieving 86% average accuracy on 10 artists’ works with better robustness.

- **Feature Extraction and Classification of Chinese Traditional Paintings** [Comput. Eng. Appl., 2008, 44(15): 166-169] [[paper\]](https://caod.oriprobe.com/articles/14073534/Feature_extraction_and_classification_of_Chinese_P.htm)

  **Authors:** Chen Junjie, Du Yajuan, Li Haifang

  **Introduction (English):** Semantic retrieval of Chinese traditional paintings relies on effective feature extraction of color and shape. This paper proposes a new feature vector by fusing color and shape features, analyzes the correlation between multi-dimensional low-order features and high-level semantics of paintings, and adopts support vector machine (SVM) for semantic classification. Experimental results show the extracted features are stable, achieving high classification accuracy.

- **Reconstructing Traditional Chinese Paintings with Immersive Virtual Reality** [CHI EA, 2020, pp. 1–8] [[paper\]](https://dl.acm.org/doi/fullHtml/10.1145/3334480.3382934)

  **Authors:** Sheng Jin, Min Fan, Yongchao Wang, Qi Liu

  **Introduction (English):** Traditional Chinese paintings are usually displayed in 2D, lacking immersive appreciation experiences. This paper proposes an immersive VR reconstruction method for traditional Chinese paintings: it converts 2D paintings into 3D virtual scenes by integrating depth estimation, scene modeling, and interactive design. The VR system supports free viewing angles, detail zooming, and contextual information overlay, enabling users to "walk into" the paintings and perceive artistic conception intuitively. User evaluations confirm the method enhances immersion and appreciation experience.

- **Deep Multimodal Learning for Affective Analysis and Retrieval** [IEEE Trans. Multim., 2015, 17(11): 2008-2020] [[paper\]](https://ieeexplore.ieee.org/document/7277066)

  **Authors:** Lei Pang, Shiai Zhu, Chong-Wah Ngo

  **Introduction (English):** Existing affective computation research mostly focuses on single media (text or visual content), ignoring the multimodal nature of emotion expression. This paper proposes a deep multimodal learning method based on Deep Boltzmann Machine (DBM) to model non-linear relationships across visual, auditory, and textual modalities. Trained on unlabeled user-generated content (UGC), the model learns a joint multimodal representation that supports emotion prediction and cross-modal retrieval (e.g., video retrieval via text queries). Experiments show the compact joint representation complements hand-crafted features, improving performance in emotion classification and cross-modal retrieval.

#### 5.2 Disentangling Structure and Semantics for Generative Control

- **ShadowPlay2.5D: A 360-Degree Video Authoring Tool for Immersive Appreciation of Classical Chinese Poetry** [J. Comput. Cult. Herit., 2020, 13(1)] [[paper\]](https://dl.acm.org/doi/10.1145/3352590)

  **Authors:** Zhenjie Zhao, Xiaojuan Ma

  **Introduction (English):**To address the difficulty of creating VR 360-degree content for classical Chinese poetry appreciation, ShadowPlay2.5D—a sketch-based tool inspired by poetry-painting homology—enables novices to make 2.5D immersive videos in 10–15 minutes via an ink-painting repository and puppet-style animation.

- **From Writing to Painting: A Kinect-Based Cross-Modal Chinese Painting Generation System** [Proceedings of the 22nd ACM International Conference on Multimedia, 2014] [[paper\]](https://dl.acm.org/doi/10.1145/2647868.2654911)

  **Authors:** LI Jiajia, Grace Ngai, Stephen C.F. Chan, Kien A. Hua, Hong Va Leong, Alvin Chan

  **Introduction (English):** This paper presents CalliPaint, a Kinect-based cross-modal system linking Chinese ink brush calligraphy and landscape painting. Based on metaphoric congruence, it maps the two modalities to enable intuitive creation: novice users can generate attractive landscape paintings through calligraphy writing. Evaluations show it offers a more enjoyable and easy-to-learn experience than general digital painting software.

- **Generative Adversarial Text to Image Synthesis** [arXiv:1605.05396 [cs.NE], 2016; ICML 2016] [[paper\]](https://arxiv.org/abs/1605.05396)

  **Authors:** Scott Reed, Zeynep Akata, Xinchen Yan, Lajanugen Logeswaran, Bernt Schiele, Honglak Lee

  **Introduction (English):** Realistic text-to-image synthesis remains challenging. This work proposes a novel GAN architecture that combines discriminative text feature representations (from recurrent neural networks) with deep convolutional GANs. It bridges text and image modeling, generating plausible images (e.g., birds, flowers) from detailed text descriptions.

- **CogView: Mastering Text-to-Image Generation via Transformers** [arXiv:2105.13290 [cs.CV], 2021; NeurIPS 2021] [[paper\]](https://arxiv.org/abs/2105.13290)

  **Authors:** Ming Ding, Zhuoyi Yang, Wenyi Hong, Wendi Zheng, Chang Zhou, Da Yin, Junyang Lin, Xu Zou, Zhou Shao, Hongxia Yang, Jie Tang

  **Introduction (English):** General-domain text-to-image generation demands strong cross-modal understanding and generative capability. This work proposes CogView, a 4-billion-parameter Transformer integrated with a VQ-VAE tokenizer. It supports finetuning for downstream tasks (style learning, super-resolution, etc.) and adopts strategies to stabilize pretraining. CogView achieves state-of-the-art FID on blurred MS COCO, outperforming GAN-based models and DALL-E.

- **Unified Multi-Modal Latent Diffusion for Joint Subject and Text Conditional Image Generation** [arXiv:2303.09319 [cs.CV], 2023] [[paper\]](https://arxiv.org/abs/2303.09319)

  **Authors:** Yiyang Ma, Huan Yang, Wenjing Wang, Jianlong Fu, Jiaying Liu

  **Introduction (English):** Existing text-to-image models struggle to balance subject fidelity and text alignment. This paper proposes a unified multi-modal latent diffusion model that fuses subject (e.g., reference image) and text conditions. It introduces a cross-attention fusion module to align dual modalities, enabling high-fidelity generation of target subjects with text-guided styles/contexts, outperforming single-condition models.

- **Generative Adversarial Text to Image Synthesis** [arXiv:1605.05396 [cs.NE], 2016; ICML 2016] [[paper\]](https://arxiv.org/abs/1605.05396)

  **Authors:** Scott Reed, Zeynep Akata, Xinchen Yan, Lajanugen Logeswaran, Bernt Schiele, Honglak Lee

  **Introduction (English):** Realistic text-to-image synthesis remains challenging. This work proposes a novel GAN architecture that combines RNN-learned discriminative text features with deep convolutional GANs, bridging text and image modeling to generate plausible birds/flowers from detailed text descriptions.

- **FHS-adapter: Fine-Grained Hierarchical Semantic Adapter for Chinese Landscape Paintings Generation** [Herit. Sci., 2024, 12(1): 265] [[paper\]](https://www.nature.com/articles/s40494-024-01370-7)

  **Authors:** Xianlin Peng, Qiyao Hu, Fangqing Fan, Penglin Xie, Yihan Zhang, Rui Cao

  **Introduction (English):** Existing text-to-image models struggle to generate authentic Chinese landscape paintings due to insufficient fine-grained cultural guidance and mismatched style adaptation. This paper proposes FHS-adapter, a fine-grained hierarchical semantic adapter, and constructs the T2ICLP dataset (10,000 image-text pairs with Meta/Description/Sentiment/Poem prompts). It uses Taiyi-CLIP for Chinese semantic understanding and injects multi-perspective prompts into the U-Net cross-attention layers in a specific sequence. Experiments show it outperforms mainstream models in brushwork, composition, and antique style, with superior FID and CLIP-T scores.

- **A New Chinese Landscape Paintings Generation Model based on Stable Diffusion using DreamBooth** [arXiv:2408.08561 [cs.CV], 2024; AHPCAI] [[paper\]](https://arxiv.org/abs/2408.08561)

  **Authors:** Yujia Gu, Xinyu Fang, Xueyuan Deng, Zihan Peng, Yinan Peng

  **Introduction (English):** Generating high-fidelity Chinese landscape paintings requires domain-specific fine-tuning of diffusion models. This study proposes a model combining Stable Diffusion (SDM) with DreamBooth, accelerated by Parameter-Efficient Fine-Tuning. Compared to generic SDM and LoRA-fine-tuned SDM, it achieves a FID of 12.75 on a Chinese landscape painting dataset and outperforms others in expert evaluations, demonstrating strong versatility, fidelity, and quality for domain-specific generation.

- **Multimodal Fusion for Traditional Chinese Painting Generation** [Adv. Multimed. Inf. Process. – PCM 2018] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-030-00764-5_3)

  **Authors:** Sanbi Luo, Si Liu, Jizhong Han, Tao Guo

  **Introduction (English):** To address the challenge of AI-generated traditional Chinese paintings with creativity, this paper proposes a multimodal fusion framework integrating suitable networks for generating different painting elements. It adopts a divide-and-conquer strategy to handle large images under limited GPU resources, enabling automatic generation of complete traditional Chinese paintings in minutes.

- **An Interactive and Generative Approach for Chinese Shanshui Painting Document** [ICDAR, 2019, pp. 819-824] [[paper\]](https://ieeexplore.ieee.org/document/8978182)

  **Authors:** Le Zhou, Qiu-Feng Wang, Kaizhu Huang, Cheng-Hung Lo

  **Introduction (English):** Creating Chinese Shanshui paintings is challenging for non-professionals due to the need for specialized skills. This paper proposes an interactive generative approach based on cycle GAN: users input simple sketches, and the model translates them into Shanshui paintings. An interactive system (Shanshui-DaDA) is developed for real-time generation, trained on large sketch and Shanshui datasets. Experimental results confirm it satisfies general users’ needs.

- **Transform a Simple Sketch to a Chinese Painting by a Multiscale Deep Neural Network** [Algorithms, 2018, 11(1): 4] [[paper\]](https://www.mdpi.com/1999-4893/11/1/4)

  **Authors:** Daoyu Lin, Yang Wang, Guangluan Xu, Jun Li, Kun Fu

  **Introduction (English):** To address the limitation of deep learning-based image synthesis focusing on simple datasets, this paper proposes a multiscale deep neural network for converting sketches to Chinese paintings. It combines L1 loss and adversarial loss for training, enabling feed-forward controllable synthesis with both local details and global framework. The model can also serve as neural style transfer with an edge detector, and exhibits universality in image colorization and super-resolution.

- **Generating Chinese Classical Landscape Paintings Based on Cycle-Consistent Adversarial Networks** [ICSAI, 2019, pp. 1265-1269] [[paper\]](https://ieeexplore.ieee.org/document/9010358)

  **Authors:** XiaoXuan Lv, XiWen Zhang

  **Introduction (English):** CycleGAN has been used to convert photos to Western oil painting styles, but not yet for Chinese classical landscape paintings. This paper applies CycleGAN to this task, using a U-Net generator to save training time and L2 Loss to improve generation quality. Experiments on PyTorch with different style photos yield satisfactory Chinese classical landscape painting results.

- **ConCLVD: Controllable Chinese Landscape Video Generation via Diffusion Model** [arXiv:2404.12903 [cs.MM], 2024] [[paper\]](https://arxiv.org/html/2404.12903v1)

  **Authors:** Dingming Liu, Shaowei Li, Ruoyan Zhou, Lili Liang, Yongguan Hong, Fei Chao, Rongrong Ji

  **Introduction (English):** Static Chinese landscape paintings lack dynamic expression, and existing text-to-video models face challenges like scarce specialized datasets and poor style consistency. This paper proposes ConCLVD, a controllable diffusion model for Chinese landscape video generation, along with the CLV-HD dataset (1,300 text-video pairs). It integrates a motion module with dual attention mechanisms, latent space noise contrastive learning, and optical flow-based frame interpolation. The model runs on a single RTX 3090, achieving high temporal consistency and style fidelity, outperforming baselines in user studies.

- **DLP-GAN: Learning to Draw Modern Chinese Landscape Photos with Generative Adversarial Network** [Neural Comput. Appl., 2023, 36(10): 5267–5284] [[paper\]](https://arxiv.org/abs/2403.03456)

  **Authors:** Xiangquan Gui, Binxuan Zhang, Li Li, Yi Yang

  **Introduction (English):** Generating modern Chinese landscape photos requires capturing natural scenery and cultural context. This paper proposes DLP-GAN, a generative adversarial network integrating a dual-branch feature extraction module and landscape-aware loss. It learns texture details and spatial structure of modern Chinese landscapes, outperforming baseline GAN models in visual quality and similarity to real photos.

- **Ancient Painting to Natural Image: A New Solution for Painting Processing** [arXiv:1901.00224 [cs.CV] 2019] [[paper\]](https://arxiv.org/abs/1901.00224)

  **Authors:** Tingting Qiao, Weijing Zhang, Miao Zhang, Zixuan Ma, Duanqing Xu

  **Introduction (English):** To address the lack of large-scale annotated datasets for ancient Chinese painting processing, this paper proposes a Domain Style Transfer Network (DSTN) that converts ancient flower, bird, and landscape paintings to photo-realistic natural images. With a compound loss ensuring preserved color composition and content, the transferred images outperform state-of-the-art methods in human perceptual tests and downstream image processing tasks.

- **Mural Sketch Generation via Style-aware Convolutional Neural Network** [Comput. Graph. Int., 2018, pp. 239–245] [[paper\]](https://dl.acm.org/doi/10.1145/3208159.3208160)

  **Authors:** Gang Pan, Di Sun, Rui Zhan, Jiawan Zhang

  **Introduction (English):** Mural sketch generation requires preserving cultural style and structural fidelity. This paper proposes a style-aware CNN framework: it extracts content features from reference images and style features from mural samples, fuses dual features via adaptive normalization, and generates sketches consistent with mural artistic styles. Experiments validate the model’s effectiveness in style preservation and structural accuracy.

- **Outline Font Generating from Images of Ancient Chinese Calligraphy** [Transactions on Edutainment V, 2011, pp. 122-131] [[chapter\]](https://link.springer.com/chapter/10.1007/978-3-642-18452-9_10)

  **Authors:** Junsong Zhang, Guohong Mao, Hongwei Lin, Jinhui Yu, Changle Zhou

  **Introduction (English):** Preserving ancient Chinese calligraphy via outline font generation requires retaining calligraphic style and structural accuracy. This paper proposes a method: detect feature points from character boundaries using a calligrapher-specific statistical approach, smooth contours with Gaussian kernels (parameterized via linear regression from a stroke database), and fit contour segments with parametric curves to generate outline fonts.

#### 5.3 Bridging Semantic Structures Across Text and Visual Domains

- **iPoet: Interactive Painting Poetry Creation with Visual Multimodal Analysis** [J. Vis., 2022, 25(3): 671-685] [[paper\]](https://link.springer.com/article/10.1007/s12650-021-00780-0)

  **Authors:** Yingchaojie Feng, Jiazhou Chen, Keyu Huang, Jason K. Wong, Hui Ye, Wei Zhang, Rongchen Zhu, Xiaonan Luo, Wei Chen

  **Introduction (English):** Creating painting poetry for ancient Chinese paintings requires integrating visual content and emotional nuances, which is challenging for ordinary users. This paper proposes the iPoet interactive system: it uses object detection and image captioning to describe painting content, extends modern color theory to analyze emotions, and adopts an interactive poetry generation method. Visual components guide users to create personalized painting poetry, validated by case studies and user interviews.

- **Automatic Poetry Generation Based on Ancient Paintings** [J. Comput.-Aided Des. Comput. Graph., 2021, 33(7): 1038-1044] [[paper\]](https://www.jcad.cn/en/article/doi/10.3724/SP.J.1089.2021.18633)

  **Authors:** Jiazhou Chen, Keyu Huang, Yingchaojie Feng, Wei Zhang, Siwei Tan, Wei Chen

  **Introduction (English):** Generating poetry that aligns with ancient Chinese paintings’ content and artistic conception is non-trivial. This paper proposes a multi-modal framework: it extracts visual features (objects, colors, composition) and cultural semantics from paintings, fuses them with classical poetry templates, and uses a recurrent neural network (RNN) to generate context-consistent, stylistically authentic poetry. Experiments show the generated works outperform baseline models in relevance and literary quality.

- **Learning to Generate Poetic Chinese Landscape Painting with Calligraphy** [arXiv:2305.04719 [cs.CV], 2023] [[paper\]](https://arxiv.org/abs/2305.04719)

  **Authors:** Shaozu Yuan, Aijun Dai, Zhiling Yan, Ruixue Liu, Meng Chen, Baoyang Chen, Zhijie Qiu, Xiaodong He

  **Introduction (English):** Integrating calligraphy into poetic Chinese landscape paintings requires harmonizing visual style and cultural connotation. This paper proposes a multi-modal generation framework that fuses poetry, calligraphy, and landscape painting. It uses a cross-modal attention module to align poetic semantics, calligraphic style, and landscape composition, generating paintings with integrated calligraphy that matches the poetic artistic conception. Experiments validate the model’s effectiveness in style consistency and cultural integration.

- **Paint4Poem: A Dataset for Artistic Visualization of Classical Chinese Poems** [arXiv:2109.11682 [cs.CV], 2021] [[paper\]](https://arxiv.org/abs/2109.11682)

  **Authors:** Dan Li, Shuai Wang, Jie Zou, Chang Tian, Elisha Nieuwburg, Fengyuan Sun, Evangelos Kanoulas

  **Introduction (English):** Artistic visualization of classical Chinese poems lacks dedicated datasets for training text-to-image models. This work constructs Paint4Poem: it includes 301 high-quality manual poem-painting pairs (Feng Zikai’s works), 3,648 caption-painting pairs, and 89,204 automatic web-collected poem-painting pairs. Benchmark experiments with AttnGAN and MirrorGAN show the dataset supports style mimicry and pictorial quality but highlights room for improving semantic alignment between poems and paintings.

- **Poetry4painting: Diversified Poetry Generation for Large-Size Ancient Paintings Based on Data Augmentation** [Comput. Graph., 2023, 116: 206-215] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0097849323001577)

  **Authors:** Jiazhou Chen, Keyu Huang, Xinding Zhu, Xianlong Qiu, Haidan Wang, Xujia Qin

  **Introduction (English):** Generating diverse yet content-consistent poetry for large-size ancient paintings is challenging due to repeated local content. This paper proposes Poetry4painting: it uses CNN-LSTM to convert painting captions into poetry, and introduces four data augmentations (quantity/shape/surrounding/object) for online processing. An enlarged dataset (1500+ paintings, 7500+ captions) is built via semi-automatic annotation, balancing poetry diversity and conformity to painting content.

- **Text-to-Ink Painting Generation Method Based on Multi-Domain VQGAN** [J. Softw., 2023, 34(5): 2116] [[paper\]](https://www.jos.org.cn/jos/article/abstract/6769)

  **Authors:** Zelong Sun, Guoxing Yang, Jingyuan Wen, Nanyi Fei, Zhiwu Lu, Jirong Wen

  **Introduction (English):** Existing text-to-ink painting models struggle with insufficient style fidelity and semantic alignment. This paper proposes a multi-domain VQGAN-based method: it constructs a multi-scale ink painting dataset, uses a domain-adaptive VQGAN to learn fine-grained style features (e.g., brushwork, wash), and fuses text semantics via cross-modal attention. The model achieves superior style authenticity and content consistency compared to single-domain VQGAN and GAN-based baselines.

#### 5.4 Graph-Based Modeling for Cultural Reasoning and Interaction

- **"Writing Poems for You": A Visualization-Based Interactive Creation System for Chinese Classical Poetry** [J. Comput.-Aided Des. Comput. Graph., 2021, 33(9): 1318-1325]

  **Authors:** Yingchaojie Feng, Zihan Zhou, Wei Zhang, Siwei Tan, Ruimin Shao, Jiazhou Chen, Wei Chen

  **Introduction (English):** Creating personalized Chinese classical poetry requires integrating literary rules and user intentions, which is challenging for ordinary users. This paper proposes an interactive visualization system: it provides modular guidance for theme selection, rhythm adjustment, and imagery matching, visualizes poetic structure and semantic connections, and supports real-time modification. User studies confirm it lowers creation thresholds while ensuring poetic quality and cultural authenticity.

- **Feature Fusion based Cross-modal Retrieval for Traditional Chinese Painting** [ICCST, 2020, pp. 383-387] [[paper\]](https://www.researchgate.net/publication/347159383_Feature_Fusion_based_Cross-modal_Retrieval_for_Traditional_Chinese_Painting)

  **Authors:** Zhenhao Dong, Jing Wan, Chaoyue Li, Han Jiang, Yingge Qian, Wenxie Pan

  **Introduction (English):** Cross-modal retrieval (text-to-painting/painting-to-text) for traditional Chinese paintings (TCPs) faces challenges of cultural semantic gap and insufficient feature alignment. This paper proposes a feature fusion framework: it extracts visual features (color, texture, composition) via CNN and text features via BERT, fuses dual-modal features with an attention-based fusion module, and optimizes with triplet loss. Experiments on a TCP dataset show it outperforms single-modal and naive fusion methods in retrieval accuracy.

- **Extraction of Visual Elements from Dunhuang Frescoes Based on Image Segmentation Algorithm and Application to Modern Visual Communication Design in New Media Environment** [Int. J. High Speed Appl., 2025, 46(3): 1835–1844] [[paper\]](https://housingscience.org/volume-46-issue-3/extraction-of-visual-elements-from-dunhuang-frescoes-based-on-image-segmentation-algorithm-and-application-to-modern-visual-communication-design-in-new-media-environment/)

  **Authors:** Nan Shi, Yun Qiu

  **Introduction (English):** Extracting visual elements from Dunhuang frescoes for modern design requires high-precision segmentation while preserving cultural details. This paper proposes an enhanced edge segmentation framework: it combines Sobel-Canny edge enhancement with an improved GrabCut algorithm, and builds a visual semantic segmentation model via region suggestion network and full convolutional network. Experiments show it achieves PSNR of 22.35dB, SSIM of 0.735, and average running time of 5.25s, outperforming mainstream algorithms. User surveys confirm its recognition in functionality, usability, and cultural preservation.

- **Research on Chinese Painting Seal Recognition Based on EfficientNet and SIFT** [J. Beijing Univ. Chem. Technol. (Nat. Sci. Ed.), 2025, 52(4): 74-84] [[paper\]](https://journal.buct.edu.cn/EN/10.13543/j.bhxbzr.2025.04.009)

  **Authors:** Qingyang Zeng, Jing Wan, Hao Zhang

  **Introduction (English):** Seal recognition in Chinese paintings faces challenges like blurred images, scale/rotation variations, and complex backgrounds. This paper proposes a two-stage method: first, preprocess images (super-resolution, color correction, noise reduction), extract candidate seal regions via HSV color space, and classify with EfficientNet for precise extraction (95.25% accuracy). Second, use SIFT to extract invariant features for nearest-neighbor matching, achieving 98.20% matching accuracy and robust performance against scale/rotation changes.

- **Relic2Contour: Salient Contour Detection in Relics Using Semi-Supervised Generative Adversarial Networks Based on Knowledge Sharing** [npj Herit. Sci., 2025, 13(1): 84] [[paper\]](https://www.nature.com/articles/s40494-025-01606-0)

  **Authors:** Zhe Yu, Qingqing Kang, Jun Wang, Shenglin Peng, Qunxi Zhang, Yirong Ma, Shuyi Qu, Jinye Peng, Xianlin Peng

  **Introduction (English):** Extracting salient contours from cultural relics (e.g., murals, paintings) is hindered by pigment mottling, cracks, and limited paired data. This paper proposes Relic2Contour, a semi-supervised GAN framework with knowledge sharing: it integrates supervised (paired clean relics-contours) and unsupervised (diseased relics-unpaired contours) branches, plus contour generation/auxiliary gradient flows. The CAT module transfers spatial features, and Bi-GTF fuses dual flows. Experiments show it outperforms 6 SOTA methods in SSIM/RMSE/AP, generating clear contours for murals, landscape paintings, and painted pottery.

- **WuMKG: A Chinese Painting and Calligraphy Multimodal Knowledge Graph** [Herit. Sci., 2024, 12(1): 159] [[paper\]](https://www.nature.com/articles/s40494-024-01268-4)

  **Authors:** Jing Wan, Hao Zhang, Jun Zou, Ao Zou, Yubin Chen, Qingyang Zeng, Xinrong Li, Qiya Wang

  **Introduction (English):** Organizing scattered Chinese painting and calligraphy (ChP&C) data requires a unified multimodal knowledge graph. This paper proposes WuMKG, built on CIDOC CRM and Shlnames ontologies, integrating 104,374 entities and 418,450 triples (1,200 artists, 12,000 works). It extracts textual knowledge via LeBERT and visual knowledge (seals/subjects) via EfficientNet/EfficientDet, supporting cross-modal retrieval, Q&A, and visualization. Experiments validate the effectiveness of its knowledge extraction methods.

- **PaintKG: The Painting Knowledge Graph Using BiLSTM-CRF** [ICISE-IE, 2020, pp. 412-417] [[paper\]](https://ieeexplore.ieee.org/document/9418951)

  **Authors:** Han Wu, Shuo Yan Liu, Wenkai Zheng, Yifu Yang, Han Gao

  **Introduction (English):** Building a specialized knowledge graph for paintings helps organize discrete cultural relic data and facilitate knowledge sharing. This paper proposes PaintKG, which uses BiLSTM-CRF to extract entities (paintings, painters) and relations from unstructured web text and encyclopedia data. The extracted knowledge is stored in Neo4j as graph data, supporting applications like painting recommendation and painter association, with improved F1-measure for knowledge extraction.

- **Linking Past Insights with Contemporary Understanding: An Ontological and Knowledge Graph Approach to the Transmission of Ancient Chinese Classics** [Herit. Sci., 2024, 12(1): 382] [[paper\]](https://www.nature.com/articles/s40494-024-01504-x)

  **Authors:** Yu Cui, Shenjun Yao, Jianping Wu, Muhan Lv

  **Introduction (English):** Studying the transmission of ancient Chinese classics (ACCs) requires integrating historical versions, translation paths, and contemporary reception. This paper proposes ClaOnto, an ontology with three modules (Basic/Transmission/Evaluation Information) built on CIDOC CRM/[Schema.org/GeoNames](https://Schema.org/GeoNames). It constructs a knowledge graph via factual extraction (template matching), logic reasoning (SWRL), and algorithm-based analysis (LDA/sentiment analysis), demonstrated with the Tao Te Ching (2052 translations, 551 transmission relationships). The graph supports semantic retrieval and transmission path tracing.

- **A Survey of Techniques for Constructing Chinese Knowledge Graphs and Their Applications** [Sustainability, 2018, 10(9): 3245] [[paper\]](https://www.mdpi.com/2071-1050/10/9/3245)

  **Authors:** Tianxing Wu, Guilin Qi, Cheng Li, Meng Wang

  **Introduction (English):** Constructing Chinese knowledge graphs (CKGs) is critical for supporting Chinese-language intelligent applications. This survey systematically reviews CKG construction techniques, covering four core stages: knowledge extraction (from structured/semi-structured/unstructured data), knowledge integration (linking/fusion), knowledge quality improvement (completion/correction), and knowledge update (periodical/active). It also summarizes typical CKGs (Zhishi.me, CN-DBpedia, XLORE) and their applications in semantic search, QA, and intelligence analysis, with insights for cross-lingual knowledge graph development.

- **Hotspots and Trends of Research on Literati Painting and Scholar’s Painting in Art Education: An Analysis Based on CiteSpace Knowledge Graph** [ARTSEDUCA, 2023, 36(Original Article)] [[paper\]](https://artseduca.com/submissions/index.php/ae/article/view/91)

  **Authors:** Lang Qianwen, Lilian Lee Shiau Gee

  **Introduction (English):** This study analyzes research trends of literati painting and scholar’s painting in 2000-2022 using CiteSpace and CNKI literature. It constructs knowledge graphs (keyword co-occurrence, institution/author collaboration, emergent words) to identify hotspots: distinguishing the two painting types, sorting out scholar’s painting’s origin/period/style/painter personality. The results provide references for college art education, art history, and theory research.

- **An LLM-Based QA System for Chinese Painting and Calligraphy with Knowledge Graphs and External Documents** [npj Herit. Sci., 2025, 13(1): 643] [[paper\]](https://www.nature.com/articles/s40494-025-02219-3)

  **Authors:** Jing Wan, Xinrong Li, Hao Zhang, Ao Zou, Rumei Wang

  **Introduction (English):** Large Language Models (LLMs) suffer from hallucinations in domain-specific QA for Chinese Painting and Calligraphy (ChP&C). This paper proposes an LLM-based QA system integrated with Retrieval-Augmented Generation (RAG): it decomposes complex questions into sub-questions, retrieves structured knowledge from ChP&C KG (e.g., WuMKG) and unstructured knowledge from external documents (authoritative cultural heritage sources), then integrates answers via LLM. A dedicated CHPCQAD dataset (4055 samples) is constructed, and experiments show the system outperforms baselines in accuracy (52.31%) and zero-shot generalization, reducing hallucinations effectively.

### 6. Rhythmic Vitality: Global Aesthetic Coherence and Affective Modeling

#### 6.1 Computational Representation of Affective and Aesthetic Features

- **Emotional Valence Categorization Using Holistic Image Features** [ICIP, 2008, pp. 101-104] [[paper\]](https://ieeexplore.ieee.org/document/4711701)

  **Authors:** V. Yanulevskaya, J.C. van Gemert, K. Roth, A.K. Herbold, N. Sebe, J.M. Geusebroek

  **Introduction (English):** Evoking emotions is central to art, but machine perception of these emotions is challenging. We propose an emotion categorization system trained on IAPS (a standard psychological dataset with human-scored emotional valences). It leverages local image statistics learned via SVMs per emotional category, validated on IAPS and artistic masterpieces. Preliminary results demonstrate machines’ potential to perceive realistic emotions from art.

- **Emotion Distribution Prediction for Abstract Paintings Based on Weighted K-Nearest Neighbor** [J. Commun. Univ. China (Sci. Technol.), 2018, 25(1): 36-40] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=iwDheDcO5w4jbT0YUaNmOUZ0YTmAfV7PvhAjN16wklwwXtzM8yL5axZDB3xUO7FQME_A5keYkso9Hj2-H2MC57DReJ8QbII5m2TIcUUzaQ7fXMIyrI8RUUHj-UDZzJshIoEixScvSDHrU492yFkmztEtkc_7Zi8Z59SUh7FWJUDEJq5NWUIHhw==&uniplatform=NZKPT&language=CHS)

  **Authors:** Bo Li, Chen Guo, Hui Ren

  **Introduction (English):** Most existing image emotion computing focuses on category prediction, ignoring viewers’ subjective differences in emotional perception, which fails to meet practical needs. This paper proposes a weighted k-nearest neighbor (k-NN) method to predict discrete emotion distribution of abstract paintings. It first extracts emotional features of images, then predicts the corresponding emotion distribution for each image by weighting distances under different K values, and finally compares with the known emotion distribution of the dataset. Experiments on the Abstract image library validate the algorithm’s effectiveness.

- **Emotion Classification of Chinese Paintings Based on Convolutional Neural Networks and SVM** [J. Nanjing Norm. Univ. (Nat. Sci. Ed.), 2017, 40(3): 74-79, 86] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=iwDheDcO5w6PlJgZFdO3jkq1_suYkp3fmgJIk-vMUmaNAUTg_WMOaG2CWdITbbjD7VNVRePE9GGWq1oXfjfb1dLjwwdWQIjEHQicVIFYjkuC4PAk6cCRlr6cVKliV8iPXL5YZQjFjfDjBNoUYAvXCg8bvkUC7cguMWuX0bUquFckl9gPQtUYKg==&uniplatform=NZKPT&language=CHS)

  **Authors:** Zheng Wang, Haoyue Li, Hongshan Xu, Meijun Sun

  **Introduction (English):** Image emotion classification helps with image annotation and retrieval, boasting significant social and commercial value. Unlike Western paintings that "depict form through form," Chinese paintings emphasize expressing the artist’s subjective emotions rather than perspective, light-color changes, or literal resemblance—making it harder to bridge the gap between low-level features and high-level emotional semantics. This paper proposes a method combining CNN and SVM: CNN (with advantages of simple structure and adaptive feature extraction) directly processes raw Chinese painting images to avoid complex preprocessing, extracts features, which are then subjected to PCA dimensionality reduction and normalization. Finally, SVM classifies emotions by linking low-level features to emotional semantics.

- **An Emotion Classification Algorithm for Chinese Paintings Based on Deep Network Feature Aggregation and Recalibration** [J. Comput. Aided Des. Comput. Graph., 2020, 32(9): 1420-1429] [[paper\]](https://www.jcad.cn/en/article/doi/10.3724/SP.J.1089.2020.18005)

  **Authors:** Jiachuan Sheng, Yaqi Chen, Yanhong Han

  **Introduction (English):**Chinese paintings focus on emotional expression, which makes emotion classification difficult. This paper proposes an emotion classification algorithm based on deep network feature aggregation and recalibration. It uses seam carving to retain brushwork, aggregates and recalibrates deep features, and adopts multi-class weighted activation mapping for emotion visualization. Experiments show the method achieves high accuracy and effectively classifies emotions in Chinese paintings.

- **Emotion Recognition of Chinese Paintings at the Thirteenth National Exhibition of Fines Arts in China Based on Advanced Affective Computing** [Front. Psychol., 2021, 12: 741665] [[paper\]](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2021.741665/full)

  **Authors:** Jing Li, Dongliang Chen, Ning Yu, Ziping Zhao, Zhihan Lv

  **Introduction (English):** Chinese painting emotion recognition suffers from "semantic gap" and data redundancy/noise. This study proposes a multimodal model combining improved AlexNet (optimized for better generalization) and Chi Square Test (to remove redundancy/noise). Validated on Chinese paintings from the 13th National Exhibition of Fines Arts, it achieves 92.23% (training) and 97.11% (test) accuracy, with training/test time of 54.97s/23.74s. It outperforms LSTM, CNN, RNN, and DNN, supporting digital emotional management of traditional art.

- **Sentiment Analysis of Chinese Paintings Based on Lightweight Convolutional Neural Network** [Wireless Commun. Mob. Comput., 2021, 2021(1): 6097295] [[paper\]](https://onlinelibrary.wiley.com/doi/10.1155/2021/6097295)

  **Authors:** Jianying Bian, Xiaoying Shen

  **Introduction (English):** Chinese paintings are a core part of traditional Chinese culture. This paper proposes an optimized SqueezeNet-based lightweight CNN for their sentiment analysis: expanding the model width to extract more effective emotional features, and introducing residual network ideas to avoid gradient issues and enhance generalization. Comparative experiments on multi-theme Chinese paintings (four sentiment categories) confirm the model’s improved classification accuracy and generalization ability, supporting cultural protection, painting appreciation, and art education.

- **Computational Aesthetics Learning of Traditional Chinese Painting** [PhD Thesis, The University of Manchester, 2021] [[thesis\]](https://research.manchester.ac.uk/en/studentTheses/computational-aesthetics-learning-of-traditional-chinese-painting/)

  **Author:** Qianqian Gu

  **Supervisors:** David Morris (Main), Xiaojun Zeng (Co), Ross King (Co)

- **Introduction (English):** This PhD thesis presents a Computational Aesthetics Learning System for Traditional Chinese Painting (TCP), mimicking human visual processing of TCP and aesthetic information. It focuses on four core tasks: feature extraction/analysis, image classification, object detection, and neural style transfer, with key components including a hybrid image descriptor, SVM/VGG-based style classifiers, and an A-RPN detector (outperforming YOLO 2 and Faster R-CNN).

- **Research on Emotion Analysis of Chinese Literati Painting Images Based on Deep Learning** [Front. Psychol., 2021, 12: 723325] [[paper\]](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2021.723325/full)

  **Authors:** Jie Zhang, Yingjing Duan, Xiaoqing Gu

  **Introduction (English):** This study proposes a pure-image-based cross-cutting approach for Chinese literati painting emotion analysis using deep learning. It constructs a dedicated emotion dataset, tests five classic models to select the optimal one (ResNet50), and improves it to achieve 54.17% training accuracy. By visualizing salient feature areas in machine vision, it summarizes the connection between painting content and expressed emotions, validating the integration of deep learning with Chinese cultural research.
  
- **Design of Chinese painting style classification model based on multi-layer aggregation CNN** [PeerJ Comput. Sci., 2024, 10: e2303] [[paper\]](https://peerj.com/articles/cs-2303/)

  **Authors:** Xiaofang Du, Yangfeng Cai

  **Introduction (English):** To bridge the "emotional gap" between traditional Chinese painting (TCP) features and human emotions, this study proposes a CNN-based emotion classification model. It extracts emotional feature regions via image saliency, integrates a multi-layer aggregation recalibration module to enhance emotion-related feature activation, and adopts multi-category weighted activation localization in the CMYK color space. Experiments show it outperforms VGG-19, GoogLeNet, ResNet-50, and WSCNet, achieving 92.36% accuracy (max error 0.191) in TCP emotion recognition.

- **An End-to-End Weakly Supervised Learning Network Model for Emotion Recognition of Chinese Paintings** [J. Harbin Univ. Sci. Technol., 2022, 27(1): 69-78] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=zO3wb1M9ekwE1oirvj2OyckjsWYTKynuJJ8vB_jahtCQ6BEIjhBnLm3RnSnzNCHIMZ4hOUBTVL2qO-SMGFvgmuPHvJpw1VDOMCOK5ll5PS4tMSIXYanGiThGsr0722yFWPbH5T27N9stxBcX0APpNek-J_CeHXFF_ii7T5cbv9yYk1wqmVZNeg==&uniplatform=NZKPT&language=CHS)

  **Authors:** Kebin Lu, Shoulin Yin

  **Introduction (English):** Emotion recognition of Chinese paintings is vital for artwork appreciation. Traditional CNNs lose effective information when extracting local features. This study proposes an end-to-end weakly supervised learning network, consisting of two classification modules and one emotion intensity prediction module. It builds an intensity prediction channel via improved Feature Pyramid Network to extract multi-level features, generates pseudo-intensity maps through Grad-CAM from the first classification channel, and inputs them into the second channel for final recognition. Validated on public datasets, the model improves confusion matrix performance, average classification accuracy, and average emotion recognition rate by 10%, 15%, and 13% respectively.

- **Emotion Recognition of Chinese Paintings Optimized by Human Cognition Network Fusion** [Pattern Recognit. Artif. Intell., 2020, 33(2): 141]

  **Authors:** Jiachuan Sheng, Yaqi Chen, Jun Wang, Liang Li

  **Introduction (English):** To align Chinese painting emotion recognition with human cognitive patterns, this study proposes an optimized method via human cognition network fusion. It integrates cognitive mechanisms into the recognition framework, enhancing the model’s ability to capture emotional nuances consistent with human perception. Validated through experiments, the method improves the rationality and accuracy of Chinese painting emotion recognition, providing a new approach for bridging the gap between machine analysis and human aesthetic cognition.

- **Building Emotional Machines: Recognizing Image Emotions through Deep Neural Networks** [IEEE Trans. Multimed., 2018, 20(11): 2980-2992] [[paper\]](https://ieeexplore.ieee.org/document/8344491)

  **Authors:** Hye-Rin Kim, Yeong-Seok Kim, Seon Joo Kim, In-Kwon Lee

  **Introduction (English):** Images effectively convey emotions. This study focuses on high-level object and background semantic features (with objects highly correlated to emotions, backgrounds refining predictions). It builds a feedforward deep neural network fusing multi-level features, outputting continuous valence-arousal emotion values (more effective than discrete categories). Experiments validate the network’s effectiveness in image emotion prediction.

- **An Emotion-Embedded Visual Attention Model for Dimensional Emotion Context Learning** [IEEE Access, 2019, 7: 72457-72468] [[paper\]](https://ieeexplore.ieee.org/document/8721122)

  **Authors:** Yuhao Tang, Qirong Mao, Hongjie Jia, Heping Song, Yongzhao Zhan

  **Introduction (English):** Dimensional emotion recognition (valence-arousal) requires capturing temporal context and selective visual features. This study proposes an Emotion-Embedded Visual Attention Model (EVAM): deep CNN extracts facial features, GRU-based visual attention learns emotion context by focusing on key facial regions, and k-means discretizes prior emotions (embedded via MLP) to enhance prediction robustness. Validated on AVEC 2016/2017 datasets, EVAM outperforms classic LSTM with better CCC scores, demonstrating effectiveness in continuous emotion learning.

- **Tang and Song Ink Painting Context to Taoist Philosophy and Mikels' Emotion Classification** [PhD Thesis, Hanyang University, 2024] [[thesis\]](https://repository.hanyang.ac.kr/handle/20.500.11754/188994)

  **Author:** Zhang Qinyan

  **Advisor:** Albert Young Choi

  **Introduction (English):** This PhD thesis explores the connection between Tang-Song ink paintings, Taoist philosophy, and Mikels' emotion classification. It integrates Taoist concepts (geometric, color, white space, natural philosophy) as emotional scales, selects emotional stimuli from ink paintings (instead of whole-image feature extraction), and adopts MobileNet (lightweight CNN) for emotion quantification. The dataset (Tang-Song ink paintings, 9:1 train-test split, 4:6 positive-negative ratio) achieves 85% classification accuracy. The model is deployed as a web application, supporting hard/soft outputs and radar chart visualization, providing insights for modern ink painting innovation.

- **Semantic Representation and Emotional Awareness in Chinese Painting Viewing: Is There a Difference Between Landscape Painting and Figure Painting?** [Behav. Sci., 2025, 15(6): 790] [[paper\]](https://www.mdpi.com/2076-328X/15/6/790)

  **Authors:** Tinghu Kang, Ping Wang

  **Introduction (English):** To explore aesthetic processing differences between Chinese landscape and figure paintings, this study uses vocabulary generation tasks and Implicit Association Test (IAT) with high school students. Experiment 1 shows both genres elicit abundant content words, but figure paintings generate more emotional association words. Experiment 2 finds faster responses in incompatible joint tasks than compatible ones. Results indicate painting aesthetics involve automatic processes, with semantic representation and emotional awareness unaffected by genre—content processing dominates due to emotional arousal’s temporal characteristics.

- **Modeling Water Animation in the Style of Traditional Chinese Painting** [J. Comput. Aided Des. Comput. Graph., 2012, 24(7): 864-870] [[paper\]](https://www.jcad.cn/en/article/id/8343364f-5e02-489c-839d-af3a94b76be5)

  **Authors:** Fang Jianwen, Yu Jinhui, Zhang Junsong

  **Introduction (English):** Water is a key element in traditional Chinese paintings, but stylized water simulation remains understudied. This paper proposes a Chinese painting-style water animation model: basic shapes are constructed via Bézier curves, ripples are generated by connecting these shapes and placed on a procedurally built water surface. Animation controls ripple arrangement, directional movement, and dynamic behaviors; line color and width vary with depth to enhance layering. Experiments show the model can generate diverse Chinese painting-style water animations.

#### 6.2 Stylistic Disentanglement and Aesthetic Differentiation

- **Rhythmic Brushstrokes Distinguish van Gogh from His Contemporaries: Findings via Automated Brushstroke Extraction** [IEEE Trans. Pattern Anal. Mach. Intell., 2012, 34(6): 1159-1176] [[paper\]](https://ieeexplore.ieee.org/document/6042878)

  **Authors:** Jia Li, Lei Yao, Ella Hendriks, James Z. Wang

  **Introduction (English):** Van Gogh’s distinctive brushstrokes are key for authentication and dating, but automated analysis is lacking. This study proposes a brushstroke extraction method integrating edge detection and clustering-based segmentation. Statistical analysis of massive extracted brushstrokes reveals van Gogh’s works feature strong rhythmicity—regularly shaped brushstrokes arranged tightly in repetitive patterns. These unique brushwork traits persist across his French periods (1886-1890) and distinguish him from contemporaries, with period-specific distinguishing traits differing from inter-artist ones.

- **Analysis of Painting Complexity Based on Feature Extraction** [2022 4th Int. Conf. Adv. Comput. Technol. Inf. Sci. Commun. (CTISC), Suzhou, China, 2022, pp. 1-5] [[paper\]](https://ieeexplore.ieee.org/document/9849770)

  **Authors:** Tingting Zhang, Shuang Xiao, Wei Zhou, Ling Xia, Jinwei Xie, Xiaofeng Liu

  **Introduction (English):** To quantify painting complexity and its relation to aesthetic value/image processing difficulty, this study classifies artwork features into stroke, color, and texture categories. Taking Picasso’s paintings as examples, two complexity prediction models are proposed. Experimental results confirm that stroke features are the most significant factor influencing painting complexity, providing a quantitative basis for aesthetic evaluation and image processing task design.

- **Computational Aesthetics: On the Complexity of Computer-Generated Painting** [Leonardo, 2012, 45: 243-248] [[paper\]](https://muse.jhu.edu/pub/6/article/475456/pdf)

  **Authors:** Zhang Kang, D. Fox Harrell, Ji Xin

  **Introduction (English):** Focusing on computational aesthetics of computer-generated paintings, this study explores the relationship between work complexity and aesthetic experience. It analyzes how algorithmic design (e.g., generative rules, parameter adjustments) shapes visual complexity, and discusses quantitative evaluation methods for complexity. The research provides insights into optimizing computer-generated artworks’ aesthetic value and enriches the theoretical system of computational aesthetics.

- **Analysis and Classification of Aesthetic Characteristics in Chinese Traditional Painting Art** [J. Beihang Univ., 2019, 45(12): 2514-2522] [[paper\]](https://html.rhhz.net/BJHKHTDXXBZRB/20191220.htm)

  **Authors:** Zhan Ying, Gao Yan, Xie Lingyun

  **Introduction (English):** To realize quantitative analysis and automatic classification of Chinese painting aesthetics, this study constructs a database of 511 Chinese paintings annotated with 5 aesthetic categories (majestic, serene, vibrant, elegant, bleak) and their intensity. Through feature extraction (covering color, brushwork, brightness, lines, etc.) and recursive feature elimination, 33 optimal features are selected. Experiments on 8 classifiers (Extra-Trees, SVM, etc.) via 10-fold cross-validation confirm the feasibility of automatic aesthetic classification. Results show color is the most influential artistic element, followed by brushwork, brightness, and lines.

- **A Comprehensive Survey on Computational Aesthetic Evaluation of Visual Art Images: Metrics and Challenges** [IEEE Access, 2021, 9: 77164-77187] [[paper\]](https://ieeexplore.ieee.org/document/9439479/)

  **Authors:** Jiajing Zhang, Yongwei Miao, Jinhui Yu

  **Introduction (English):** This comprehensive survey focuses on computational aesthetic evaluation of visual art images (photographs, paintings). It first summarizes benchmark datasets for aesthetic assessment across categories, then reviews conventional handcrafted feature-based methods and recent deep learning techniques (for scoring, distribution, attribute, and description-oriented aesthetic prediction). Additionally, it discusses practical applications: aesthetic-aware color enhancement, photo recomposition, and automatic generation of aesthetic-guided art paintings. Finally, current challenges and future research directions are analyzed, serving as a comprehensive reference for computational aesthetics in visual media.

#### 6.3 Designing Human-Centric Affective Experiences

- **A Real-Time ProCam System for Interaction with Chinese Ink-and-Wash Cartoons** [2007 IEEE Conf. Comput. Vis. Pattern Recognit. (CVPR), Minneapolis, MN, USA, 2007, pp. 1-2] [[paper\]](https://ieeexplore.ieee.org/document/4270478/)

  **Authors:** Ming Jin, Hui Zhang, Xubo Yang, Shuangjiu Xiao

  **Introduction (English):** To innovate the appreciation of Chinese ink-and-wash cartoons, this study develops a real-time ProCam (projector-camera) interactive system. It integrates GPU-accelerated real-time water simulation, computer vision-based sensing subsystem, and Chinese-stylized rendered elements (e.g., fish). Users can interact with static painting elements (water, fish, lotus) by stirring virtual water, creating vivid, immersive experiences that traditional static exhibitions cannot achieve, promoting the dissemination of Chinese traditional culture.

- **Annotating traditional Chinese paintings for immersive virtual exhibition** [J. Comput. Cult. Herit., 2012, 5(2): 1-12] [[paper\]](https://dl.acm.org/doi/10.1145/2307723.2307725)

  **Authors:** Wei Ma, Yizhou Wang, Ying-Qing Xu, Qiong Li, Xin Ma, Wen Gao

  **Introduction (English):** To address the unique characteristics of traditional Chinese paintings (long scroll form, moving focus composition without rigorous perspective), this study proposes an annotation method integrating voice dubbings and environmental sounds for immersive virtual exhibitions. A novel algorithm infers the 3D space of paintings based on their layout to embed audio annotations. The paintings are scanned into high-resolution gigapixel images to preserve details, and an interactive multimedia system with panning/zooming functions enables smooth navigation. During interaction, the system estimates the user’s 3D viewpoint in real time and synthesizes a realistic stereo audio field based on the viewer’s orientation and distance from annotations, achieving visual-audio consistency and immersive experiences.

- **Immersive Spring Morning in the Han Palace: Learning Traditional Chinese Art Via Virtual Reality and Multi-Touch Tabletop** [Int. J. Hum.-Comput. Interact., 2021, 38: 1-14] [[paper\]](https://kns.cnki.net/kcms2/article/abstract?v=zO3wb1M9ekyDP1zs7F3xuc9noioX0lls-4vLfq-eqDKHKnq3CVKdheQrH9rE9VzAQsG6oB2tXzvgLmrPKLwXakyc80W-77yyY8ygcMlNC98D7nQhfxbdHPFs4BKJuvT4zmrL0Du99zRughFB1aDDYKwerURAc0SchLtRS41Y8Md-FxKqqRkmrqsQMlD0tzv_l2GBylfumPAysFKIUNezGg==&uniplatform=NZKPT&language=CHS)

  **Authors:** Jin Sheng, Fan Min, Aynur Kadir

  **Introduction (English):** To explore effective ways of learning traditional Chinese art, this study compares the learning experience of 54 young adults (in pairs) using immersive virtual reality (IVR) and multi-touch tabletop (MTT). IVR is applied to learn *Spring Morning in the Han Palace*, while MTT is used for *The Night Revels of Han Xizai*. Mixed methods (knowledge assessments, questionnaires, observation, interviews) are adopted. Results show IVR significantly improves learning effectiveness and motivation, especially in detail recall and spatial-related tasks. The IVR system includes five learning scenes, enabling users to develop exploratory/embodied learning strategies, quickly focus on core content, and achieve equitable collaborative interactions, providing insights for traditional cultural heritage learning design.

- **Reconstructing Traditional Chinese Paintings with Immersive Virtual Reality** [Extended Abstracts of the 2020 CHI Conf. Hum. Factors Comput. Syst. (CHI EA '20), Honolulu, HI, USA, 2020, pp. 1-8] [[paper\]](https://dl.acm.org/doi/fullHtml/10.1145/3334480.3382934)

  **Authors:** Sheng Jin, Min Fan, Yongchao Wang, Qi Liu

  **Introduction (English):** To innovate the learning and experience of traditional Chinese paintings, this study designs an immersive virtual reality (VR) environment based on head-mounted displays (HMD) for reconstructing *Spring Morning in the Han Palace*. The design fully considers key factors affecting the learning experience, including the restoration of the painting’s art style, enhanced interpretation of cultural connotations, and interactive design strategies. The research also outlines future plans to conduct user studies with young undergraduate students, aiming to verify the effectiveness of VR in cultural heritage learning and provide insights for related design practices.

- **Research on the Reconstruction of Artistic Conception of Traditional Chinese Landscape Painting Based on VR Immersive Interaction** [Culture and Computing, HCII 2025, Lecture Notes in Computer Science, vol. 15800, Springer, Cham, 2025, pp. 341-356] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-031-93160-4_22)

  **Authors:** Xin Wang, Chul Soo Kim

  **Introduction (English):** Traditional Chinese landscape painting embodies profound cultural, philosophical, and emotional meanings, adhering to the spatial construction concept of "accessible, viewable, habitable, and tourable." However, 2D expression limits viewers’ full perception of its artistic conception. Based on embodied cognition theory, this study proposes an immersive interaction model that leverages multisensory interaction to enhance immersion and emotional resonance. Taking *Dwelling in the Fuchun Mountains* as a case, a virtual landscape space is constructed for 3D reconstruction and interactive experiences. Experimental results confirm that VR technology effectively deepens viewers’ understanding of the painting’s artistic conception, offering new ideas for the digital presentation of traditional art and expanding possibilities for cultural heritage preservation and artistic innovation.

- **Enhancing the Appreciation of Traditional Chinese Painting Using Interactive Technology** [Multimodal Technol. Interact., 2018, 2(2): 16] [[paper\]](https://www.mdpi.com/2414-4088/2/2/16)

  **Authors:** Shichao Zhao, David Kirk, Simon Bowen, Peter Wright

  **Introduction (English):** To address cross-cultural appreciation challenges of traditional Chinese painting, this study conducts a two-part research: a cultural appreciation study exploring cross-cultural aesthetic approaches, and a design-led study developing a tablet application. The app integrates an elemental archive (colors, subjects, textures) and multi-touch gestures, supporting users in self-expression and collaborative creation by combining painting elements. Results show non-Chinese audiences prefer this interactive approach—colours and subjects serve as effective entry points, while gestural interaction and collaborative engagement deepen aesthetic understanding without requiring drawing skills, providing transferable insights for HCI in cultural heritage appreciation.

- **Unveiling an Interactive and Immersive Virtual Reality Experience Through Digital Construction of a Historical Landscape Painting** [Master’s Thesis, Iowa State University, 2024] [[thesis\]](https://www.design.iastate.edu/gallery-181/unveiling-an-interactive-and-immersive-virtual-reality-vr-experience-through-digital-construction-of-a-historical-landscape-painting/)

  **Author:** Hang Yuan

  **Introduction (English):** This master’s thesis integrates Northern Song Dynasty landscape paintings (celebrated for sophisticated brushwork and nature appreciation) with virtual reality (VR) technology. It creates an interactive and immersive VR experience through digital construction, featuring digital reproductions of historical landscape paintings, 3D-printed characters from the works, and interactive elements (flowers, fish, boats, bridges) that allow viewers to engage directly. The project bridges ancient Chinese culture and modern technology, recontextualizes historical art, and enables personal connections between audiences and the cultural richness of the Northern Song Dynasty.

- **From Writing to Painting: A Kinect-Based Cross-Modal Chinese Painting Generation System** [Proceedings of the 22nd ACM International Conference on Multimedia, 2014] [[paper\]](https://dl.acm.org/doi/10.1145/2647868.2654911)

  **Authors:** LI Jiajia, Grace Ngai, Stephen C.F. Chan, Kien A. Hua, Hong Va Leong, Alvin Chan

  **Introduction (English):** This paper presents CalliPaint, a Kinect-based cross-modal system linking Chinese ink brush calligraphy and landscape painting. Based on metaphoric congruence, it maps the two modalities to enable intuitive creation: novice users can generate attractive landscape paintings through calligraphy writing. Evaluations show it offers a more enjoyable and easy-to-learn experience than general digital painting software.

- **METHODS FOR THE PRESERVATION AND RESTORATION OF DUNHUANG WALL PAINTINGS: FOREIGN EXPERIENCE** [Int. J. Conserv. Sci., 2024, 15: 731-748] [[paper\]](https://www.researchgate.net/publication/379866808_METHODS_FOR_THE_PRESERVATION_AND_RESTORATION_OF_DUNHUANG_WALL_PAINTINGS_FOREIGN_EXPERIENCE)

  **Authors:** Shiru Wang, Ion Sandu, Yulia Ivashko

  **Introduction (English):** Focusing on the preservation and restoration of Dunhuang wall paintings, this study systematically summarizes foreign experience and applicable methods. It analyzes key challenges such as pigment fading, mural detachment, and environmental damage, and reviews advanced foreign technologies including non-invasive material analysis, micro-consolidation techniques, environmental control systems, and digital preservation approaches. The research compares the advantages and limitations of different methods in adapting to Dunhuang’s unique cultural relic characteristics and environmental conditions, providing valuable references for optimizing the preservation and restoration practices of Dunhuang wall paintings and promoting international academic exchange in cultural heritage protection.

- **Computable Classification and Evaluation of Image Aesthetics** [J. Comput. Aided Des. Comput. Graph., 2014, 26(7): 1075-1083] [[paper\]](https://www.jcad.cn/en/article/id/863e9f67-6bb0-4e28-ad32-6caffa294b38)

  **Authors:** Weining Wang, Jingjian Yi, Xiangmin Xu, Li Wang

  **Introduction (English):** To realize computable analysis of image aesthetics, this study proposes a classification and evaluation framework for image aesthetics. It extracts multi-dimensional visual features (including color harmony, composition balance, texture richness, etc.), constructs an aesthetic evaluation index system, and designs a computable model for aesthetic classification and scoring. Validated on a self-built image dataset and public datasets, the model achieves effective classification of aesthetic levels and accurate prediction of aesthetic scores, providing technical support for applications such as intelligent image editing, aesthetic retrieval, and artistic creation assistance.

- **Aesthetic Visual Quality Assessment of Paintings** [IEEE J. Sel. Top. Signal Process., 2009, 3(2): 236-252] [[paper\]](https://ieeexplore.ieee.org/document/4799314)

  **Authors:** Congcong Li, Tsuhan Chen

  **Introduction (English):** To address the subjectivity of painting aesthetic evaluation, this study frames it as a machine learning task, proposing a method to assess the aesthetic visual quality of digital painting images. Features are extracted based on art theory and questionnaire-derived human judgment factors, covering both global and local characteristics of paintings. A dataset of painting images with human aesthetic scores is constructed for training and testing. Experimental results show the model can classify high/low aesthetic quality paintings with performance comparable to humans, establishing a computational link between human aesthetic perception and visual features of paintings.

- **A Multimodal Visual Analysis Approach for the Authentication of Ancient Chinese Paintings** [J. Comput. Aided Des. Comput. Graph., 2025, 37(4): 713-724] [[paper\]](https://www.jcad.cn/en/article/doi/10.3724/SP.J.1089.2023-00350)

  **Authors:** Xiaojiao Chen, Yonghao Chen, Tan Tang, Xin Ge, Ruihan Wang, Yifan Wang, Xiaosong Wang

  **Introduction (English):** To address the limitations of traditional authentication of ancient Chinese paintings (reliance on expert experience) and deep learning-based methods (black-box nature, poor human-machine collaboration), this study proposes a multimodal visual analysis approach. First, ancient painting images are semantically segmented into three categories: inscriptions, seals, and painting content. Then, image matching and text recognition are used to construct association structures between corresponding segments of different paintings and with relevant literary references. Finally, experts select painting segments to generate a multimodal semantic network graph for verification. A human-machine collaborative auxiliary authentication system is also developed. Expert evaluations using a 5-point Likert scale (scores 0.78-1.78) confirm the method’s efficiency and accuracy in ancient painting analysis and authentication.

#### 6.4 Generative Models Guided by Emotional and Stylistic Priors

- **Inkthetics: A Comprehensive Computational Model for Aesthetic Evaluation of Chinese Ink Paintings** [IEEE Access, 2020, 8: 225857-225871] [[paper\]](http://www.cad.zju.edu.cn/home/jhyu/Papers/Inkthetics.pdf)

  **Authors:** Jiajing Zhang, Yongwei Miao, Junsong Zhang, Jinhui Yu

  **Introduction (English):** Aiming at the lack of targeted computational aesthetic evaluation models for Chinese ink paintings, this study proposes a comprehensive framework named Inkthetics. First, a benchmark dataset of 1200 Chinese ink paintings (covering 6 themes) with professional aesthetic ratings is constructed. Then, a Deep Multi-View Parallel Convolutional Neural Network (DMVCNN) is designed to extract global attribute features (ink color, texture, composition) and adaptive local patch features. Finally, 77 handcrafted features (based on art expert knowledge of ink color, brushwork, and composition) are fused with deep learning features to build a comprehensive evaluation model via Support Vector Regression (SVR). Experimental results show the model achieves a Pearson correlation coefficient of 0.843 with human aesthetic judgments, outperforming existing methods and verifying its effectiveness in quantitative evaluation of Chinese ink paintings.

- **Adaptive Computational Aesthetic Evaluation of Chinese Ink Paintings Based on Deep Learning** [J. Comput. Aided Des. Comput. Graph., 2021, 33(9): 1349-1360] [[paper\]](https://www.sciengine.com/JCADC/doi/10.3724/SP.J.1089.2021.18815)

  **Authors:** Jiajing Zhang, Jinhui Yu, Yongwei Miao, Peng Ren

  **Introduction (English):** To address the gap in quantitative aesthetic evaluation of Chinese ink paintings (most existing studies focus on photographs and oil paintings), this study proposes an adaptive computational aesthetic evaluation framework based on deep learning. First, a benchmark dataset for aesthetic evaluation of Chinese ink painting images is constructed. Then, according to the aesthetic principles of Chinese ink paintings, global images and local patches are extracted as multi-channel inputs, and a multi-view parallel deep convolutional neural network (with 6 parallel subject convolution groups) is designed to extract deep aesthetic features. Finally, an adaptive deep aesthetic evaluation model is built based on a subject query mechanism. Experimental results show that the proposed multi-view network outperforms the basic VGG16 architecture; the extracted deep aesthetic features are significantly superior to traditional handcrafted features. The adaptive model achieves a highly significant Pearson correlation of 0.823 with human aesthetic evaluations (MSE = 0.161). Interference experiments confirm the network’s sensitivity to three key painting elements: composition, ink color, and texture.

- **Computational Aesthetic Evaluation of Chinese Ink Paintings** [J. Softw., 2016, 27(S2): 220-233] [[paper\]](http://www.cad.zju.edu.cn/home/jhyu/Papers/水墨画审美-软件学报.pdf)

  **Authors:** Jiajing Zhang, Peng Ren, Jian Wang, Jinhui Yu

  **Introduction (English):** As computational aesthetics gains traction, existing research primarily focuses on photographs and oil paintings, neglecting Chinese ink paintings—whose visual features (dominated by ink and supplemented by colors) differ significantly. This study proposes the first computational aesthetic evaluation framework for Chinese ink paintings. It extracts 29 features across three dimensions: color (hue contrast, color-white background contrast, etc.), composition, and texture. Validated on 60 Qi Baishi’s ink paintings, the framework uses linear regression to correlate computed features with human aesthetic scores. Experimental results show a Pearson correlation coefficient of 0.949 between the model’s evaluations and human judgments, providing a foundational reference for ink painting aesthetic assessment and exploring the link between human perception and computable visual features.

- **EmoGraphArt: A Knowledge Graph for Representing and Explaining Emotions in Abstract Paintings** [MAI-XAI@ECAI, CEUR Workshop Proc., vol. 3803, 2024] [[paper\]](https://ceur-ws.org/Vol-3803/paper9.pdf)

  **Authors:** Rafael Berlanga Llavori, Dolores María Llidó, María José Aramburu Cabo

  **Introduction (English):** To address the lack of explainable emotion representation in abstract paintings, this study proposes EmoGraphArt—a framework integrating a logical model and knowledge graph (KG) for explaining emotions evoked by visual stimuli. Based on Lazarus’ appraisal theory (emotions stem from stimulus rationalization), the KG connects three core components: visual stimuli (colors, shapes, textures), annotator appraisals, and evoked emotions. Experiments use the FeelingBlue dataset (912 abstract paintings with emotion rationales), mapping text rationales, image features, and emotion labels to the KG. The framework enables extracting patterns (e.g., emotion opposites, stimulus-emotion correlations) via queries, verifying the feasibility of explaining abstract art emotions through structured knowledge representation.

- **Simulating Aging and Reverse-Aging Phenomena of Traditional Chinese Paintings** [Proc. Annu. Conf. Jpn. Soc. Artif. Intell. (JSAI) 2012] [[paper\]](https://www.jstage.jst.go.jp/article/pjsai/JSAI2012/0/JSAI2012_4M1IOS3c5/_article/-char/ja/)

  **Authors:** Lieu-Hen Chen, Meng-Feng Tsai, Chien-Hui Hsu, Yu-Sheng Chen

  **Introduction (English):** Conventional image processing techniques for simulating painting aging and restoration are overly simplistic, failing to consider storage conditions, pigment/surface material status, and historical color trends. This leads to unrealistic results in both aging simulation of contemporary works and reverse-aging (restoration) of old paintings. To address this, the paper proposes a knowledge-based approach: it discovers color fading knowledge over time by collecting, categorizing, and analyzing paintings from different eras, and tracks relationships between color distribution histograms, painting subjects, creation dynasties, and pigment properties. The prototype system enables simulation of both aging and reverse-aging processes, with initial results verifying its potential for realistic aging effects on traditional Chinese paintings.

- **Ink Restorer: Virtual Restoration of Ancient Chinese Paintings Inheriting Traditional Restoration Processes** [CHI '25: Proc. 2025 CHI Conf. Hum. Factors Comput. Syst., 2025] [[paper\]](https://dl.acm.org/doi/10.1145/3706598.3714190)

  **Authors:** Ying Zhang, Zejian Li, Jiesi Zhang, Fang Hu, Kewen Zhu, Qi Liu, Huanghuang Deng, Xiaoyu Chen, Lingyun Sun

  **Introduction (English):** To address the inaccessibility of traditional Chinese painting restoration (high professional threshold, time-consuming) and the lack of cultural inheritance in existing AI restoration tools, this study proposes Ink-Restorer—a virtual restoration tool that inherits the four traditional stages: Xi (washing), Jie (separating), Bu (mending), and Quan (completing). The tool integrates SAM (Segment Anything Model) for precise missing area segmentation, Stable Diffusion XL (finetuned with LoRA) for content inpainting, and Unity-based interactive interfaces to simulate professional restoration operations. A formative study (expert interviews + 306 public questionnaires) confirms public interest in virtual restoration and expert demands for cultural integration. A user study with 60 novices shows Ink-Restorer outperforms two baselines (w/o AI, w/o traditional stages) in UEQ/USE scores, and expert evaluations verify its superiority in cultural connotation and restoration quality (e.g., detail consistency, style coherence).

- **Computational Aesthetics of Visual Artworks: Review and Outlook** [Cognitive Computing and Internet of Things, AHFE Int. Conf. Proc., vol. 43, AHFE International, USA, 2022] [[paper\]](https://openaccess.cms-conferences.org/publications/book/978-1-958651-19-3/article/978-1-958651-19-3_1)

  **Authors:** Pu Meng, Yueqi Liu, Liqun Zhang, Xiaodong Li

  **Introduction (English):** As a cross-discipline integrating mathematics, computer science, and art, computational aesthetics aims to quantify and analyze the aesthetic properties of visual artworks. This study provides a comprehensive review and outlook on computational aesthetics of visual artworks. It classifies aesthetic features into five categories: visual (color, texture, shape), compositional (layout, balance, spatial structure), statistical (feature distribution, correlation), perceptual (human subjective perception-related), and artistic (style, cultural connotation, creative intention). The review points out that existing research mainly focuses on static aesthetic evaluation of completed artworks, failing to reflect the continuous process of artistic creation. With the emergence of new art forms such as generative art, the paper prospects future research directions for computational aesthetic evaluation algorithms adapted to these new forms, offering a systematic reference for the development of the field.

- **Computational Aesthetics of Fine Art Paintings: The State of the Art and Outlook** [Zidonghua Xuebao/Acta Automatica Sinica, 2020, 46: 2239-2259] [[paper\]](https://www.researchgate.net/publication/355382765_Computational_Aesthetics_of_Fine_Art_Paintings_The_State_of_the_Art_and_Outlook)

  **Authors:** Y. Lu, Chao Guo, Y.-L Lin, F. Zhuo, F.-Y Wang

  **Introduction (English):** As an interdisciplinary field integrating computer science, art, and psychology, the computational aesthetics of fine art paintings aims to simulate human aesthetic processes through machine computation. For the first time, this study systematically categorizes the field into three core research directions aligned with human aesthetic mechanisms (perception, cognition, evaluation): attribute recognition (e.g., style, brushstroke, pigment identification), content understanding (e.g., subject, composition, cultural connotation analysis), and aesthetic judgment (e.g., quality evaluation, emotional tendency prediction). It summarizes key scientific issues in each direction, including problem modeling, dataset construction, and cutting-edge methods (traditional machine learning, deep learning), compares the characteristics and application scenarios of the three research contents, and discusses future trends such as cross-modal fusion, cultural knowledge integration, and dynamic aesthetic process modeling, providing a comprehensive theoretical framework for the development of fine art painting computational aesthetics.

- **Deep Learning Based Image Aesthetic Quality Assessment - A Review** [ACM Comput. Surv., 2025, 57(7)] [[paper\]](https://dl.acm.org/doi/10.1145/3716820)

  **Authors:** Maedeh Daryanavard Chounchenani, Asadollah Shahbahrami, Reza Hassanpour, Georgi Gaydadjiev

  **Introduction (English):** This comprehensive review focuses on deep learning-based Image Aesthetic Quality Assessment (IAQA) over the past decade, structured around three core phases: input, process, and output. Input methods are categorized into general and task-specific approaches based on image type and diversity. The processing phase covers network architectures, learning structures, and feature extraction techniques. Output results include scoring, distribution, attributes, and description. Despite state-of-the-art models achieving up to 91.5% accuracy, the review highlights key challenges: adapting to task-specific methodologies, accounting for environmental factors affecting aesthetics, scarcity of large-scale labeled datasets, data imbalance, preserving image aspect ratio/integrity in network design, and the need for explainable AI to clarify aesthetic judgment mechanisms. The work provides a systematic overview of IAQA’s development and directions for future research.

- **Towards Artistic Image Aesthetics Assessment: a Large-scale Dataset and a New Method** [2023 IEEE/CVF Conf. Comput. Vis. Pattern Recognit. (CVPR), Vancouver, BC, Canada, 2023] [[paper\]](https://ieeexplore.ieee.org/document/10205454)

  **Authors:** Ran Yi, Haoyuan Tian, Zhihao Gu, Yu-Kun Lai, Paul L. Rosin

  **Introduction (English):** To address the lack of large-scale datasets and targeted methods for Artistic Image Aesthetics Assessment (AIAA), this study proposes two core contributions: the Boldbrush Artistic Image Dataset (BAlD) and the Style-specific Art Assessment Network (SAAN). BAlD contains 60,337 artistic images covering diverse art forms, annotated with over 360,000 user votes to ensure reliable aesthetic labels. SAAN is designed to extract both style-specific and generic aesthetic information, enabling effective evaluation of artistic images by adapting to the unique characteristics of different art styles. Quantitative experiments verify that SAAN outperforms existing general image aesthetics assessment (IAA) methods on BAlD, providing a foundational dataset and technical framework for future AIAA research.

## Datasets<a id="datasets"></a>

- **AVA: A large-scale database for aesthetic visual analysis**[CVPR 2012] [[paper]](https://ieeexplore.ieee.org/document/6247954)[[dataset]](https://snalyami.github.io/Isharah_CSLR/)

  **Authors:** Murray Naila , Marchesotti Luca, Perronnin Florent

  **Introduction:**Given the growing need to organize visual content by aesthetic preference and the potential of computational aesthetic preference models (still in early stages), this paper introduces the large-scale AVA database (over 250,000 images with rich metadata) that outperforms existing ones in scale, diversity and annotation heterogeneity, presents key insights from it, and demonstrates its ability to improve performance on existing preference tasks via three applications.
  
- **JenAesthetics Subjective Dataset: Analyzing Paintings by Subjective Scores** [Computer Vision - ECCV 2014 Workshops, Lecture Notes in Computer Science, vol. 8925, Springer, Cham, 2015, pp. 3-19] [[paper\]](https://link.springer.com/chapter/10.1007/978-3-319-16178-5_1)[[dataset\]]([https://github.com/Bin-ary-Li/JenAesthetics/tree/master/JenAesthetics%20subjective%20Dataset](https://github.com/Bin-ary-Li/JenAesthetics/tree/master/JenAesthetics subjective Dataset))

  **Authors:** Seyed Ali Amirshahi, Gregor Uwe Hayn-Leichsenring, Joachim Denzler, Christoph Redies

  **Introduction (English):** Addressing the lack of public subjective datasets for painting aesthetic research (a key barrier compared to photograph-related studies), this work conducts a subjective test on the newly released JenAesthetics dataset. The test collects not only subjective aesthetic quality scores but also data on other properties linked to aesthetic judgment (e.g., color, composition, content). As a public dataset dedicated to painting aesthetic research, JenAesthetics provides valuable labeled resources for computational aesthetics studies, laying the foundation for analyzing the factors influencing painting aesthetics and developing related assessment models.

- **Towards Artistic Image Aesthetics Assessment: A Large-Scale Dataset and a New Method** [Proc. IEEE/CVF Conf. Comput. Vis. Pattern Recognit. (CVPR), 2023, pp. 22388-22397] [[paper\]](https://arxiv.org/abs/2303.15166)[[dataset\]](https://github.com/Dreemurr-T/BAID)

  **Authors:** Ran Yi, Haoyuan Tian, Zhihao Gu, Yu-Kun Lai, Paul L. Rosin

  **Introduction (English):** To fill the gap of large-scale datasets and specialized methods for Artistic Image Aesthetics Assessment (AIAA), this study proposes the Boldbrush Artistic Image Dataset (BAID) and the Style-specific Art Assessment Network (SAAN). BAID contains 60,337 artistic images across multiple art forms, annotated with over 360,000 user votes to ensure reliable aesthetic labels. SAAN is designed to extract both style-specific and generic aesthetic features, adapting to the unique characteristics of different artistic styles. Experimental results demonstrate that SAAN outperforms existing general image aesthetics assessment methods on BAID, providing a foundational dataset and technical framework for future AIAA research.

- **Automated Flower Classification over a Large Number of Classes** [2008 Sixth Indian Conf. Comput. Vis. Graph. Image Process. (ICVGIP), Bhubaneswar, India, 2008, pp. 722-729] [[paper\]](https://ieeexplore.ieee.org/document/4756141)[[dataset\]](https://www.kaggle.com/datasets/nunenuh/pytorch-challange-flower-dataset)

  **Authors:** Maria-Elena Nilsback, Andrew Zisserman

  **Introduction (English):** To address the challenge of classifying similar classes in large datasets, this study introduces a 103-class flower dataset and explores feature combination for improved classification performance. Four distinct features are computed to capture different floral characteristics: local shape/texture, boundary shape, overall petal spatial distribution, and color. These features are integrated using a multiple kernel framework with a Support Vector Machine (SVM) classifier, where class weights are learned via the Varma and Ray method (a state-of-the-art approach for large datasets like Caltech 101/256). The dataset presents unique challenges of high inter-class similarity and low intra-class similarity. Experimental results show that combining all features significantly boosts performance—achieving 72.8% accuracy, compared to 55.1% with the best single feature—validating the effectiveness of multi-feature fusion for fine-grained flower classification.

- **ConvSRGAN: super-resolution inpainting of traditional Chinese paintings** [Heritage Sci., 2024, 12(1), 176] [[paper\]](https://www.nature.com/articles/s40494-024-01279-1)[[dataset\]](https://doi.org/10.1186/s40494-024-01279-1)

  **Authors:** Qiyao Hu, Xianlin Peng, Tengfei Li, Xiang Zhang, Jiangpeng Wang, Jinye Peng

  **Introduction (English):** Addressing the unique challenges of traditional Chinese painting super-resolution (e.g., preserving brushstroke details, abstract elements, and artistic style), this study proposes ConvSRGAN, a generative adversarial network tailored for the task. Key contributions include three core components: 1) the SRCLP dataset (900 high-resolution Chinese landscape paintings, augmented to 2175 images) providing specialized training data; 2) novel network modules (Enhanced Adaptive Residual Module (EARM), Enhanced High-Frequency Retention Module (EHRM), and Adaptive Deep Convolution Block (ADCB)) for multi-scale feature extraction and high-frequency detail preservation; 3) a joint loss function combining MS-SSIM loss with adversarial, perceptual, and L1 losses to maintain structural integrity and artistic fidelity. Experiments on SRCLP, Mural, and other datasets show ConvSRGAN outperforms SOTA methods (e.g., Real-ESRGAN) with 28.281 dB PSNR, 0.803 SSIM, and 0.2334 LPIPS, effectively restoring brushstrokes, colors, and spatial layout while retaining the original artistic style.

- **SGRGAN: sketch-guided restoration for traditional Chinese landscape paintings** [Heritage Sci., 2024, 12(1), 163] [[paper\]](https://www.nature.com/articles/s40494-024-01253-x)[[dataset\]](https://github.com/Makbaka1/MaskCLP)

  **Authors:** Qiyao Hu, Weilu Huang, Yinyin Luo, Rui Cao, Xianlin Peng, Jinye Peng, Jianping Fan

  **Introduction (English):** Addressing the challenges of restoring traditional Chinese landscape paintings (e.g., preserving brushstrokes, abstract elements, and cultural connotations), this study proposes SGRGAN, a sketch-guided generative adversarial network. Key contributions include: 1) the MaskCLP dataset (12,242 images, including ancient paintings, masks, and grayscale sketches) for specialized training; 2) sketch as structural prior to guide fine texture and stroke reconstruction; 3) novel modules (Focal block for feature fusion, BiSCCFormer block with bi-level routing attention for structural/semantic understanding); 4) a joint loss function (reconstruction, perceptual, style, intermediate, adversarial losses) ensuring fidelity. Experiments on MaskCLP and Mural datasets show SGRGAN achieves 30.59 PSNR, 0.87 SSIM, and 0.105 LPIPS, outperforming SOTA methods in restoring structure, color, and artistic style.

- **Enhanced Deep Residual Networks for Single Image Super-Resolution** [Proc. IEEE Conf. Comput. Vis. Pattern Recognit. Workshops (CVPRW), 2017, pp. 136–144] [[paper\]](https://ieeexplore.ieee.org/document/8014885)[[dataset\]](https://www.kaggle.com/datasets/daehoyang/flickr2k)

  **Authors:** Bee Lim, Sanghyun Son, Heewon Kim, Seungjun Nah, Kyoung Mu Lee

  **Introduction (English):** To advance single image super-resolution (SISR), this study proposes the Enhanced Deep Super-Resolution Network (EDSR) and Multi-Scale Deep Super-Resolution system (MDSR). EDSR optimizes traditional residual networks by removing redundant modules, expands model size to enhance performance, and stabilizes training. MDSR enables a single model to reconstruct high-resolution images with different upscaling factors. Experimental results show EDSR outperforms state-of-the-art methods on benchmark datasets and won the NTIRE2017 Super-Resolution Challenge, laying a foundation for deep learning-based SR research.

- **LAION-5B: An open large-scale dataset for training next generation image-text models** [arXiv:2210.08402 [cs.CV], 2022] [[paper\]](https://arxiv.org/abs/2210.08402)[[dataset\]](https://laion.ai/blog/laion-5b/)

  **Authors:** Christoph Schuhmann, Romain Beaumont, Richard Vencu, Cade Gordon, Ross Wightman, Mehdi Cherti, Theo Coombes, Aarush Katta, Clayton Mullis, Mitchell Wortsman, Patrick Schramowski, Srivatsa Kundurthy, Katherine Crowson, Ludwig Schmidt, Robert Kaczmarczyk, Jenia Jitsev

  **Introduction (English):** To address the lack of open large-scale multi-modal datasets for training image-text models, this study presents LAION-5B, a public dataset containing 5.85 billion CLIP-filtered image-text pairs (2.32 billion with English text). The dataset supports replication and fine-tuning of foundational models like CLIP, GLIDE, and Stable Diffusion, with additional resources including nearest neighbor indices, a web-based exploration interface, and detection scores for watermarks, NSFW, and toxic content. As a freely available resource, LAION-5B democratizes research on large-scale multi-modal models, enabling advancements in text-guided image generation, zero-shot classification, and out-of-distribution robustness.

- **End-to-End Chinese Landscape Painting Creation Using Generative Adversarial Networks** [IEEE Winter Conf. Appl. Comput. Vis. (WACV), 2021] [[paper\]](https://arxiv.org/abs/2011.05552)

  **Author:** Alice Xue

  **Introduction (English):** Addressing the lack of original art generation in GAN-based methods (which rely on conditional input), this study proposes Sketch-And-Paint GAN (SAPGAN)—the first end-to-end model for generating Chinese landscape paintings without conditional inputs. SAPGAN consists of two sub-GANs: SketchGAN (generates edge maps) and PaintGAN (translates edge maps into complete paintings). Trained on a novel dataset of traditional Chinese landscape paintings, the model is validated via a 242-person Visual Turing Test, where 55% of SAPGAN-generated works are mistaken for human-created art—outperforming baseline GANs significantly. This work establishes a foundation for machine-original art generation in traditional Chinese painting.

- **One-shot learning of object categories** [IEEE Trans. Pattern Anal. Mach. Intell., 2006, 28(4), 594–611] [[paper\]](https://ieeexplore.ieee.org/document/1597116/)[[dataset\]](https://data.caltech.edu/records/mzrjq-6wc02)

  **Authors:** Li Fei-Fei, R. Fergus, P. Perona

  **Introduction (English):** Addressing the limitation that traditional visual object category learning requires hundreds or thousands of training examples, this study proposes a Bayesian one-shot learning framework. The core insight is leveraging prior knowledge from previously learned categories to infer models for new categories with only one or a handful of training images. Object categories are represented by probabilistic models, and prior knowledge is encoded as a probability density function on model parameters. The posterior model for a new category is obtained by updating the prior with limited observations. Evaluated on a 101-category object database, the Bayesian approach outperforms maximum likelihood (ML) and maximum a posteriori (MAP) methods in low-data scenarios, demonstrating the feasibility of learning informative category models with minimal training samples.

- **FHS-adapter: Fine-Grained Hierarchical Semantic Adapter for Chinese Landscape Paintings Generation** [Herit. Sci., 2024, 12(1): 265] [[paper\]](https://www.nature.com/articles/s40494-024-01370-7)[[dataset\]](https://github.com/T2ICLP/t2iclp)

  **Authors:** Xianlin Peng, Qiyao Hu, Fangqing Fan, Penglin Xie, Yihan Zhang, Rui Cao

  **Introduction (English):** Existing text-to-image models struggle to generate authentic Chinese landscape paintings due to insufficient fine-grained cultural guidance and mismatched style adaptation. This paper proposes FHS-adapter, a fine-grained hierarchical semantic adapter, and constructs the T2ICLP dataset (10,000 image-text pairs with Meta/Description/Sentiment/Poem prompts). It uses Taiyi-CLIP for Chinese semantic understanding and injects multi-perspective prompts into the U-Net cross-attention layers in a specific sequence. Experiments show it outperforms mainstream models in brushwork, composition, and antique style, with superior FID and CLIP-T scores.

- **LAION-400M: Open Dataset of CLIP-Filtered 400 Million Image-Text Pairs** [arXiv:2111.02114 [cs.CV], 2021] [[paper\]](https://arxiv.org/abs/2111.02114)[[dataset\]](https://arxiv.org/abs/2111.02114)

  **Authors:** Christoph Schuhmann, Richard Vencu, Romain Beaumont, Robert Kaczmarczyk, Clayton Mullis, Aarush Katta, Theo Coombes, Jenia Jitsev, Aran Komatsuzaki

  **Introduction (English):** To fill the gap of publicly available large-scale datasets for training multi-modal language-vision models (e.g., CLIP, DALL-E), this community-driven study releases LAION-400M—an open dataset containing 400 million CLIP-filtered image-text pairs. The dataset also provides precomputed CLIP embeddings and k-nearest neighbor (kNN) indices to enable efficient similarity search. As a foundational resource, LAION-400M supports training and fine-tuning of models for zero-shot/few-shot learning and cross-modal transfer, democratizing research on large-scale multi-modal systems. It was accepted at the Data Centric AI NeurIPS Workshop 2021.

- **Paint4Poem: A Dataset for Artistic Visualization of Classical Chinese Poems** [arXiv:2109.11682 [cs.CV], 2021] [[paper\]](https://arxiv.org/abs/2109.11682)[[dataset\]](https://github.com/T2ICLP/t2iclp)

  **Authors:** Dan Li, Shuai Wang, Jie Zou, Chang Tian, Elisha Nieuwburg, Fengyuan Sun, Evangelos Kanoulas

  **Introduction (English):** Artistic visualization of classical Chinese poems lacks dedicated datasets for training text-to-image models. This work constructs Paint4Poem: it includes 301 high-quality manual poem-painting pairs (Feng Zikai’s works), 3,648 caption-painting pairs, and 89,204 automatic web-collected poem-painting pairs. Benchmark experiments with AttnGAN and MirrorGAN show the dataset supports style mimicry and pictorial quality but highlights room for improving semantic alignment between poems and paintings.

- **Microsoft COCO: Common Objects in Context** [arXiv:1405.0312 [cs.CV], 2015 (v3)] [[paper\]](https://arxiv.org/abs/1405.0312)[[dataset\]](https://huggingface.co/datasets/HuggingFaceM4/COCO)

  **Authors:** Tsung-Yi Lin, Michael Maire, Serge Belongie, Lubomir Bourdev, Ross Girshick, James Hays, Pietro Perona, Deva Ramanan, C. Lawrence Zitnick, Piotr Dollár

  **Introduction (English):** To advance object recognition by integrating it with broader scene understanding, this study presents the Microsoft COCO dataset. It contains 328k complex everyday scene images, covering 91 common object categories (recognizable by a 4-year-old) with 2.5 million labeled instances. Each object is annotated with per-instance segmentations for precise localization, created via novel crowd-sourcing interfaces for category detection, instance spotting, and segmentation. The dataset is comprehensively compared with PASCAL, ImageNet, and SUN datasets, and baseline performance is provided using a Deformable Parts Model for bounding box and segmentation detection. COCO has become a foundational benchmark for object detection, segmentation, and scene understanding research.

- **An Interactive and Generative Approach for Chinese Shanshui Painting Document** [ICDAR, 2019, pp. 819-824] [[paper\]](https://ieeexplore.ieee.org/document/8978182)[[dataset\]](https://github.com/PremiLabXJTLU/ShanshuiDaDA_pth)

  **Authors:** Le Zhou, Qiu-Feng Wang, Kaizhu Huang, Cheng-Hung Lo

  **Introduction (English):** Creating Chinese Shanshui paintings is challenging for non-professionals due to the need for specialized skills. This paper proposes an interactive generative approach based on cycle GAN: users input simple sketches, and the model translates them into Shanshui paintings. An interactive system (Shanshui-DaDA) is developed for real-time generation, trained on large sketch and Shanshui datasets. Experimental results confirm it satisfies general users’ needs.

- **CCLAP: Controllable Chinese Landscape Painting Generation via Latent Diffusion Model** [arXiv 2023] [[paper\]](https://arxiv.org/abs/2304.04156)[[dataset\]](https://github.com/Robin-WZQ/CCLAP)

  **Authors:** Zhongqi Wang, Jie Zhang, Zhilong Ji, Jinfeng Bai, Shiguang Shan

  **Introduction (English):** Controllable generation of Chinese landscape paintings (CLPs) is challenging due to their unique artistic characteristics (e.g., ink wash gradation, freehand brushwork, spatial composition) and the need for fine-grained control over creative elements. To address this, this paper proposes CCLAP, a controllable generation method based on latent diffusion models (LDMs). It introduces a CLP-specific latent space optimization to capture artistic style features, designs multi-modal control modules (e.g., sketch, text, color palette) to enable precise control over composition, content, and style, and integrates a style consistency constraint to preserve the inherent aesthetic of CLPs. Experimental results demonstrate that CCLAP generates high-quality, stylistically consistent CLPs with flexible controllability, providing a new tool for digital creation and cultural heritage inheritance of Chinese landscape painting.

- **DRANet: A Semantic Segmentation Network for Chinese Landscape Paintings** [Digit. Signal Process. 2024] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S1051200424000526)[[dataset\]](https://github.com/wanlinzhou/SegCLP)

  **Authors:** QiYao Hu, Wanlin Zhou, Xianlin Peng, Xiang Zhang, Penglin Xie, Yuzhe Liu, Jinye Peng, Jianping Fan

  **Introduction (English):** Semantic segmentation of Chinese landscape paintings (CLPs) is critical for digital analysis, restoration, and creation, but existing semantic segmentation networks fail to account for CLPs' unique artistic characteristics (e.g., abstract brushwork, ink wash gradation, implicit semantic boundaries). This leads to low segmentation accuracy and ambiguous semantic classification of core elements (mountains, rivers, trees, pavilions). To address this, this paper proposes DRANet, a specialized semantic segmentation network for CLPs. It designs a dual-branch feature extraction module to capture both appearance features (color, texture) and structural features (brushstroke direction, spatial layout) of CLPs. A semantic relation attention module is integrated to model contextual dependencies between CLP elements, enhancing semantic discriminability. Additionally, a boundary refinement loss is adopted to optimize semantic boundary clarity. Experimental results on CLP datasets demonstrate that DRANet outperforms mainstream semantic segmentation networks in segmentation precision and semantic consistency, providing a reliable technical tool for CLP digital processing and cultural heritage protection.

- **COCO-Stuff: Thing and stuff classes in context** [Proc. IEEE Conf. Comput. Vis. Pattern Recognit. (CVPR), 2018] [[paper\]](https://arxiv.org/abs/1612.03716)[[dataset\]](https://github.com/nightrome/cocostuff)

  **Authors:** Holger Caesar, Jasper Uijlings, Vittorio Ferrari

  **Introduction (English):** Addressing the lack of attention to "stuff" classes (amorphous background regions like grass, sky) compared to "thing" classes (well-shaped objects like car, person), this study introduces COCO-Stuff—an extension of the COCO 2017 dataset. It augments all 164K COCO images with pixel-wise annotations for 91 stuff classes, using an efficient superpixel-based annotation protocol that leverages existing thing annotations. The dataset enables analysis of scene type, contextual relations between stuff and things, and physical/geometric properties of scenes. Experiments explore annotation speed-quality trade-offs, surface coverage of classes, spatial relations, and semantic segmentation performance, revealing the unique value of integrating stuff and thing classes for comprehensive scene understanding.

- **ImageNet: A large-scale hierarchical image database** [Proc. IEEE Conf. Comput. Vis. Pattern Recognit. (CVPR), 2009, pp. 248–255] [[paper\]](https://ieeexplore.ieee.org/document/5206848)[[dataset\]](https://image-net.org/download)

  **Authors:** Jia Deng, Wei Dong, Richard Socher, Li-Jia Li, Kai Li, Li Fei-Fei

  **Introduction (English):** To address the challenge of harnessing the explosion of Internet image data for robust computer vision models, this study introduces ImageNet—a large-scale hierarchical image database built on the WordNet ontology. The goal is to populate 80,000 WordNet synsets with 500–1000 clean, high-resolution images each, resulting in tens of millions of annotated images. In its current state (as of 2009), ImageNet includes 3.2 million images across 5247 synsets from 12 subtrees, outperforming existing datasets in scale, diversity, and accuracy. Constructed via Amazon Mechanical Turk for data collection, it supports applications in object recognition, image classification, and automatic object clustering, providing an unparalleled resource for training and benchmarking large-scale computer vision algorithms.

- **Contour Detection and Hierarchical Image Segmentation** [IEEE Trans. Pattern Anal. Mach. Intell., 2011, 33(5), 898–916] [[paper\]](https://ieeexplore.ieee.org/document/5557884)[[dataset\]](https://github.com/BIDS/BSDS500或http://www.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html#bsds500)

  **Authors:** Pablo Arbeláez, Michael Maire, Charless Fowlkes, Jitendra Malik

  **Introduction (English):** Focusing on two core computer vision tasks—contour detection and hierarchical image segmentation—this study proposes state-of-the-art algorithms for both. The contour detector integrates multiple local cues into a spectral clustering-based globalization framework to enhance detection accuracy. The segmentation algorithm transforms contour detector outputs into a hierarchical region tree, reducing segmentation to the foundation of contour detection. Extensive experiments confirm that both methods outperform competing approaches. The hierarchical segmentations support interactive refinement via user annotations, and multi-resolution computation enables coupling with recognition applications, providing a versatile framework for image analysis.

- **BPA-SAM: A Prompt Enhancement Method for SAM Using Bounding Boxes in Gongbi Painting Datasets** [Journal of Graphics (China), 2025, 46(2), 322–331] [[paper\]](http://www.txxb.com.cn/CN/abstract/abstract2402.shtml)[[dataset\]](https://github.com/ZTSSSSS/Segmentation-TCRP)

  **Authors:** Zhang Tiansheng, Zhu Minfeng, Ren Yiwen, Wang Chenhan, Zhang Lidong, Zhang Wei, Chen Wei

  **Note:** Due to the security strategy restriction of the target URL (error message: "link hit security strategy"), the full content of the paper cannot be accessed temporarily. Based on the provided citation information and title, the core content is inferred as follows:

  **Introduction (English):** Aiming at the application of Segment Anything Model (SAM) in gongbi painting datasets, this study proposes BPA-SAM, a prompt enhancement method based on bounding boxes. Gongbi paintings are characterized by intricate lines, delicate textures, and complex structural details, which pose challenges for standard SAM in accurate segmentation. BPA-SAM improves the segmentation performance by optimizing prompt design with bounding box constraints, enabling precise extraction of painting elements (e.g., figures, flowers, birds) while preserving the artistic details of gongbi paintings. The method is validated on specialized gongbi painting datasets, providing technical support for digital analysis, restoration, and preservation of traditional Chinese gongbi artworks.

- **Discovering states and transformations in image collections** [Proc. IEEE Conf. Comput. Vis. Pattern Recognit. (CVPR), 2015, pp. 1383–1391] [[paper\]](https://ieeexplore.ieee.org/document/7298744/)[[dataset\]](https://opendatalab.com/OpenDataLab/MIT-States)

  **Authors:** Phillip Isola, Joseph J. Lim, Edward H. Adelson

  **Introduction (English):** Addressing the limitation that computer vision has primarily focused on simple parametric transformations (e.g., color, geometry changes) while neglecting semantic-rich physical transformations (e.g., bending, folding, aging), this study introduces a dataset of objects, scenes, and materials in diverse transformed states. The core goal is to develop a system that explains novel image collections by identifying the states and transformations they depict. A key innovation is cross-class generalization: states and transformations learned from one set of object classes are applied to interpret entirely new object classes. This work expands the scope of transformation analysis in computer vision, linking visual changes to the physical and functional properties of objects.

- **Automatic Spatially-aware Fashion Concept Discovery** [Proc. IEEE Int. Conf. Comput. Vis. (ICCV), 2017] [[paper\]](http://arxiv.org/abs/1708.01311)[[dataset\]](https://github.com/xthan/fashion-200k)

  **Authors:** Xintong Han, Zuxuan Wu, Phoenix X. Huang, Xiao Zhang, Menglong Zhu, Yuan Li, Yang Zhao, Larry S. Davis

  **Introduction (English):** To address the need for structured fashion concept discovery from weakly labeled shopping data, this study proposes an automatic spatially-aware approach. The framework first fine-tunes GoogleNet to model clothing images and their textual descriptions in a visual-semantic embedding space. For each fashion attribute (e.g., v-neck, round-neck), it generates a spatially-aware representation by fusing semantic word vectors with spatial features from the fine-tuned network’s convolutional maps. These representations are clustered to form meaningful fashion concepts (e.g., neckline, sleeve style), and the embedding space is decomposed into concept-specific subspaces. Validated on the newly collected Fashion200K dataset, the method achieves effective concept clustering and attribute-feedback product retrieval, leveraging multimodal linguistic regularities for structured fashion data browsing.

- **Fluency-Guided Cross-Lingual Image Captioning** [Proc. 25th ACM Int. Conf. Multimedia (MM '17), 2017, pp. 943–951] [[paper\]](https://dl.acm.org/doi/10.1145/3123266.3123366)[[dataset\]](https://github.com/weiyuk/fluent-cap)

  **Authors:** Weiyu Lan, Xirong Li, Jianfeng Dong

  **Introduction (English):** Addressing the limitation that image captioning research is mostly restricted to English (due to dominant English datasets) and existing cross-lingual methods rely on manually built target-language datasets, this study proposes a fluency-guided framework for cross-lingual image captioning. The model is trained fully on machine-translated sentences (no manually written target-language data) and includes two core modules: one to automatically estimate sentence fluency and another to utilize these scores for effective target-language captioning model training. Selected as an ORAL presentation at ACM Multimedia 2017, the approach is evaluated on English-Chinese bilingual datasets, improving both fluency and relevance of generated Chinese captions without relying on manual target-language annotation.

- **Bag-of-visual-words and spatial extensions for land-use classification** [Proc. 18th SIGSPATIAL Int. Conf. Adv. Geogr. Inf. Syst. (GIS '10), 2010, pp. 270–279] [[paper\]](https://dl.acm.org/doi/10.1145/1869790.1869824)[[dataset\]](https://opendatalab.com/OpenDataLab/UC_Merced_Land_Use_Dataset)

  **Authors:** Yi Yang, Shawn Newsam

  **Introduction (English):** Focusing on land-use classification using remote sensing or geographic images, this study explores the bag-of-visual-words (BoVW) model and its spatial extensions. BoVW, a classic image representation method, is widely used in object recognition but lacks spatial information consideration. To address this limitation, the authors propose spatial extensions to integrate positional context into the BoVW framework, enhancing the discriminative power for land-use categories (e.g., urban, agricultural, forest areas). Evaluated on geographic image datasets, the method demonstrates effective land-use classification performance, validating the value of combining local visual features with spatial constraints for geographic information system (GIS) tasks.

- **Three-dimensional reconstruction image generation of traditional Chinese painting elements** [Eng. Appl. Artif. Intell. 2025] [[paper\]](https://www.sciencedirect.com/science/article/abs/pii/S0952197625014198)[[dataset\]](https://github.com/LPDLG/3DTCP-Dataset)

  **Authors:** Qiyao Hu, Jingyu Wang, Xianlin Peng, Tengfei Li, Rui Cao

  **Introduction (English):** To address the lack of 3D datasets for traditional Chinese paintings and the challenge of single-view 3D reconstruction, this paper proposes the TCPE-3D framework, integrating the OTX-MVG multi-view synthesis module, NeRF synthesis module, and mesh generation module. It constructs the 3DTCP dataset, solves the Janus problem, and achieves high-quality 3D reconstruction of Chinese painting elements with better visualization results than state-of-the-art methods.

- **ConCLVD: Controllable Chinese Landscape Video Generation via Diffusion Model** [arXiv:2404.12903 [cs.MM], 2024] [[paper\]](https://arxiv.org/html/2404.12903v1)[[dataset\]](https://github.com/ConCLVD/ConCLVD?tab=readme-ov-file)

  **Authors:** Dingming Liu, Shaowei Li, Ruoyan Zhou, Lili Liang, Yongguan Hong, Fei Chao, Rongrong Ji

  **Introduction (English):** Static Chinese landscape paintings lack dynamic expression, and existing text-to-video models face challenges like scarce specialized datasets and poor style consistency. This paper proposes ConCLVD, a controllable diffusion model for Chinese landscape video generation, along with the CLV-HD dataset (1,300 text-video pairs). It integrates a motion module with dual attention mechanisms, latent space noise contrastive learning, and optical flow-based frame interpolation. The model runs on a single RTX 3090, achieving high temporal consistency and style fidelity, outperforming baselines in user studies.

- **HMDB: A large video database for human motion recognition** [Proc. Int. Conf. Comput. Vis. (ICCV), 2011, pp. 2556–2563] [[paper\]](https://ieeexplore.ieee.org/document/6126543)[[dataset\]](https://www.kaggle.com/datasets/easonlll/hmdb51)

  **Authors:** H. Kuehne, H. Jhuang, E. Garrote, T. Poggio, T. Serre

  **Introduction (English):** Addressing the gap between large-scale static image datasets and limited human action video databases, this study presents HMDB—the largest action video database at the time—for human motion recognition. It contains 51 action categories with around 7,000 manually annotated clips, sourced from diverse materials (digitized movies, YouTube, etc.), far exceeding the scale of existing action datasets (which typically have ~10 categories under controlled conditions). The database is used to evaluate two representative action recognition systems, exploring their robustness under real-world variations such as camera motion, viewpoint changes, video quality differences, and occlusion. HMDB fills the need for a comprehensive benchmark, enabling advancements in video-based human motion recognition research.

- **Recognizing Realistic Actions from Videos "in the Wild"** [Proc. IEEE Conf. Comput. Vis. Pattern Recognit. (CVPR), 2009, pp. 1996–2003] [[paper\]](https://ieeexplore.ieee.org/document/5206744)[[dataset\]](https://www.kaggle.com/datasets/pypiahmad/ucf-youtube-action-data-set)

  **Authors:** Jingen Liu, Jiebo Luo, Mubarak Shah

  **Introduction (English):** Addressing the under-explored problem of recognizing actions from unconstrained "in-the-wild" videos (abundant in personal collections and online platforms), this study proposes a systematic framework to handle challenges like camera motion, background clutter, appearance changes, and scale variations. The framework extracts both motion and static features from videos, then prunes noisy raw features: motion statistics are used to stabilize motion features and clean static features, while PageRank mines the most informative static features. A divisive information-theoretic algorithm groups semantically related features into compact visual vocabularies, and AdaBoost integrates these heterogeneous yet complementary features for recognition. Tested on the KTH dataset and a self-collected 11-category dataset (from YouTube and personal videos), the method achieves impressive results in both action recognition and localization.

- **Consumer video understanding: a benchmark database and an evaluation of human and machine performance** [Proc. 1st ACM Int. Conf. Multimedia Retrieval (ICMR '11), 2011, pp. 1–8, Article No. 29] [[paper\]](https://dl.acm.org/doi/10.1145/1991996.1992025)[[dataset\]](https://www.ee.columbia.edu/ln/dvmm/CCV/)

  **Authors:** Yu-Gang Jiang, Guangnan Ye, Shih-Fu Chang, Daniel Ellis, Alexander C. Loui

  **Introduction (English):** To address the lack of large-scale, diverse datasets for unconstrained consumer video analysis, this study introduces the CCV benchmark database—containing 9,317 web videos across 20 semantic categories (e.g., events like "baseball", scenes like "beach", objects like "cat"). The dataset prioritizes consumer relevance and original, unedited content (with minimal textual annotation), supporting the development of automatic content analysis techniques. Using Amazon MTurk for manual annotation, the authors evaluate human annotator performance and compare human vs. machine understanding of consumer videos. The machine learning approach employs a state-of-the-art multi-modal classifier (fusing audio and video features) that excelled in TRECVID multimedia event detection. Results show multi-modal fusion outperforms single-modality methods; humans outperform machines on nonrigid object categories (e.g., "cat"), while machines approach human performance on categories with distinctive scenes or audio patterns.

- **Research on Emotion Analysis of Chinese Literati Painting Images Based on Deep Learning** [Front. Psychol., 2021, 12: 723325] [[paper\]](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2021.723325/full)

  **Authors:** Jie Zhang, Yingjing Duan, Xiaoqing Gu

  **Introduction (English):** This study proposes a pure-image-based cross-cutting approach for Chinese literati painting emotion analysis using deep learning. It constructs a dedicated emotion dataset, tests five classic models to select the optimal one (ResNet50), and improves it to achieve 54.17% training accuracy. By visualizing salient feature areas in machine vision, it summarizes the connection between painting content and expressed emotions, validating the integration of deep learning with Chinese cultural research.

- **Research on the Integration of Digital Media and Oil Painting Teaching in Colleges and Universities in the Era of Artificial Intelligence** [Appl. Math. Nonlinear Sci., 2023, 9, -] [[paper\]](https://www.researchgate.net/publication/377552805_Research_on_the_Integration_of_Digital_Media_and_Oil_Painting_Teaching_in_Colleges_and_Universities_in_the_Era_of_Artificial_Intelligence)[[dataset\]](https://www.researchgate.net/figure/Gallerix-data-set-Style-subsets-each-sample-size_tbl2_377552805)

  **Author:** Zhao Lingyu

  **Introduction (English):** Focusing on the integration of digital media and oil painting teaching in colleges under the artificial intelligence era, this study constructs a resource library of oil painting images created by college students. The research converts original RGB images to HSV mode and classifies college oil painting images by style based on color entropy. It draws on the category-balanced intersectionality loss function commonly used in edge extraction networks and designs an objective evaluation index based on the AdaIN network model to compare the stylistic categorization ability of oil painting image translation networks. A generalization experiment is conducted on college oil painting teaching images using the Gallerix dataset. Results show that in the 2566-dimensional vector data distribution extracted from the oil painting resource library of art majors in H University, the correct clustering centers are found when dc=0.05 and dc=0.1, significantly improving college students' oil painting creation efficiency. This method promotes the application and development of artificial intelligence technology in art creation and evaluation.

- **Building Emotional Machines: Recognizing Image Emotions through Deep Neural Networks** [arXiv:1705.07543 [cs.CV], 2017 (v2)] [[paper\]](https://arxiv.org/abs/1705.07543)[[dataset\]](https://figshare.com/articles/dataset/CGnA10766_Dataset/5383105)

  **Authors:** Hye-Rin Kim, Yeong-Seok Kim, Seon Joo Kim, In-Kwon Lee

  **Introduction (English):** To effectively recognize emotions conveyed by images, this study proposes a feedforward deep neural network that leverages high-level semantic features—objects and backgrounds. The core insight is that image semantics (especially objects) have a strong correlation with emotional expression, while backgrounds further refine emotion prediction even for the same object. The network combines multi-level features to output continuous emotion values in a 2-dimensional Valence-Arousal space, which is more expressive than discrete emotion categories. Experiments validate that the model effectively predicts image emotions by integrating object and background semantic information, advancing the development of "emotional machines" in computer vision.

- **Deep Learning with Darwin: Evolutionary Synthesis of Deep Neural Networks** [Neural Process. Lett., 2018, 48, -] [[paper\]](https://arxiv.org/abs/1606.04393)[[dataset\]](https://www.researchgate.net/figure/MSRA-B-image-dataset-this-dataset-contains-5000-natural-images-divided-into-2500-500_fig2_321170017)

  **Authors:** Mohammad Javad Shafiee, Akshaya Mishra, Alexander Wong

  **Introduction (English):** Inspired by biological evolution, this study explores whether deep neural networks can "naturally evolve" into highly efficient models over successive generations. The core framework encodes architectural traits of ancestor networks into synaptic probability models (analogous to "DNA"), then synthesizes descendant networks with diverse architectures via random variation—mimicking heredity, natural selection, and mutation—by combining these synaptic models with computational environmental factor models. Offspring networks are trained to full functionality, achieving more efficient architectures than ancestors while maintaining powerful modeling capabilities. Experimental results on visual saliency tasks show that evolved networks reach state-of-the-art performance, with a ~48-fold reduction in synapses by the fourth generation compared to the original ancestor network, verifying the effectiveness of evolutionary synthesis for efficient deep learning.

- **International Affective Picture System (IAPS): Technical Manual and Affective Ratings** [1995] [[paper\]](https://www.semanticscholar.org/paper/International-Affective-Picture-System-(IAPS)-%3A-and-Lang/09bb229a610acdd3150b8e0176194e7b7cf471b7)[[dataset/](https://en.wikipedia.org/wiki/International_Affective_Picture_System)]

  **Author:** Peter J. Lang

  **Note:** The target URL is unavailable (error message: "link dead"), so the full content cannot be accessed. Based on the title, field conventions, and public knowledge of the IAPS dataset, the core content is inferred as follows:

  **Introduction (English):** As a foundational resource for affective computing and psychological research, the International Affective Picture System (IAPS) is a standardized set of emotional picture stimuli with normative affective ratings. The manual details the development, composition, and usage of the dataset, which includes thousands of pictures covering diverse themes (e.g., nature, people, objects, scenes) rated on two core emotional dimensions: Valence (pleasure-displeasure) and Arousal (excitement-calm). These normative ratings provide a quantitative basis for studying emotional responses to visual stimuli, supporting research in psychology, neuroscience, computer vision (e.g., image emotion recognition), and human-computer interaction. The IAPS has become a widely adopted benchmark for validating emotion-related models and experiments globally.

- **Large-scale visual sentiment ontology and detectors using adjective noun pairs** [Proc. 21st ACM Int. Conf. Multimedia (MM '13), 2013, pp. 223–232] [[paper\]](https://dl.acm.org/doi/10.1145/2502081.2502282)

  **Authors:** Damian Borth, Rongrong Ji, Tao Chen, Thomas Breuel, Shih-Fu Chang

  **Introduction (English):** Addressing the challenge of visual sentiment analysis, this study proposes a novel approach that infers sentiment from sentiment-related visual concepts rather than direct low-level features. The key contributions are two-fold: first, a large-scale Visual Sentiment Ontology (VSO) with over 3,000 Adjective Noun Pairs (ANPs) is automatically constructed via psychological theories and web mining; second, SentiBank—a library of 1,200 ANP visual concept detectors—is developed to identify ANP presence in images. These resources enable automatic sentiment analysis for diverse applications. Experiments on image tweets show that SentiBank-based predictors outperform text-based methods in sentiment detection accuracy. The work also provides a public resource package including the VSO, detector library, and training/testing benchmarks, advancing visual sentiment analysis research.

- **Novel Dataset for Fine-Grained Image Categorization: Stanford Dogs** [2012] [[paper\]](https://www.semanticscholar.org/paper/Novel-Dataset-for-Fine-Grained-Image-Categorization-Khosla-Jayadevaprakash/b5e3beb791cc17cdaf131d5cca6ceb796226d832)[[dataset\]](https://www.kaggle.com/datasets/jessicali9530/stanford-dogs-dataset)

  **Authors:** Aditya Khosla, Nityananda Jayadevaprakash, Bangpeng Yao, Li Fei-Fei

  **Introduction (English):** To advance fine-grained image categorization research—a challenging task requiring discrimination between visually similar subcategories—this study introduces the Stanford Dogs dataset. It contains over 22,000 annotated images covering 120 dog species, designed to address the complexity of fine-grained recognition (e.g., subtle inter-class variations, self-occlusions, and pose differences). As a large-scale and challenging benchmark, the dataset has become widely adopted in the field, supporting the development and evaluation of fine-grained categorization methods. With 1,522 citations to date, it has significantly influenced research on visual feature extraction, part-based modeling, and weakly supervised learning for subordinate-level object recognition.

- **3D Object Representations for Fine-Grained Categorization** [Proc. IEEE Int. Conf. Comput. Vis. Workshops (ICCVW), 2013, pp. 554–561] [[paper\]](https://ieeexplore.ieee.org/document/6755945)[[dataset\]](https://www.kaggle.com/datasets/eduardo4jesus/stanford-cars-dataset)

  **Authors:** Jonathan Krause, Michael Stark, Jia Deng, Li Fei-Fei

  **Introduction (English):** Addressing the limitation that fine-grained categorization mostly relies on flat 2D representations (which model objects as unconnected views and lack viewpoint generalization), this study lifts state-of-the-art 2D object representations to 3D—covering both local feature appearance and location. 3D representations have shown advantages in multi-view object detection and scene understanding by linking object parts across views, but they were underutilized in fine-grained recognition. Extensive experiments on existing and new datasets demonstrate that the proposed 3D representations outperform their 2D counterparts in fine-grained categorization. Additionally, the method proves effective for 3D geometry estimation from images via ultra-wide baseline matching and 3D reconstruction, expanding the utility of 3D modeling in fine-grained vision tasks.

- **WikiArt Dataset** [Kaggle Dataset] [[link\]](https://www.kaggle.com/datasets/steubk/wikiart)

  **Creator:** steubk

  **Introduction (English):** As a large-scale benchmark dataset for artistic image analysis, the WikiArt Dataset is derived from the WikiArt online art gallery, covering thousands of artworks from renowned artists worldwide. It includes diverse art styles (e.g., Impressionism, Cubism, Surrealism, Baroque), genres (portraits, landscapes, still lifes), and media (oil paintings, watercolors, sketches). Each artwork is annotated with metadata such as artist name, creation year, style category, and genre, providing a rich resource for research tasks like art style classification, style transfer, artistic sentiment analysis, and fine-grained artistic image recognition. The dataset has become a foundational resource in computer vision and digital art research, supporting the development and evaluation of models for artistic content understanding.


## Cite This Survey

If you find this repository useful for your research, please consider citing our paper:
