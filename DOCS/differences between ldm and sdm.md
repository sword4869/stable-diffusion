# stable多的
```bash
.
├── configs
│   └── stable-diffusion
│       └── v1-inference.yaml
├── ldm
│   ├── models
│   │   └── diffusion
│   │       ├── dpm_solver
│   │       │   ├── __init__.py
│   │       │   ├── dpm_solver.py
│   │       │   └── sampler.py
├── scripts
│   ├── img2img.py
│   ├── tests
│   │   └── test_watermark.py
```
# stable与ldm不同的

```bash
.
├── ldm
│   ├── models
│   │   └── diffusion
│   │       ├── ddim.py     # 多了个 stochastic_encode(), decode()
│   ├── modules
│   │   ├── encoders
│   │   │   └── modules.py  # 多了 CLIP 相关的 FrozenCLIPEmbedder
├── scripts
│   └── txt2img.py          # 很大
```