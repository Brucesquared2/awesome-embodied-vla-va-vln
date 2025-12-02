# Using This Repository as a Git Submodule

This repository is designed to be used as a submodule in the MAPS-QUADCore project.

## Adding as a Submodule

To add this repository as a submodule to a parent repository (e.g., MAPS-QUADCore):

```bash
# Navigate to your parent repository
cd /path/to/MAPS-QUADCore

# Add this repository as a submodule
git submodule add https://github.com/Brucesquared2/awesome-embodied-vla-va-vln.git awesome-embodied-vla-va-vln

# Commit the changes
git commit -m "Add awesome-embodied-vla-va-vln as submodule"
```

## Cloning a Repository with This Submodule

If you're cloning a parent repository that includes this as a submodule:

```bash
# Clone with submodules
git clone --recursive https://github.com/USER/MAPS-QUADCore.git

# Or if you've already cloned without --recursive:
git submodule init
git submodule update
```

## Updating the Submodule

To update this submodule to the latest version:

```bash
# Navigate to the parent repository
cd /path/to/MAPS-QUADCore

# Update the submodule
git submodule update --remote awesome-embodied-vla-va-vln

# Commit the update
git add awesome-embodied-vla-va-vln
git commit -m "Update awesome-embodied-vla-va-vln submodule"
```

## Working with the Submodule

When working within the submodule directory:

```bash
# Navigate to the submodule
cd awesome-embodied-vla-va-vln

# You can make changes and commit them
git checkout main
git pull origin main

# Return to parent repository and commit the submodule reference update
cd ..
git add awesome-embodied-vla-va-vln
git commit -m "Update submodule reference"
```

## About This Repository

This repository contains a curated list of awesome embodied AI resources, including:
- Vision-Language-Action (VLA) models
- Vision-Language Navigation (VLN) models
- Vision-Action (VA) models
- Other MLLM-based embodied learning resources

For more information, see the [README.md](README.md).
