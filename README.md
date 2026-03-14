DevDoctor

DevDoctor is an open-source CLI tool that scans your development environment and project configuration to detect common issues before they break your workflow.

It analyzes your system, services, dependencies, and project setup to identify problems such as missing tools, misconfigured environment variables, inactive services, port conflicts, and insecure settings.

Run a single command and instantly get a clear diagnostic report with actionable suggestions.

DevDoctor helps developers spend less time debugging environment problems and more time building.

Features

Environment diagnostics for development tools and runtimes

Project configuration analysis (.env, dependencies, debug settings)

Service health checks (database, Redis, Docker, etc.)

Port conflict detection

Security checks for common misconfigurations

Parallel diagnostics engine for fast scans

Plugin system for extending checks

Multiple report formats (CLI, JSON, HTML)

CI/CD integration support

Installation
Using Homebrew (macOS / Linux)
brew install devdoctor
Download Binary

Download the latest release from:

https://github.com/your-org/devdoctor/releases

Then move the binary to your PATH.

Quick Start

Navigate to your project directory and run:

devdoctor scan

DevDoctor will automatically detect your project type and run diagnostics.

Example Output
DevDoctor Scan Report
────────────────────────

Environment
✔ Node.js installed
✔ Docker running

Services
❌ Redis not running
⚠ MySQL port conflict

Configuration
✔ .env file found
⚠ APP_DEBUG enabled

Security
⚠ API key detected

Health Score: 81%
Commands
Scan environment and project
devdoctor scan
Quick health check
devdoctor doctor
Generate report
devdoctor report
Fix detected issues
devdoctor fix
Supported Checks

DevDoctor currently supports checks for:

Environment setup

System configuration

Running services

Project configuration

Security issues

Future versions will support many additional frameworks and tools.

Plugin System

DevDoctor supports plugins that allow developers to extend diagnostics with custom checks.

Examples:

framework-specific checks

infrastructure diagnostics

security analysis

Plugins can register new checks that run automatically during scans.

CI/CD Integration

DevDoctor can be integrated into CI pipelines to automatically detect configuration problems.

Example:

devdoctor scan --format=json

This allows CI systems to parse results and fail builds if critical issues are detected.

Roadmap

Upcoming features include:

More framework detection

Advanced diagnostics engine

Expanded plugin ecosystem

Improved security checks

Performance diagnostics

Web-based report viewer

Contributing

Contributions are welcome.

To contribute:

Fork the repository

Create a new branch

Implement your changes

Submit a pull request

Before submitting, ensure all tests pass.

License

This project is licensed under the MIT License.

Vision

DevDoctor aims to become the universal diagnostic tool for development environments — a fast, reliable way to check the health of your project with a single command.
