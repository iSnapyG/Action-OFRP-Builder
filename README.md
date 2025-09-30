
# OrangeFox Recovery Builder for Samsung Galaxy Tab S9 FE (gts9fewifi)

[![Build Status](https://github.com/iSnapyG/Action-OFRP-Builder/actions/workflows/Recovery%20Build.yml/badge.svg)](https://github.com/iSnapyG/Action-OFRP-Builder/actions/workflows/Recovery%20Build.yml)
[![License](https://img.shields.io/github/license/iSnapyG/Action-OFRP-Builder)](https://github.com/iSnapyG/Action-OFRP-Builder/blob/main/LICENSE)

This repository provides a fully automated GitHub Actions workflow to compile OrangeFox Recovery Project (OFRP) for the **Samsung Galaxy Tab S9 FE (Wi-Fi)**, codenamed `gts9fewifi`.

---

## Architecture

This workflow is designed as a generic, configurable build pipeline. It automatically performs the following steps on a remote server:

-   **Sets up a clean build environment** with all necessary dependencies.
-   **Syncs the latest OrangeFox source code** for the specified manifest branch.
-   **Clones the device-specific tree** for `gts9fewifi`.
-   **Compiles the recovery image** using the AOSP build system.
-   **Creates a GitHub Release** with the final recovery image for easy download.

## How to Use

This builder is configured to be run manually from the GitHub Actions tab.

1.  Navigate to the **[Actions]** tab of this repository.
2.  In the left sidebar, click on **"Recovery Build for gts9fe"**.
3.  Click the **"Run workflow"** dropdown button.
4.  The form will be pre-filled with the correct parameters for `gts9fewifi`. No changes are needed.
5.  Click the green **"Run workflow"** button to start the build.

## Output

When the build is complete (it may take 1-2 hours), the final `recovery.img` will **not** be in the "Artifacts" section. Instead, a new **Release** will be automatically created.

-   Find the output on the **[Releases page]** of this repository.

## Credits

* **OrangeFox Recovery Project Team** for their incredible work on the recovery.
* The original author of the generic build workflow.
