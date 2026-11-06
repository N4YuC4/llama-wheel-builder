# llama-wheel-builder

Automated GitHub Actions builder for `llama-cpp-python` Linux wheels with native NVIDIA Blackwell (`sm_120`), Hopper (`sm_90`), and Ada Lovelace (`sm_89`) CUDA acceleration.

## Features
- **CUDA 12.8 Toolkit** with `nvcc` compilation for `sm_120`.
- Multi-architecture SASS binary generation (`ARCHITECTURES=80;86;89;90;120`).
- Generates Python 3.12 `linux_x86_64` wheels for Hugging Face Spaces (ZeroGPU).
- Automatically uploads built `.whl` as an Action Artifact.
- Optionally creates a GitHub Release and/or uploads directly to Hugging Face Spaces.

## How to Run
1. Go to the **Actions** tab on GitHub.
2. Select **Build Blackwell sm_120 Wheel**.
3. Click **Run workflow**.
4. Once completed (~10-15m), download the wheel from **Artifacts** or **Releases**.
