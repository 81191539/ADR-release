# ADR Binary Release

This repository provides a closed-source Windows x64 binary release of the ADR solver for academic exchange and evaluation.

No source code is included in this repository.

## Contents

```text
bin/
  df2d.exe
input/
  input_parameter_0001.toml
  input_parameter_reference.toml
run_example.bat
NOTICE.md
LICENSE.md
```

## Requirements

- Windows 10/11 x64.
- Run from a writable folder, because the program writes results to `output/`.

## Quick Start

Double-click `run_example.bat`, or run from PowerShell:

```powershell
.\bin\df2d.exe --case 1 --force-restart
```

The solver reads case files from `input/` and writes results to `output/`.
The included case `input_parameter_0001.toml` is a small smoke-test case for confirming that the binary runs; it is not intended as a validation or publication case.

## Input Files

Use TOML case files named like this:

```text
input/input_parameter_0001.toml
input/input_parameter_0002.toml
```

`input/input_parameter_reference.toml` is a copyable parameter template.

## Distribution Notice

This binary is provided only for academic exchange and evaluation. Redistribution, commercial use, reverse engineering, decompilation, disassembly, modification, and source extraction are not authorized unless separately approved by the copyright holders. See `LICENSE.md` and `NOTICE.md`.
