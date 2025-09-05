# Multimodal Deepfake Detection Using Frame-Level Visual Features and Mel Spectrograms

#Abstract

Deepfake content has become increasingly convincing and accessible with the rapid progress of generative models. As manipulation techniques evolve, detectors that rely on a single modality often fail to maintain robustness. In this paper, we introduce a dual-stream deepfake detection framework that integrates both visual and auditory information. Frame-level representations are extracted from video sequences, while complementary audio features are derived from Mel-spectrograms; each modality is processed through dedicated convolutional neural networks (DCNNs). The resulting feature embeddings are fused to enable reliable classification of authentic and manipulated media. Experimental results demonstrate that our approach achieves 96% accuracy on FakeAVCeleb and 97% accuracy on Celeb-DF, significantly outperforming single-modality baselines. These findings underscore the effectiveness of multimodal fusion for improving detection reliability and cross-dataset generalization, establishing a strong foundation for future research on resilient deepfake detection systems.


Pipeline of the proposed model : 

<img width="1536" height="1024" alt="pipeline" src="https://github.com/user-attachments/assets/fbf80b12-c7a0-4b8f-ace0-e32711b4d588" />

Model Architecture : 

<img width="7917" height="18458" alt="model_architecture" src="https://github.com/user-attachments/assets/365b17a4-adf4-443c-ab9e-ab9543c6ec6d" />
