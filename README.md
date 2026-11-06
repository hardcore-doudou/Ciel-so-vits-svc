# Ciel — so-vits-svc 4.1

English | [简体中文](README_CN.md)

An unofficial Ciel singing voice conversion experiment based on so-vits-svc 4.1. It converts the timbre of existing vocals rather than generating speech from text.

## Project status

Documentation release only. The local configuration and training log have been inspected; checkpoint loading and inference testing remain pending. Model weights, configuration files, original recordings, and audio demonstrations are not distributed in this release.

## Model information

| Property | Value |
| --- | --- |
| Character | Ciel |
| Framework | so-vits-svc 4.1, reported by the trainer |
| Exact framework revision | Unverified |
| Latest checkpoint observed | G_31200.pth |
| Checkpoint size | 627,905,309 bytes (approximately 599 MiB) |
| Saved training step | 31,200, confirmed by training log |
| Epoch at checkpoint save | 459 |
| Speaker mapping | Ciel → 0 |
| Sample rate | 44,100 Hz |
| Speech encoder | vec768l12 |
| Vocoder | nsf-hifigan |
| Dataset duration and clip count | Unverified |
| Inference compatibility and quality | Not yet tested |

These values describe the files inspected on November 6, 2026. The latest checkpoint is not necessarily the best-performing checkpoint.

## Usage and availability

No downloadable model is currently provided. Inference requires a compatible framework, checkpoint and matching configuration. Tested commands and download instructions will be added after validation and distribution approval.

See the bilingual [training record](docs/training.md) for verified settings and remaining checks.

## Rights and distribution

This is an independent fan experiment, with no claimed affiliation with or endorsement by the original creators or performer. Third-party rights remain with their respective owners. This documentation does not grant permission to redistribute weights or third-party material. Any future model or demonstration release requires confirmation of distribution rights and applicable terms.
