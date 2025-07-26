Gated Relative-position and Importance-aware Transformer for 360° IQA
---
📘 Abstract
---

Immersive formats such as 360° images and virtual reality are increasingly adopted in modern broadcasting and adaptive streaming applications, where maintaining perceptual visual quality is critical for enhancing user experience. Unlike traditional planar images, omnidirectional content introduces unique challenges—such as spherical distortions, stitching artifacts, and non-uniform perceptual saliency—that conventional quality metrics fail to model effectively.

To address these issues, we propose GRIT360, a no-reference image quality assessment framework specifically designed for omnidirectional imagery. GRIT360 divides each equirectangular image into 120 structured viewports and applies a perceptual bottom-masking strategy to discard geometrically distorted regions based on empirical gaze priors.

These viewports are processed through a hierarchical Swin Transformer backbone to extract multi-scale spatial features. A novel Viewport-Weighted Gated Relative Position Bias (VW-GRPB) module is introduced to enhance spatial attention through learnable position encoding and gated modulation. Additionally, a trainable viewport weighting mechanism dynamically adjusts the contribution of each region during feature fusion and quality regression.

GRIT360 adopts a dual-headed prediction scheme that estimates both global image quality and viewport-level perceptual fidelity. Evaluations on three public datasets—CVIQ, OIQA, and ODI-IQA—demonstrate that GRIT360 achieves state-of-the-art performance. On the ODI-IQA dataset, it attains PLCC and SRCC scores of 0.973 and 0.968, respectively, affirming its suitability for real-time perceptual quality modeling in immersive streaming and broadcasting scenarios.
