
* TOC 
{:toc}

## A Summary of the Project

Object detection is the problem of labeling and locating the objects in a given image. Modern object detection methods solve the problem in two stages, which we can call as "search" and "recognition". In the search phase, candidates for objects are determined independently of the class, and in the recognition phase, their classes are estimated.

Our project and our contributions focused on two key challenges:

(1) Context in object detection: Using global and local context in an end-to-end deep learning system to increase the performance of the recognition phase in object detection in images and videos; and a deep neural network-based "generalized Hough transform" method was developed as an alternative to the "object proposal" methods corresponding to the search phase. It has been shown that when our method is applied to object detection problems in images and videos, it successfully can exploit contextual information and produces better results than baseline methods.

(2) Object detection in videos with the referring expressions: A new dataset was created for object search with referring expressions (e.g. "blue car on the right") in videos; and we have developed new methods for searching objects with referring expressions in this dataset. It has been shown that the methods we have developed are very successful in detecting objects corresponding to complex referring expressions and in generating the most appropriate referring expression for two selected objects in a video.

## Project Members

* PI: [Emre Akbaş](https://user.ceng.metu.edu.tr/~emre/), Dept. of Computer Engineering, METU.
* Co-PI: [Sinan Kalkan](http://kovan.ceng.metu.edu.tr/~sinan/), Dept. of Computer Engineering, METU
* Students: Hazan Anayurt, [İlker Bozcan](https://bozcani.github.io/), Barış Can Çam, Bedrettin Çetinkaya, Gökçen Gökçeoğlu,  Raheem Karim Hashmani, [Nermin Samet](https://nerminsamet.github.io/), [Kemal Öksüz](https://kemaloksuz.github.io/), [Sezai Artun Özyeğin](https://user.ceng.metu.edu.tr/~artun/), Abdussamet Tarık Temür.

## Project's Academic Contributions

### Publications

* K. Oksuz, B. C. Cam, S. Kalkan*, E. Akbas*, "One Metric to Measure them All: Localisation Recall Precision (LRP) for Evaluating Visual Detection Tasks", IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), under review, 2021. [Arxiv](https://arxiv.org/abs/2011.10772), [Code](https://github.com/kemaloksuz/LRP-Error) *Equal senior contribution.
* K. Oksuz, B. C. Cam, S. Kalkan*, E. Akbas*, "Imbalance Problems in Object Detection: A Review", IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), in press, 2021. [Arxiv](https://arxiv.org/abs/1909.00169), [Publisher's page](https://ieeexplore.ieee.org/document/9042296), [Repository](https://github.com/kemaloksuz/ObjectDetectionImbalance) *Equal senior contribution.
* N. Samet, S. Hicsonmez, E. Akbas, "HoughNet: Integrating near and long-range evidence for bottom-up object detection", European Conference on Computer Vision (ECCV), 2020. [Arxiv](https://arxiv.org/abs/2007.02355), [Publisher's page](https://link.springer.com/chapter/10.1007/978-3-030-58595-2_25), [Code](https://github.com/nerminsamet/houghnet).
* N. Samet, S. Hicsonmez, E. Akbas, "Reducing Label Noise in Anchor-Free Object Detection", British Machine Vision Conference (BMVC), 2020. [Arxiv](https://arxiv.org/abs/2008.01167), [Code](https://github.com/nerminsamet/ppdet)
* K. Oksuz, B. C. Cam, E. Akbas*, S. Kalkan*, "A Ranking-based, Balanced Loss Function Unifying Classification and Localisation in Object Detection", Thirty-fourth Conference on Neural Information Processing Systems (NeurIPS), spotlight paper, 2020. [Arxiv](https://arxiv.org/abs/2009.13592), [Conference page](https://proceedings.neurips.cc/paper/2020/hash/b2eeb7362ef83deff5c7813a67e14f0a-Abstract.html), [Code](https://github.com/kemaloksuz/aLRPLoss). *Equal senior contribution.
* H. Anayurt, S. A. Ozyegin, U. Cetin, U. Aktas, S. Kalkan, "Searching for Ambiguous Objects in Videos using Relational Referring Expressions", 30th British Machine Vision Conference (BMVC), 2019. [Arxiv](https://arxiv.org/abs/1908.01189), [Code](https://github.com/hazananayurt/viref).
* K. Oksuz, B. C. Cam, E. Akbas*, S. Kalkan*, "Generating Positive Bounding Boxes for Balanced Training of Object Detectors", IEEE Winter Conference on Applications of Computer Vision (WACV), 2020. [Arxiv](https://arxiv.org/abs/1909.09777), [Publisher's page](https://www.computer.org/csdl/proceedings-article/wacv/2020/09093503/1jPbqXS57W0), [Code](https://github.com/kemaloksuz/BoundingBoxGenerator). *Equal senior contribution.
* K. Oksuz, B. C. Cam, E. Akbas, S. Kalkan, "Localization Recall Precision (LRP): A New Performance Metric for Object Detection", European Conference on Computer Vision (ECCV), pp. 521-537, Springer, 2018. [Arxiv](https://arxiv.org/abs/1807.01696), [Publisher's page](https://link.springer.com/chapter/10.1007/978-3-030-01234-2_31), [Code](https://github.com/cancam/LRP).

### Theses

Completed:
* Bedrettin Cetinkaya, "Does estimated depth help object detection?", Dept. of Computer Engineering, METU, 2020. [Thesis copy](https://open.metu.edu.tr/handle/11511/44129)
* Baris Can Cam, “Training object detectors by directly optimizing LRP metric", Dept. of Computer Engineering, METU, 2020. [Thesis copy](https://tez.yok.gov.tr/UlusalTezMerkezi/tezDetay.jsp?id=FHUZtNW2yRDWU3VWBud_mg&no=V55zHSMS2t6FuhgksIMJFg)

Ongoing:
* Hazan Anayurt, Dept. of Computer Engineering, METU, 2021.
* Sezai Artun Özyeğin, Dept. of Computer Engineering, METU, 2021.
* Kemal Öksüz, Dept. of Computer Engineering, METU, 2021.
* Nermin Samet, Dept. of Computer Engineering, METU, 2021. 

### Workshop

* [ECCV2020 Workshop on Imbalance Problems in Computer Vision (IPCV)](https://sites.google.com/view/ipcv2020/home).

### Invited Talks

* TBC.

## Models and Methods Developed within the Project

### [HoughNet](https://github.com/nerminsamet/houghnet) 

A method for object detection in images using context and generalized hough transform.

The corresponding paper: Samet, N., Hicsonmez, S., & Akbas, E. (2020). HoughNet: Integrating near and long-range evidence for bottom-up object detection. In European Conference on Computer Vision (pp. 406-423).  [link](https://link.springer.com/chapter/10.1007/978-3-030-58595-2_25)

### [PPDet](https://github.com/nerminsamet/ppdet)

A method for reducing label noise in anchor-free object detectors. 

The corresponding paper: Samet, N., Hicsonmez, S., & Akbas, E. (2020). Reducing Label Noise in Anchor-Free Object Detection. British Machine Vision Conference (BMVC). [link](https://www.bmvc2020-conference.com/conference/papers/paper_0737.html)

### [VIREF](https://github.com/hazananayurt/viref)

A method and a dataset for object search in videos using referring expressions. 

The corresponding paper: Anayurt, H., Ozyegin, S. A., Cetin, U., Aktas, U., & Kalkan, S. (2019). Searching for ambiguous objects in videos using relational referring expressions. British Machine Vision Conference (BMVC). [link](https://bmvc2019.org/wp-content/uploads/papers/0697-paper.pdf)

### [aLRP Loss](https://github.com/kemaloksuz/aLRPLoss) 

A novel ranking based loss function for object detection. 

The corresponding papers:
* K. Oksuz, B. C. Cam, E. Akbas*, S. Kalkan*, "A Ranking-based, Balanced Loss Function Unifying Classification and Localisation in Object Detection", Thirty-fourth Conference on Neural Information Processing Systems (NeurIPS), spotlight paper, 2020. [Arxiv](https://arxiv.org/abs/2009.13592), [Conference page](https://proceedings.neurips.cc/paper/2020/hash/b2eeb7362ef83deff5c7813a67e14f0a-Abstract.html), [Code](https://github.com/kemaloksuz/aLRPLoss). *Equal senior contribution.  

* K. Oksuz, B. C. Cam, S. Kalkan*, E. Akbas*, "One Metric to Measure them All: Localisation Recall Precision (LRP) for Evaluating Visual Detection Tasks", IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), under review, 2021. [Arxiv](https://arxiv.org/abs/2011.10772), [Code](https://github.com/kemaloksuz/LRP-Error) *Equal senior contribution.

### [LRP Error](https://github.com/kemaloksuz/LRP-Error) 

A novel evaluation metric for visual detection problems. 

The corresponding papers:
* K. Oksuz, B. C. Cam, S. Kalkan*, E. Akbas*, "One Metric to Measure them All: Localisation Recall Precision (LRP) for Evaluating Visual Detection Tasks", IEEE Transactions on Pattern Analysis and Machine Intelligence (PAMI), under review, 2021. [Arxiv](https://arxiv.org/abs/2011.10772), [Code](https://github.com/kemaloksuz/LRP-Error) *Equal senior contribution.

* K. Oksuz, B. C. Cam, E. Akbas, S. Kalkan, "Localization Recall Precision (LRP): A New Performance Metric for Object Detection", European Conference on Computer Vision (ECCV), pp. 521-537, Springer, 2018. [Arxiv](https://arxiv.org/abs/1807.01696), [Publisher's page](https://link.springer.com/chapter/10.1007/978-3-030-01234-2_31), [Code](https://github.com/cancam/LRP).

## Contact

[Emre Akbas](https://user.ceng.metu.edu.tr/~emre/), Dept. of Computer Engineering, METU

Last updated on March 29, 2021. 
