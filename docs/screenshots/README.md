# Stage 1 visual QA

These screenshots were captured by the passing Development quality workflow
for development main commit
`e66ca671c446ef1c2b1f353c7475f0a9db06cff3`. The same workflow built and
checksum-locked the browser-facing `site/` bytes in this repository.

- `desktop.jpg`: 1440 × 1000 desktop viewport
- `mobile.jpg`: 390 × 844 mobile viewport
- `webgl2-required.jpg`: 1440 × 1000 forced-no-WebGL2 compatibility view
- `browser-diagnostics.txt`: captured HTTP and browser diagnostic record

The compatibility capture overrides the browser's WebGL2 context request,
then verifies the exact requirement heading and recovery guidance, the absence
of the interactive map shell, and the absence of console or page errors.

The screenshots are pull-request evidence and are not part of the deployed
`site/` inventory.
