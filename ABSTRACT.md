The **CCP: Clothing Co-Parsing** dataset contains 2,098 high-resolution fashion photos with diverse human/clothing variations, including superpixel-level annotations with 57 tags for over 1,000 images, along with image-level tags for the rest of the dataset, all meticulously produced by a professional team.

Authors introduce a system aimed at parsing clothing images to provide accurate pixel-wise annotations of clothing items, addressing challenges such as diverse clothing styles, human pose variations, and a large number of fine-grained clothing categories. The system comprises two sequential phases: image co-segmentation for extracting distinct clothing regions and region co-labeling for recognizing various garment items.

Clothing recognition and retrieval have huge potential in internet-based e-commerce, as the revenue of online clothing sales keeps increasing every year. The authors focused on building an engineered and applicable system to jointly parse a batch of clothing images and produce accurate pixel-wise annotation of clothing items. They consider the following challenges to build such a system:

- The appearances of clothes and garment items are often diverse with different styles and textures, compared with other common objects. It is usually hard to segment and recognize clothes via only bottom-up image features.
- The variations of human poses and self-occlusions are non-trivial issues for clothing recognition, although the clothing images can be in clear resolution and nearly frontal view.
- The number of fine-grained clothes categories is very large, e.g., more than 50 categories in the [Fashionista dataset](https://www.cs.unc.edu/~hadi/publications/papers/yamaguchiICVPR12parsing.pdf); the categories are relatively fewer in existing co-segmentation systems.

To address the above issues, authors develop a system consisting of two sequential phases of inference over a set of clothing images, i.e. image co-segmentation for extracting distinguishable clothes regions, and region co-labeling for recognizing various garment items.

![Fig](https://i.ibb.co/LZ96bbk/Screenshot-2023-10-06-113318.png)

<span style="font-size: smaller; font-style: italic;">Illustration of the proposed clothing co-parsing framework, which consists of two sequential phases of optimization: (a) clothing co-segmentation for extracting coherent clothes regions, and (b) region co-labeling for recognizing various clothes garments. Specifically, clothing co-segmentation iterates with three steps: (a1) grouping superpixels into regions, (a2) selecting confident foreground regions to train E-SVM classifiers, and (a3) propagating segmentations by applying E-SVM templates over all images. Given the segmented regions, clothing co-labeling is achieved based on a multi-image graphical model, as illustrated in (b).</span>
