# Watermark Remover (demo)

Single-page browser tool. Choose an image, paint over the watermark, tap Remove, download.
Runs on-device with the MI-GAN inpainting model (MIT licence, `migan_pipeline_v2.onnx.gz` (gzipped to fit the 25 MB web upload limit)) via onnxruntime-web. Nothing is uploaded.

Limits: filled pixels are guessed. Detailed areas (faces, text, product detail) will not match the original. Use only on images you own or may edit.
Serve over http (e.g. `python3 -m http.server`, or GitHub Pages) so the model file can load.
