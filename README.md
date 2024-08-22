# Advanced Termux Setup Script
----

This repository contains a powerful shell script for setting up Termux with a comprehensive list of packages. The script performs multi-level package installation attempts, handles build dependencies, and provides professional feedback throughout the setup process.

## Features

- **Multi-Level Package Installation**: Attempts installation using `pkg`, `apt`, `apt-get`, and various Python package managers (`pip`, `pip3`, `python -m pip`).
- **Dependency Handling**: Checks for build dependencies and removes problematic packages if they fail to install.
- **Colorful and Informative Output**: Provides color-coded messages and animations to enhance readability and user experience.
- **OS Detection**: Automatically adapts installation commands based on the detected operating system (Android, Linux, Docker, macOS).

## Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/mdriyadkhan585/termux_setup
   cd termux_setup
   ```

2. **Make the Script Executable**

   ```bash
   chmod +x setup
   ```

3. **Run the Script**

   ```bash
   bash setup
   ```
4. **One Command**

   ```bash
   git clone https://github.com/mdriyadkhan585/termux_setup && cd termux_setup && chmod +x setup && ./setup
   ```
   
## Script Overview

- **`print_colored`**: Prints colored text to the terminal.
- **`show_animation`**: Displays a simple animation during package installation.
- **`is_package_installed`**: Checks if a package is already installed.
- **`remove_package`**: Uninstalls packages that fail to build due to dependencies.
- **`install_pkg`**: Handles installation attempts for each package.
- **`detect_os`**: Detects the operating system to tailor installation commands.
- **`progress_bar`**: Displays a progress bar during initial setup.

## Packages Included

The script includes a comprehensive list of packages for development, network tools, and system utilities. For a detailed list, refer to the `packages` array in the script.

## Error Handling

The script logs installation errors and build dependency issues to `termux_setup.log`. If a package fails to install due to missing dependencies, it will be removed, and the issue will be reported.

## Contribution

Feel free to open issues or submit pull requests if you have suggestions or improvements. Contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
