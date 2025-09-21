# DiT-Flow Policy

A flow-based visuomotor policy that uses continuous normalizing flows and Diffusion Transformers (DiT) for robotic action prediction. This implementation combines flow matching with transformer architectures to generate action sequences conditioned on visual and proprioceptive observations.

## Key Features

- **Flow Matching**: Uses continuous normalizing flows instead of traditional diffusion denoising
- **Transformer Architecture**: DiT blocks with adaptive layer normalization and gating
- **Multi-modal Input**: Supports robot state, environment state, and multi-camera observations
- **Action Chunking**: Predicts action horizons with configurable execution steps

## Implementation

This policy is essentially based on the implementation from:
- **LeRobot Pull Request #680**: https://github.com/huggingface/lerobot/pull/680/files

## Papers

This policy is derived from ideas presented in:

- **DiT-Policy**: https://github.com/SudeepDasari/dit-policy/
- **DiT (Diffusion Transformers)**: https://github.com/facebookresearch/DiT/

## Citations

```bibtex
@article{peebles2023scalable,
  title={Scalable diffusion models with transformers},
  author={Peebles, William and Xie, Saining},
  journal={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  pages={4195--4205},
  year={2023}
}
```