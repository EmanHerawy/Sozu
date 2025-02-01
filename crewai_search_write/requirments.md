# Project Setup Guide

## Prerequisites

- Python (Download from [python.org](https://www.python.org/downloads/))
- pip (included with Python installation)
- VS Code (or preferred IDE)

### Required VS Code Extensions
- Python (by Microsoft)
- Python Environment Manager
- Python IntelliSense

## Installation Verification

1. Verify Python installation:
   ```bash
   python --version
   ```

2. Verify pip installation:
   ```bash
   pip --version
   ```

3. Upgrade pip if needed:
   ```bash
   python -m pip install --upgrade pip
   ```

## Required Packages

Install the following packages:
```bash
pip install crewai==0.28.8
pip install crewai_tools==0.1.6
pip install langchain_community==0.0.29
```

To verify package installations:
```bash
pip show crewai
pip show crewai_tools
pip show langchain_community
```

## Troubleshooting

### Windows Long Path Issue

If you encounter long file path issues on Windows, follow these steps:

1. Open Registry Editor (`Win + R`, type `regedit`)
2. Navigate to:
   ```
   HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FileSystem
   ```
3. Locate `LongPathsEnabled`
4. Set value to `1`
5. Restart your computer