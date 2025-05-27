# Security Policy

The Real-Time Drowsiness Detection team takes the security of our project seriously. We appreciate your efforts to responsibly disclose your findings, and we will make every effort to address security issues in a timely manner.

## 🛡️ Reporting a Vulnerability

If you discover a security vulnerability within this project, please **DO NOT** create a public GitHub issue. Instead, we encourage you to report it privately.

Please send an email to the project maintainer, Oussema Mansouri (or provide a dedicated security email address if available).

When reporting a vulnerability, please include the following details:

* A clear and concise description of the vulnerability.
* Steps to reproduce the vulnerability. Please be as specific as possible.
* The version or commit hash of the project you were using.
* Any potential impact of the vulnerability.
* Any suggested mitigations, if you have any.

We will acknowledge your email within 48 hours and will aim to provide a more detailed response within 72 hours, including a plan for addressing the vulnerability. We kindly ask that you do not disclose the vulnerability publicly until we have had a chance to investigate and release a patch.

We will do our best to keep you informed of our progress throughout the process.

## ⚠️ Scope

This security policy applies to the code and dependencies within the `Real-Time-Drowsiness-Detection` repository. Please note that while we strive for security, this system relies on third-party libraries (TensorFlow, OpenCV, etc.). Vulnerabilities found in those libraries should be reported to their respective maintainers. However, if a vulnerability in a dependency directly impacts this project's security in a specific way, please let us know.

## ✅ Supported Versions

As an open-source project, we generally provide security updates for the **latest version** on the main branch. We encourage users to stay updated with the most recent release to benefit from the latest features and security patches.

| Version | Supported          |
| :------ | :----------------- |
| Latest  | :white_check_mark: |
| < Latest| :x:                |

## 🔐 Security Best Practices for Users

* **Keep Dependencies Updated:** Regularly update the required libraries (`tensorflow`, `opencv-python`, etc.) by running `pip install -r requirements.txt --upgrade`. New versions often include security fixes.
* **Webcam Access:** Be aware that this application requires access to your webcam. Only run this software in an environment where you are comfortable with webcam usage. Ensure no unauthorized software is running that could misuse this access.
* **Input Data:** While this project primarily uses webcam input, be cautious if modifying it to use pre-recorded video files. Ensure that any video files come from trusted sources.

## 🚫 Disclaimer

This Real-Time Drowsiness Detection system is provided "as is" and is intended for demonstration and educational purposes. **It is NOT a certified safety device and should NOT be solely relied upon to prevent drowsy driving or any other safety-critical situation.** Always prioritize responsible driving habits, take regular breaks, and never drive when feeling tired. The maintainers and contributors of this project assume no liability for any incidents or damages that may occur during its use or misuse.

We appreciate your help in keeping this project secure.
