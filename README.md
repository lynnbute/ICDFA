# CIP-B101 Lab 1B — PC System Fundamentals, Disk Sectors and Partition Analysis

## Overview

This repository contains my practical work and supporting evidence for **CIP-B101 Lab 1B: PC System Fundamentals, Disk Sectors and Partition Analysis**.

The lab introduces fundamental concepts in digital forensics and computer system analysis, with a focus on understanding system specifications, storage devices, disk partitions, filesystems, processes, boot mechanisms, and forensic evidence found at different system layers.

The practical work was performed using **Windows 11 and Kali Linux**, with command-line tools used to collect and examine system and disk information.

## Objectives

The lab covered:

- Identifying and documenting computer system specifications.
- Understanding the different layers where digital forensic evidence may exist.
- Investigating running processes and process identifiers (PIDs).
- Examining disks, partitions, and logical volumes.
- Understanding disk sectors and their role in forensic analysis.
- Identifying partitioning schemes such as **MBR and GPT**.
- Understanding the **UEFI/boot process**.
- Identifying filesystems and their characteristics.
- Performing basic disk and hexadecimal inspection.
- Applying manual calculations and interpreting forensic evidence.
- Documenting observations and explaining their forensic significance.

## Operating Systems

### Windows 11

Windows was used for system-level investigation and process analysis.

Tools and commands included:

- `msinfo32`
- PowerShell
- `Get-Disk`
- `Get-Partition`
- `Get-Volume`
- `Get-Process`

The Windows system was identified as using **UEFI and GPT**, with a **SK hynix SC401 512 GB** storage device.

> Note: `wmic` was unavailable on the Windows installation, so PowerShell commands were used as alternatives for obtaining disk and system information.

### Kali Linux

Kali Linux was used for additional disk, partition, filesystem, and hexadecimal analysis.

Tools and commands included:

- `fdisk`
- `parted`
- `lsblk`
- `blkid`
- `df`
- `dd`
- `xxd`

## Evidence and Forensic Methodology

The practical work follows a structured evidence-documentation approach:

**Command → Screenshot → Observation → Forensic Significance**

For each investigation step, the command or procedure is documented, relevant output is captured, observations are recorded, and the forensic importance of the result is explained.

The lab also considers evidence across different system layers, including:

- User activities
- Applications
- Operating system
- Disk and storage
- Memory/process activity

## Process Investigation

Process analysis was used to understand the difference between:

- **Program** — a stored executable or set of instructions.
- **Process** — a running instance of a program.
- **Thread** — an execution path within a process.

Process information such as process names and PIDs can assist investigators in identifying suspicious or unexpected activity during live forensic triage and malware investigations.

## Disk and Partition Analysis

The lab examines:

- Physical disks
- Disk sectors
- Partitions
- Logical volumes
- Filesystems
- MBR
- GPT
- UEFI
- Boot sequence

Disk and partition information was collected using both Windows PowerShell and Kali Linux utilities.

## Repository Contents

This repository contains the practical report, supporting screenshots/evidence, and relevant files produced during the lab.

The material is intended for **educational and digital-forensics training purposes**.

## Key Learning Outcomes

Through this lab, I gained practical experience in:

1. Collecting system information for forensic documentation.
2. Investigating processes and identifying process-related evidence.
3. Understanding disk structures and partitioning schemes.
4. Using Windows PowerShell for forensic system enumeration.
5. Using Kali Linux tools for disk and filesystem analysis.
6. Understanding the forensic relevance of MBR, GPT, UEFI, and filesystems.
7. Documenting technical findings with supporting evidence.

## Course

**Course:** CIP-B101  
**Lab:** Lab 1B — PC System Fundamentals, Disk Sectors and Partition Analysis  
**Field:** Digital Forensics
