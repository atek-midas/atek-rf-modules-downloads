<p align="center">
  <h1 align="center">ATEK RF Modules UI</h1>
</p>

<p align="center">
  Pre-built desktop application packages for controlling supported ATEK MIDAS RF modules.
</p>

---

## Downloads

The latest Windows and Linux packages are available on the Releases page:

[Download the latest release](../../releases/latest)

Available packages:

- `ATEK_RF_MODULES_UI-v1.0.0-windows-x86_64.zip`
- `ATEK_RF_MODULES_UI-v1.0.0-linux-x86_64.zip`

---

## Windows Installation

1. Download the Windows ZIP package.
2. Extract the complete ZIP archive to a folder.
3. Open the extracted folder.
4. Run `ATEK_RF_MODULES_UI.exe`.

> Do not run the application directly from inside the ZIP archive.

> Keep the `_internal` folder in the same directory as `ATEK_RF_MODULES_UI.exe`.

The extracted package should contain:

```text
ATEK_RF_MODULES_UI-v1.0.0-windows-x86_64/
├── ATEK_RF_MODULES_UI.exe
└── _internal/
```

Do not delete, rename, or move the `_internal` folder. Do not distribute only the `.exe` file.

Windows SmartScreen may display a warning because the application is not digitally signed. Confirm that the package was downloaded from the official ATEK MIDAS GitHub repository before running it.

---

## Linux Installation

1. Download the Linux ZIP package.
2. Extract the complete ZIP archive.
3. Open a terminal inside the extracted directory.
4. Make the application executable:

```bash
chmod +x ATEK_RF_MODULES_UI
```

5. Start the application:

```bash
./ATEK_RF_MODULES_UI
```

The current user must have permission to access the serial device. On distributions that use the `dialout` group:

```bash
sudo usermod -aG dialout $USER
```

Log out and log back in after changing the group membership.

---

## Using the Application

1. Connect the ATEK RF module to the computer using USB.
2. Start the application.
3. Select the detected serial port.
4. Select `115200` baud.
5. Click **CONNECT**.
6. The connected RF module will be identified automatically.
7. The appropriate control panel will be loaded.

Use the refresh button if the serial port does not appear.

---

## Supported Modules

- ATEK256N3
- ATEK357P4
- ATEK366P5
- ATEK656N5 / ATEK1601
- ATEK888P5 / ATEK1801
- ATEK950P6

---

## Repository Purpose

This repository contains release packages and installation information only.

Application and firmware source code are maintained separately and are not distributed through this repository.

GitHub may automatically display `Source code (zip)` and `Source code (tar.gz)` files for each release. These archives contain only the public files stored in this release repository and do not contain the application or firmware source code.

---

## License

The downloadable software packages are distributed under the MIT License.

Copyright © 2026 ATEK MIDAS
