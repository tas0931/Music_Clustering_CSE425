**🎶 Unsupervised Music Clustering with VAEs**

**Overview:**
This project explores unsupervised music clustering using Variational Autoencoders (VAEs) with multi-modal features (audio, lyrics, genre). We progressively implement three levels of complexity:

Basic VAE – audio features only

Convolutional VAE – audio + lyrics embeddings

Advanced VAEs (Beta-VAE, CVAE) – incorporating genre information

**Dataset:**
FMA (Free Music Archive) subset: 1,910 tracks across 8 genres

Features: MFCC audio, lyrics embeddings, genre labels

Dataset Drive Link:  https://drive.google.com/drive/folders/1vI6cgQ4MN_3vgbOsjszqvxqUJaSwVSYI?usp=sharing

**Methods:**
Feature extraction: MFCC (audio), Sentence Transformers (lyrics)
Architectures: VAE, Beta-VAE, CVAE
Clustering: K-Means, Agglomerative, DBSCAN
Evaluation: Silhouette, Calinski-Harabasz, Davies-Bouldin, NMI, ARI, Purity

**Key Findings:**
Beta-VAE achieved best clustering quality (Silhouette: 0.186)
Genre alignment remained moderate (NMI: 0.151, ARI: 0.109) → clusters capture musical traits beyond genre
Multi-modal features (audio + lyrics) did not consistently improve results
Posterior collapse observed (15.6% active latent dimensions), suggesting room for architectural improvements

All results drive link: https://drive.google.com/drive/folders/1vI6cgQ4MN_3vgbOsjszqvxqUJaSwVSYI?usp=sharing

Source of Music Data (FMA): https://github.com/mdeff/fma.git (Only fma_small.zip and fma_metadata.zip is used)

All tasks (easy,medium,hard) have been implemented in colab notebooks (with results and output) which is located in code(src) folder.

**Conclusion:**
VAEs, especially Beta-VAE, show strong potential for music representation learning and clustering. Learned clusters highlight musical characteristics beyond genre boundaries


