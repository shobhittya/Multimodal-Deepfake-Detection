## Multimodal Deepfake Detection Using Frame-Level Visual Features and Mel Spectrograms

**Abstract**
The rapid advancement of generative artificial intelligence has enabled the creation of highly realistic deepfake content, raising serious concerns regarding digital media authenticity, information integrity, and public trust. Existing deepfake detection approaches predominantly rely on unimodal analysis, making them vulnerable to sophisticated manipulations that preserve either visual or auditory realism while introducing subtle cross-modal inconsistencies. To address this limitation, we propose a lightweight dual-stream multimodal framework that jointly leverages visual and auditory cues for robust deepfake detection. The proposed architecture employs parallel feature-extraction pipelines, using MobileNetV2 to derive visual representations from video frames and a Mel-spectrogram-based encoder for audio signals. These modality-specific embeddings are subsequently fused through a shared classification network to capture cross-modal artifacts indicative of synthetic media effectively. The proposed framework is evaluated on three publicly available benchmarks: FakeAVCeleb, CelebDF, and KoDF. Experimental results demonstrate strong performance, achieving accuracies of 96.9%, 97.0%, and 88.4%, respectively. Furthermore, ablation studies confirm that multimodal fusion consistently outperforms unimodal approaches, yielding improvements of 3.1% over video-only and 5.4% over audio-only models of FakeAVCeleb. These findings highlight the critical importance of integrating complementary audio-visual information for reliable deepfake detection and demonstrate the effectiveness of
lightweight multimodal architectures for real-world deployment. 

 # Requirements
 
1. Hardware
GPU: NVIDIA RTX 2080 Ti or higher (≥11 GB VRAM recommended, experiments in this work were conducted on an RTX 3090 with 24 GB).
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
<img width="1536" height="1024" alt="Model_Pipeline" src="https://github.com/user-attachments/assets/89cba0cc-f900-4724-850d-8770e0a0f9fb" />


# Model Architecture
<img width="1024" height="1536" alt="Model_arch" src="https://github.com/user-attachments/assets/4531fb6b-0faa-4395-908b-eb8da466a96a" />



# Authors
1. Shobhit Tyagi∗, 2. Naveen Chauhan∗, 3. Divakar Yadav†, 4. Prashant Upadhyay‡, 5. Piyush Rawat §

∗Department of CSE&IT, Jaypee Institute of Information Technology, Noida, U.P., India, Email: shobhit.tyagi@jiit.ac.in, naveen.chauhan@jiit.ac.in

†School of Computer and Information Sciences, IGNOU, New Delhi, India Email: divakaryadav@ignou.ac.in

‡Department of CSE, SSET, Sharda University, Greater Noida, India, Email: prashanttheace@gmail.com

§Department of CSE, Delhi Technological University, Delhi, India, Email: psh.rawat@gmail.com

