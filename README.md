\documentclass{article}

\title{Generative AI: Denoising Autoencoder Final Report}
\author{Zahra Rahmani \and Adi Ghosh}
\date{}

\begin{document}

\maketitle

\section*{Abstract}
The primary aim of this project is to identify the most suitable DAE architecture for handling specific noise profiles in corrupted images. By employing a rigorous methodology involving grid search and systematic exploration of different combinations of hyperparameters and architectures, we aim to enhance the quality and usability of noisy images across various applications.

\section{Introduction}
In this study, we aim to discern the effectiveness of Variational Autoencoders (VAEs) and Denoising Autoencoders (DAEs) in image denoising tasks across various noise profiles. Image denoising is crucial in numerous applications, from medical imaging to digital photography. This report delves into the methodology, results, and implications of our findings.

\subsection{Denoising potential of generative models}
Our goal is to identify the best deep learning architectures for cleaning up noisy images, specifically exploring VAEs and DAEs across different types of noise. This study is crucial for improving the quality of images that are corrupted by noise, making them more useful in a variety of applications.

\subsection{The challenge of image denoising}
The complexity of our problem lies in the variety of ways images can become corrupted by noise during acquisition and transmission. Addressing this challenge is crucial, as developing effective denoising models plays a significant role in fields where high-quality image data is essential for precise analysis and decision-making.

\subsection{Objectives of the denoising exploration}
In our exploration of image denoising, we set several key objectives, including methodically evaluating different configurations of VAEs and DAEs across a range of noise profiles, identifying the most effective autoencoder architecture for each noise type, and optimizing resource usage for practical deployment.

\section{Methodology}
\subsection{Data source and noise types}
We utilized the MNIST and Fashion-MNIST datasets as foundational sets of clean images and introduced a variety of noise profiles into these datasets to challenge our models and simulate real-world scenarios.

\subsection{Architectural choices in denoising}
We experimented with varying depths of encoder and decoder layers, different activation functions, and training durations to assess the efficiency of image reconstruction and noise reduction.

\subsection{Loss function}
We selected the Kullback-Leibler (KL) Divergence as our primary loss function due to its effectiveness in the context of Denoising Autoencoders (DAEs) and the denoising process.

\section{Results and Analysis}
\subsection{Results}
From the grid search, we identified optimal architectures for different noise profiles, with varying numbers of encoder layers, decoder layers, and activation functions.

\subsection{Novelty}
Our project fills a significant gap in academic research regarding the identification of the most suitable architecture for each specific type of noise in image processing.

\subsection{Challenges and Limitations}
Technical challenges such as automatic shutdown of jobs in the High-Performance Computing (HPC) environment and the complexity of finding the best architecture were encountered during the project.

\section{Conclusion and Future Direction}
Our experiments have yielded promising data indicating optimal combinations of variables for configuring DAE architectures. Looking ahead, we plan to broaden the scope of our research to include a wider array of image datasets and explore the integration of more advanced neural network techniques.

\section*{References}
\begin{enumerate}
    \item Bengio, Yoshua, et al. "Generalized denoising auto-encoders as generative models." Advances in neural information processing systems 26 (2013).
    \item Gondara, L. "Medical Image Denoising Using Convolutional Denoising Autoencoders," 2016 IEEE 16th International Conference on Data Mining Workshops (ICDMW), Barcelona, Spain, 2016.
\end{enumerate}

\end{document}
