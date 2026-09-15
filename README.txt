CLLMSE Practical Lab - cllmse-lab
==================================

Pick the binary that matches your OS/CPU and run it. No installation,
no internet access, no third-party dependencies. It listens on
127.0.0.1 only.

  macOS Apple Silicon (M1/M2/M3/M4):
    chmod +x cllmse-lab-darwin-arm64
    ./cllmse-lab-darwin-arm64

  macOS Intel:
    chmod +x cllmse-lab-darwin-amd64
    ./cllmse-lab-darwin-amd64

  Linux x86_64:
    chmod +x cllmse-lab-linux-amd64
    ./cllmse-lab-linux-amd64

  Linux ARM64:
    chmod +x cllmse-lab-linux-arm64
    ./cllmse-lab-linux-arm64

  Windows x86_64:
    Double-click cllmse-lab-windows-amd64.exe
    (or from PowerShell: .\cllmse-lab-windows-amd64.exe)

Once it prints "listening at http://127.0.0.1:8090", open that URL in
your browser.

Troubleshooting
---------------
* Port already in use -> set PORT before launching:
    PORT=9090 ./cllmse-lab-darwin-arm64
* macOS Gatekeeper "cannot be opened" -> run once:
    xattr -d com.apple.quarantine cllmse-lab-darwin-arm64
* Windows SmartScreen "protected your PC" -> click More info -> Run anyway.
* Linux "Permission denied" -> chmod +x the binary first.

See LAB.md (in the exam package root) for full step-by-step instructions
and how the 10 bonus exam questions map to this lab.
