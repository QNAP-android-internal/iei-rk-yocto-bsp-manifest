# IEI RK Yocto BSP Manifest

This repository contains the manifest file for the IEI RK Yocto BSP. The manifest file is used to fetch all the necessary layers and dependencies required to build the Yocto image for IEI RK boards.

## Repository Structure

- `iei-rk-yocto-bsp.xml`: The main manifest file that includes references to various Yocto layers and repositories.

## Manifest File

The `iei-rk-yocto-bsp.xml` file contains the following main components:

- **Default Sync Settings**: Defines the default sync-j value.
- **Remote Repositories**: Lists the remote repositories used in the manifest.
- **Projects**: Lists the projects (Yocto layers) included in the build.

## Usage

To use this manifest file, follow these steps:

1. Install the `repo` tool if you don't have it already:
    ```bash
    curl https://storage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
    chmod a+x ~/bin/repo
    ```

2. Initialize the repo with the manifest file:
    ```bash
    repo init -u https://github.com/QNAP-android-internal/iei-rk-yocto-bsp-manifest -m iei-rk-yocto-bsp.xml
    ```

3. Sync the repositories:
    ```bash
    repo sync
    ```
## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
