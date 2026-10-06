# LocalEnhance runtime models

This public repository hosts metadata and release assets used by LocalEnhance. Model packages are distributed only as GitHub Release assets and are never embedded in the iOS IPA.

## Release `models-v1`

- `source-faithful-sr-x2.mlpackage.zip`: Core ML conversion of the BSD-licensed Real-ESRNet x4 photographic model. LocalEnhance runs the model at x4 and downsamples the rendered tile to a source-faithful 2x result.
- `monocular-depth.mlpackage.zip`: Core ML conversion of the MIT-licensed MiDaS v2.1 Small model at 256x256.

The app verifies SHA-256 before extraction and compiles the package with `MLModel.compileModel(at:)` at runtime. No photographs are uploaded.
