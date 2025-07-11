Gated Relative-position and Importance-aware Transformer for 360° IQA
---
📘 Abstract
---
Immersive visual content, such as virtual reality and 360° imagery, presents unique challenges for image quality assessment (IQA) due to spherical distortions, stitching artifacts, and uneven importance across different viewing regions. To address these issues, we present GRIT360, a transformer-based framework for blind omnidirectional IQA (OIQA) that incorporates region-based feature processing and adaptive weighting.

GRIT360 begins by dividing each equirectangular image into 120 viewports. To focus on areas that are more likely to be viewed by users, we apply a selective masking strategy that excludes less informative regions based on common viewing tendencies. The retained viewports are then passed through a hierarchical Swin Transformer backbone, which extracts spatial features at multiple scales.

To enhance attention modeling across different regions, we propose a Viewport Weighted Gated Relative Position Bias (VW-GRPB) module that applies learnable positional encoding and dynamic gating to regulate attention flow. Additionally, we introduce a learnable viewport weighting mechanism, initialized with simple heuristic values, that adjusts the contribution of each viewport during feature encoding and final quality prediction. These weights are optimized jointly with the model parameters through training.

Our framework employs a dual-headed prediction head to estimate both global image quality and individual viewport scores, allowing the model to capture both localized distortions and overall visual quality. We evaluated GRIT360 on three public datasets—CVIQ, OIQA, and ODI-IQA—where it achieves state-of-the-art performance, with PLCC and SRCC scores reaching up to 0.950 and 0.961, respectively. The results demonstrate the benefits of region-aware design and adaptive weighting in 360° IQA.
