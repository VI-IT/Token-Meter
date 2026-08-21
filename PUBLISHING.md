# Publishing a new Token Meter by VI-IT version

Token Meter by VI-IT checks the latest public release of:

`https://github.com/VI-IT/Token-Meter`

To publish an update:

1. Build and test an installer with a version higher than the installed version.
2. Open the repository's **Releases** page and choose **Draft a new release**.
3. Create a semantic version tag such as `v1.1.0`.
4. Attach the binary with this exact filename: `Token-Meter-by-VI-IT-Setup.exe`.
5. Attach `SHA256.txt` and add release notes.
6. Publish the release and mark it as the latest release.

Installed copies check GitHub at startup and every six hours. When the release tag is newer, Token Meter by VI-IT downloads the installer, shows download and installation progress, installs it unattended, and restarts automatically. If the automatic installation fails, the app keeps a manual download fallback visible.

The public repository contains release documentation and binaries only. Do not upload the private application source.
