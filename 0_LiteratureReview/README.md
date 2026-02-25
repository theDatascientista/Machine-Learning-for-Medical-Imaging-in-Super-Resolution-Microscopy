# Literature Review

Approaches or solutions that have been tried before on similar projects.

**Summary of Each Work**:

- **Source 1**: [Lal et al.: A Frequency Domain SIM Reconstruction Algorithm Using Reduced Number of Images, IEEE Transactions
on Image Processing, vol. 27, no. 9, 2018.]

  - **[Link](https://ieeexplore.ieee.org/document/8369094)**
  - **Objective**: The paper presents a Neural Network for image super-resolution that operates entirely in the frequency domain. The goal is to reduce computational cost while maintaining reconstruction quality comparable to state-of-the-art spatial-domain deep networks.
  - **Methods**: The authors developed a frequency-domain Neural Network based on the convolution theorem, where spatial convolutions are replaced by point-wise multiplications in the frequency domain and nonlinear activation is modeled as frequency-domain convolution. The network predicts high-frequency residual components using residual learning and is implemented with the Hartley transform to avoid complex numbers, enabling efficient training via backpropagation.
  - **Outcomes**: The frequency-domain Neural Network achieves good performance, close to leading deep learning approaches, but with improved computational efficiency.
  - **Relation to the Project**: We used this method as inspiration to develop our own frequency-domain Neural Network. Since the code of this paper was not available, we could not perform a comparison between this model and ours.

- **Source 2**: [Burns, Z.; Liu, Z: Untrained, physics-informed neural networks for structured illumination microscopy, Opt. Express
31, 2023.]

  - **[Link](https://opg.optica.org/oe/fulltext.cfm?uri=oe-31-5-8714)**
  - **Objective**: The authors intended to develop a training-free reconstruction method for structured illumination microscopy (SIM) that overcomes the limitations of traditional linear algorithms and supervised learning. The method therefor does not require ground-truth data, which often is hard to obtain in many scientific fields. Especially traditional Deep Learning methods need large datasets including ground truth data.
  - **Methods**: The model takes a set of diffraction-limited sub-images that were captured under different structured illumination patterns. A Neural Network predicts a high resolution image from these. The predicted high-resolution image is passed through the known SIM forward model (illumination patterns + microscope blur) to generate simulated sub-images. The simulated sub-images are compared to the experimentally measured ones using a similarity loss. This loss is used for the network training / back-propagation.
  - **Outcomes**: The proposed PINN achieves resolution improvements matching theoretical expectations across multiple cell structures. The method eliminates the need for training datasets or extensive parameter tuning.
  - **Relation to the Project**: We used this method as starting point for our own research and the search for alternative methods.

- **Source 3**: [Manton JD.: Answering some questions about structured illumination microscopy, Phil. Trans. R. Soc. A 380: 20210109, 2022.]

  - **[Link](https://royalsocietypublishing.org/doi/pdf/10.1098/rsta.2021.0109)**
  - **Objective**: The article provides a general introduction to the method of SIM including mathematical backgrounds, usages, problems, limitations, but also the application of Machine Learning.
  - **Methods**: Machine Learning has been used to convert SIM images to higher resolution.
  - **Outcomes**: No details.
  - **Relation to the Project**: The article provides a basic understanding of SIM technology and how ML can be used in it.
