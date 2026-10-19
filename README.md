# SBT-DF204 Case Study 3: Investigating Memory Evidence

## Overview
This repository contains the forensic evidence logs, Volatility 2 outputs, reconstructed UTC timeline, and executive report for SBT-DF204 Case Study 3: Investigating Memory Evidence (Investigating Suspected Illegal File Transfer From Memory Evidence).

## Repository Structure
SBT-DF204-Investigating-Memory-Evidence/
├── evidence/              # Hash records and memory image documentation (memdumpWin7.mem)
├── reports/               # Volatility extraction reports, evidence logs, and formal investigation report
├── screenshots/           # Labeled command execution and verification captures
└── README.md              # Project overview and findings summary

## Key Investigation Highlights
* Memory Ingestion: Windows 7 SP1 memory image (memdumpWin7.mem) securely acquired and hashed.
* Profile Validation: Identified profile Win7SP1x86_23418 via imageinfo and registry verification.
* Process & Network Analysis: Correlated Chrome process (PID 2388) network artifacts with a downloaded document (secret_file.docx) originating from 192.168.56.5.
* Command History & Removable Media: Reconstructed command prompt execution (copy secret_file.docx F:) mapping to a generic USB storage device (General UDisk) under user profile IEUser.
