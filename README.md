# chimahon-local-models

Downloadable on-device OCR payloads used by Chimahon.

## Structure

```
screenai_models/   # Lens OCR: TFLite models, protobuf configs, LM FSTs (-> models.zip)
paddle_ocr/        # Paddle OCR: PP-OCRv6 manga NCNN models + prebuilt libpaddle_ocr.so per ABI (-> paddle-ocr.zip)
```

## Release

Trigger the `Release Models` workflow manually with a version tag:

```bash
gh workflow run release-models.yml -f version=v1.0
```

Or use the GitHub UI: Actions → Release Models → Run workflow.
