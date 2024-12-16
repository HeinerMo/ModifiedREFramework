# Modified REFramework

A customized version of UiPath's **Robotic Enterprise Framework (REFramework)** that integrates the dispatcher process into the initialization stage. This version introduces Boolean flags to:

- **Enable/disable the dispatcher process**.
- **Activate test mode** for streamlined debugging.

This framework is designed to require minimal configuration, enabling developers to quickly begin work on new projects.

---

## Features

- **Integrated Dispatcher Process**: Simplifies workflows by combining the dispatcher within the initialization stage.
- **Configurable Boolean Flags**: Easily toggle dispatcher execution and test mode without modifying the core code.
- **Developer-Friendly Setup**: Preconfigured structure reduces manual setup time, letting you focus on development.
- **Exception Screenshot on Init**: Exception screenshots are capture in the initialization stage when a system exception is thrown. 

---

## Requirements

To use this framework, ensure the following are in place:

1. **Orchestrator Asset**: 
   - An asset named `Path_RPA_Folder` must exist in Orchestrator.
   - This asset should specify the directory path where:
     - The `config.xlsx` file is stored.
     - The `Screenshots` folder is located.
   - Recommended location: A shared drive or other easily accessible location to facilitate team collaboration.

2. **Config File**:
   - The `config.xlsx` file should include all necessary settings and constants for the project.

3. **UiPath Dependencies**:
   - Ensure all standard REFramework dependencies are installed in your project.

---

## Getting Started

1. Clone this repository to your local machine.
2. Ensure the required Orchestrator asset (`Path_RPA_Folder`) is configured and points to the correct directory.
3. Open the project in UiPath Studio and review the `config.xlsx` file for any project-specific changes.
4. Use the Boolean flags in the `Init` state to:
   - Enable/disable the dispatcher process.
   - Activate test mode for debugging.

