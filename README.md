# C2EFI Script 🥂

A script designed to automate the process of compiling, testing, and creating bootable UEFI applications using the GNU-EFI library. It simplifies the workflow by integrating dynamic input, automated compilation, and optional testing in QEMU.

## Requirements
- **GCC**
  - Install using `sudo apt install gcc` in Debian/Ubuntu

- **GNU-EFI Library**:
  - Install using your package manager (e.g., `sudo apt install gnu-efi` on Debian/Ubuntu).

- **QEMU** (optional):
  - For testing the application in a virtual environment. [QEMU Install](https://www.qemu.org/download/)

## Steps

1. Place your UEFI source file (e.g., `main.c`) in the working directory.
2. Run the script using:

   ```
   sudo bash ./run.sh
   ```
3. Provide the following inputs when prompted:
   - Path to the source `.c` file.
   - Paths to GNU-EFI libraries and headers.
   - Note: It is always recommended to use `/usr/include/efi` as Header [GNU-EFI wiki](https://wiki.osdev.org/GNU-EFI)
4. Finally, you will be prompted to live-run (test) .efi on QEMU

## Working of Script

![working-ezgif com-optimize](https://github.com/user-attachments/assets/750b8641-7c90-4c90-b88e-2d643ea60e4d)
