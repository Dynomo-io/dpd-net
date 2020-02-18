# DPDNet
This paper proposes a deep learning-based method to detect multiple people from a single overhead depth image with high precision. Our neural network, called DPDnet, is composed by two fully-convolutional encoder-decoder blocks built with residual layers. The main block takes a depth image as input and generates a pixel-wise confidence map, where each detected person in the image is represented by a Gaussian-like distribution, The refinement block combines the depth image and the output from the main block, to refine the confidence map. Both blocks are simultaneously trained end-to-end using depth images and ground truth head position labels. The paper provides a rigorous experimental comparison with some of the best methods of the state-of-the-art, being exhaustively evaluated in different publicly available datasets. DPDnet proves to outperform all the evaluated methods with statistically significant differences, and with accuracies that exceed 99%. The system was trained on one of the datasets (generated by the authors and available to the scientific community) and evaluated in the others without retraining, proving also to achieve high accuracy with varying datasets and experimental conditions. Additionally, we made a comparison of our proposal with other CNN-based alternatives that have been very recently proposed in the literature, obtaining again very high performance. Finally, the computational complexity of our proposal is shown to be independent of the number of users in the scene and runs in real time using conventional GPUs.
![Alt text](diagrama_tof.png?raw=true "System Blocks Diagram")
