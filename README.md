# Cybersec-Suite
This project is a testing tool, not a complete security solution. It cannot detect every vulnerability, and some checks require carefully configured test accounts or infrastructure. Its cloud analysis is based on configuration files rather than live cloud accounts. It should only be used on systems you own or have explicit permission to test.
How to run it
1. Download and extract the ZIP.
2. Open the extracted folder in VS Code.
3. Open a terminal in that folder.
4. Run:
python -m venv .venv
python -m pip install -r requirements.txt
python server.py --bootstrap-admin


5. Open **http://127.0.0.1:8000** in your browser.
6. Use the generated administrator password printed in the terminal to sign in.
The password is generated at first setup, not hardcoded into the project.
Testing results
224 automated tests passed
Four existing warnings remain, including deprecation and duplicate API operation-ID warnings.



FixProof demonstration passed
19 out of 19 checks passed, including vulnerability detection and regression detection.



Deployment configuration validated
Python compilation and Compose YAML validation passed. A Docker image build was not run in this environment.



Before using this as a startup product: the application still needs further hardening for public deployment, particularly centralized session revocation, shared rate limiting, CSRF protection, and multi-tenant data isolation. The README documents these limitations.
The ZIP contains the updated source code, tests, templates, dependencies, and deployment files. Your original uploaded ZIP has not been modified.
