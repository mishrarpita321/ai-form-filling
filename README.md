# ai-form-filling

This repository contains the full implementation of ai form filling in a voice enabled application. It organizes three separate repositories as submodules to keep each module independent while enabling easy collaboration and sharing. The three modules are:

- **ai-form-field-extractor_npm**: An NPM package for extracting, validating and filling form data, handling speech recognisation and speech synthesis.
- **API_proxy**: A backend API proxy service acting as an intermediary layer.
- **Frontend**: A React-based frontend for the user interface.

Each module has its own dedicated repository with specific instructions provided in their respective `README.md` files.

## Repository Structure
```
thesis-prototype/
├── ai-form-field-extractor_npm/  # NPM package for form data extraction
├── API_proxy/                   # Backend API proxy
└── Frontend/                    # React-based frontend
```

## How to Clone the Repository
To clone this repository along with its submodules, follow the steps below:

### Step 1: Clone the Parent Repository
Run the following command to clone the parent repository:
```bash
git clone <parent-repo-url>
```

### Step 2: Initialize and Update Submodules
After cloning the parent repository, initialize and fetch all submodules using:
```bash
cd thesis-prototype
git submodule update --init --recursive
```
This command ensures that all submodules are downloaded and checked out to the correct commit.

### Step 3: Navigate to Submodules
Each submodule (i.e., `ai-form-field-extractor_npm`, `API_proxy`, and `Frontend`) contains its own `README.md` file with specific setup and usage instructions. Navigate into each submodule directory and refer to the documentation:

```bash
cd ai-form-field-extractor_npm
# Read the README for setup and usage

cd ../API_proxy
# Read the README for setup and usage

cd ../Frontend
# Read the README for setup and usage
```

## Updating Submodules
If there are updates to any of the submodules, you can update them using the following commands:
```bash
git submodule update --remote
```
This pulls the latest changes from the remote repositories of the submodules. Make sure to commit the updated submodule references in the parent repository:
```bash
git add <submodule-directory>
git commit -m "Update submodule references"
git push origin main
```

## Contributing
If you plan to contribute to this project, make sure to:
1. Follow the instructions in the submodule `README.md` files for setting up the environment.
2. Commit changes to the respective submodule repositories.
3. Update the parent repository with the latest submodule references.

## Contact
If you encounter any issues or have questions, feel free to reach out!