# G-INR: Gated Implicit Neural Representations for Medical Image Segmentation

We propose G-INR, a gated implicit neural representation that uses a residual dual-frequency architecture to control low and high frequency information and meta-learned initialization to make it easy to modify at test time. The gating method selectively amplifies border details while maintaining consistency in homogeneous areas. 

## Architecture

<img width="1397" height="616" alt="image" src="https://github.com/user-attachments/assets/cc9119d8-5c3c-490e-8669-aa46ae8a03d3" />

**Figure 1** . Proposed gated implicit neural representation. The INR adaptively mixes low- and high-frequency sinusoidal responses through a learnable gating function \( g \), enabling flexible signal representation across frequency bands.

<img width="639" height="434" alt="image" src="https://github.com/user-attachments/assets/ed8372c5-d293-43b0-9b0b-2e42afb67160" />

**Figure 2.** Meta-learning framework for INR initialization. We learn optimal initial parameters \( \theta^{*} \) and \( \phi^{*} \) for an \( L \)-layer reconstruction network, enabling fast adaptation to new signals.

## Repository Structure

- `G-INR_3d.ipynb`: Training and evaluation code for G-INR on the OASIS 3D MRI dataset.
