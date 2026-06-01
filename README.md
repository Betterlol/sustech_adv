# sustech_adv WebGL Deploy

This repository deploys the Unity WebGL page shell from the webgl directory to Vercel.

## Update Deployment

1. Build Unity WebGL into webgl.
2. Commit and push.
3. Vercel auto-deploys from GitHub.

## Vercel + CDN (recommended for large data file)

The page can load large Unity artifacts from a CDN while keeping index.html on Vercel.

1. Upload these files to your CDN under Build/:
	- WebGL Builds.data.unityweb
	- WebGL Builds.framework.js.unityweb
	- WebGL Builds.wasm.unityweb
2. Keep these files in this repo for local test:
	- webgl/index.html
	- webgl/Build/WebGL Builds.loader.js
	- webgl/TemplateData/*
3. Open your page with a CDN parameter:
	- https://your-app.vercel.app/?cdn=https://cdn.example.com

### Required CDN headers

For *.unityweb files, configure:

- Content-Encoding: br
- Build/*.wasm.unityweb -> Content-Type: application/wasm
- Build/*.framework.js.unityweb -> Content-Type: application/javascript
- Build/*.data.unityweb -> Content-Type: application/octet-stream

### Optional global variable mode

Before the Unity script runs, you can define:

- window.__UNITY_CDN_BASE__ = "https://cdn.example.com"

If set, this value is used as the CDN base.
