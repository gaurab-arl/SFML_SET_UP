# SFML Setup with Orwell Dev-C++

This repository provides a comprehensive guide to setting up **SFML (Simple and Fast Multimedia Library)** with **Orwell Dev-C++** for C++ development. Follow the steps below to configure your environment and start creating projects with SFML.

---

## Prerequisites

### 1. Download Orwell Dev-C++
- Download Orwell Dev-C++ from SourceForge: [Orwell Dev-C++](https://sourceforge.net/projects/orwelldevcpp/)

### 2. Download SFML
- Visit the SFML download page: [SFML 2.4.2](https://www.sfml-dev.org/download/sfml/2.4.2/)
- Download the version compatible with GCC 4.9.2 TDM (SJLJ) - 64-bit:
  - **File:** `SFML-2.4.2-GCC-4.9.2-TDM-64-bit.zip`
  - **Size:** 15.8 MB

---

## Installation and Configuration

### Step 1: Extract SFML
1. Extract the downloaded SFML zip file to the following directory:
 C:\Program Files (x86)\Dev-Cpp\SFML-2.4.2

### Step 2: Set Up the Compiler and Project Paths
- **Include Directory:** Add the `include` folder from the extracted SFML directory to your project's include paths.
- **Library Directory:** Add the `lib` folder from the extracted SFML directory to your project's library paths.
- **Binary Directory:** Add the `bin` folder from the extracted SFML directory to your system's PATH (if necessary for runtime execution).

### Step 3: Configure Linkers
Add the following linker flags to your project settings:
-lsfml-graphics -lsfml-window -lsfml-audio -lsfml-system -lopengl32

### Step 4: Project Folder Structure
Ensure your project folder has the following structure:
ProjectFolder/ ├── bin/ # Executables ├── lib/ # Libraries ├── include/ # Header files └── src/ # Source code files

### Step 5: Write and Execute SFML Programs
1. Write your SFML programs in the `src/` directory.
2. Compile and link the project using the configured paths and linker flags.
3. Run the program from the `bin/` directory to ensure all dependencies are resolved.

---

## Notes
- **Execution Directory:** Ensure the SFML `.dll` files are accessible in the same directory as the program executable or included in the system PATH.
- **Dev-C++ Compatibility:** This guide is specific to Orwell Dev-C++ and SFML version 2.4.2 with GCC 4.9.2 TDM (SJLJ) - 64-bit.

---

## Resources
- **SFML Documentation:** [https://www.sfml-dev.org/documentation/2.4.2/](https://www.sfml-dev.org/documentation/2.4.2/)
- **Orwell Dev-C++ SourceForge:** [https://sourceforge.net/projects/orwelldevcpp/](https://sourceforge.net/projects/orwelldevcpp/)

---

## Contributing
If you encounter issues or have suggestions for improving this guide, feel free to open an issue or submit a pull request.

---

## License
This repository is licensed under the MIT License. See the `LICENSE` file for details.

