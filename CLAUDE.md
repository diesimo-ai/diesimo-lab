# CLAUDE.md — Diesimo Lab

## What This Repo Is

Technical showcase and R&D hub for Edge AI consulting. Portfolio + pipeline factory + knowledge base.
Revenue target: $1M through audits, pilots, retainers, productized offerings.

## Commands

```bash
nox -s lint              # Black + Ruff
nox -s format            # Auto-format
nox -s test              # pytest
nox -s bench             # Run benchmarks
uv run pytest path/to/test.py   # Single test
uv pip install -r requirements-dev.txt  # Dev deps
```

## Coding Standards

- **Formatter**: Black, line length 100
- **Linter**: Ruff
- **Docstrings**: Google style on public APIs
- **Type hints**: Required on public APIs
- **Benchmark CSV schema**: `model_name,hardware,precision,batch_size,latency_ms,throughput_fps,power_w,ops_per_watt,accuracy_metric`

## File Conventions

- `benchmarks/{platform}/` — README.md (hardware specs + setup), latency.csv, run_bench.py, results/
- `models/{modality}/{task}/` — README.md (model card), model.onnx, config.json, benchmark.md
- `datasets/{domain}/` — README.md (dataset card), dvc.yaml, metadata.json
- `cases/{vertical}/` — README.md (case study), benchmarks.md, discovery.md

## Error Avoidance

- No benchmark without hardware specs and software versions (CUDA, TensorRT, OS)
- No latency claim without CSV backing
- No model card without benchmark on target hardware
- No case study without ROI/TCO numbers
- Never say "fast" or "efficient" — use latency_ms, throughput_fps, OPS/W
- Measure end-to-end: preprocessing + inference + postprocessing
- Always compare against baseline (cloud, CPU, FP32)

## Verification Rules

- Every benchmark README: reproduction steps + CSV + logs
- Every model: config.json + benchmark.md + runs on target hardware
- Every case study: financial analysis (CapEx, OpEx, ROI, payback) + baseline comparison
- Every dataset: metadata.json + dvc.yaml + README with collection methodology

## Edge Repo Sync

Source repos (local dev, public on GitHub):
- edge-language: `/home/muntu/Work/business/diesimo/consulting/engineering/projects/project-lib/edge-language`
- edge-audio: `/home/muntu/Work/business/diesimo/consulting/engineering/projects/project-lib/edge-audio`
- edge-vision: `/home/muntu/Work/business/diesimo/consulting/engineering/projects/project-lib/edge-vision`
- edge-time-series: `/home/muntu/Work/business/diesimo/consulting/engineering/projects/project-lib/times-series`
- edge-multimodal: `/home/muntu/Work/business/diesimo/consulting/engineering/projects/project-lib/multimodal`
- edge-agents: `/home/muntu/Work/business/diesimo/consulting/engineering/projects/project-lib/agents`
- edge-ai-engineering: `/home/muntu/Work/Lab/projects/edge-ai-engineering`

Sync method: script-based copy after validation. Tracked in `sync-manifest.json`.

## Hardware Platforms

- **TinyML**: Arduino Nano 33 BLE (64MHz Cortex-M4, 256KB RAM)
- **Entry**: Raspberry Pi 3B+/4/5 (1.4GHz Cortex-A53, 1-8GB RAM)
- **High-perf**: NVIDIA Jetson Nano/Orin (128-2048 CUDA cores, 4-64GB RAM, TensorRT)

## Detailed Module Guides

For templates, workflows, and deep dives, see `.github/instructions/`:
- Benchmarks → `.github/instructions/BENCHMARKS.instructions.md`
- Models → `.github/instructions/MODELS.instructions.md`
- Datasets → `.github/instructions/DATASETS.instructions.md`
- Cases → `.github/instructions/CASES.instructions.md`
- Edge repos → `.github/instructions/POPULATE-EDGE-REPOS.instructions.md`

## Plan Mode

Use Plan mode for multi-step tasks: benchmarking new platforms, creating case studies, syncing from edge repos, multi-file changes.

## Communication Style

- Technical precision: latency, throughput, OPS/W — not "fast" or "efficient"
- Numbers first, explanations second
- Minimal diffs over rewrites
- When info is missing, ask — don't guess
