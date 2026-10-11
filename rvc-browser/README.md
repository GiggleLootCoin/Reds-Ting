# Red's Ultimate RVC — Browser Edition

A client-side RVC v2 voice-conversion interface using RVC-Web-Runtime.

## Goal

This version removes the Hugging Face ZeroGPU runtime from the inference path. Audio conversion happens in the browser using ONNX Runtime Web, WebAssembly, and WebGPU where supported.

## Mobile design

The UI is tuned for short clips on Android. Start with 5–15 seconds on a Galaxy A12.

## Model requirement

The browser runtime supports RVC v2 (768-dimension) models in ONNX and compatible PTH form. A training safetensors checkpoint is not directly accepted and must be exported to a compatible inference model first.

## Runtime

https://github.com/moyue23/rvc-web-runtime
