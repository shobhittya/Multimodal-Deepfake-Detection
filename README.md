# Multimodal Deepfake Detection Using Frame-Level Visual Features and Mel Spectrograms

Abstract

Deepfake content has become increasingly convincing and accessible with the rapid progress of generative models. As manipulation techniques evolve, detectors that rely on a single modality often fail to maintain robustness. In this paper, we introduce a dual-stream deepfake detection framework that integrates both visual and auditory information. Frame-level representations are extracted from video sequences, while complementary audio features are derived from Mel-spectrograms; each modality is processed through dedicated convolutional neural networks (DCNNs). The resulting feature embeddings are fused to enable reliable classification of authentic and manipulated media. Experimental results demonstrate that our approach achieves 96% accuracy on FakeAVCeleb and 97% accuracy on Celeb-DF, significantly outperforming single-modality baselines. These findings underscore the effectiveness of multimodal fusion for improving detection reliability and cross-dataset generalization, establishing a strong foundation for future research on resilient deepfake detection systems.

 # Requirements
 
1. Hardware
GPU: NVIDIA RTX 2080 Ti or higher (≥11 GB VRAM recommended; experiments in this work were conducted on an RTX 3090 with 24 GB).
CPU: Intel i7/i9 or AMD Ryzen 7/9 (≥8 cores).
Memory (RAM): ≥16 GB (32 GB recommended for faster preprocessing).
Storage: ≥200 GB free space (to store datasets, extracted frames, and spectrograms).

2. Software
Operating System: Ubuntu 20.04 LTS (Linux recommended; Windows 10/11 supported).
Programming Language: Python 3.8+
Deep Learning Framework: PyTorch 2.0+
Supporting Libraries:
NumPy, Pandas (data manipulation)
OpenCV (video frame extraction)
Librosa (audio preprocessing and Mel-spectrogram generation)
Scikit-learn (evaluation metrics)
Matplotlib/Seaborn (visualization)

# Datasets

1) FakeAV Dataset : [https://www.kaggle.com/xhlulu/140k-real-and-fake-faces](https://github.com/DASH-Lab/FakeAVCeleb)
2) CelebDF Dataset : [https://github.com/namtpham/casia1groundtruth](https://github.com/yuezunli/celeb-deepfakeforensics/blob/master/Celeb-DF-v)

Pipeline of the proposed model : 

<img width="1536" height="1024" alt="pipeline" src="https://github.com/user-attachments/assets/fbf80b12-c7a0-4b8f-ace0-e32711b4d588" />


# Authors
1. Shobhit Tyagi∗, 2. Naveen Chauhan∗, 3. Divakar Yadav†, 4. Prashant Upadhyay‡, 5. Piyush Rawat §

∗Department of Computer Science and Engineering and Information Technology, Jaypee Institute of Information Technology, Noida, U.P., India 
Email: {shobhit.tyagi, naveen.chauhan}@jiit.ac.in}
†School of Computer and Information Sciences, IGNOU, New Delhi, India Email: divakaryadav@ignou.ac.in
‡Department of Computer Science and Engineering, School of Engineering and Technology, Sharda University, Greater Noida, India Email: prashanttheace@gmail.com
§Department of Computer Science and Engineering, Delhi Technological University, Delhi, India Email: psh.rawat@gmail.com

