# 🛠️ uBlock Origin Installer for Chrome

This repository provides registry files to install and uninstall [uBlock Origin](https://github.com/gorhill/uBlock) for Chrome via the Windows Registry, removing the need to enable developer mode or manually load extension files.

This method will automatically download and update uBlock Origin directly from the [Chrome Web Store](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm), bypassing Google's recent restrictions on normal installation.

## 📁 Files Included

- **uBlock32.reg**: Installs uBlock Origin on 32-bit Windows systems.
- **uBlock64.reg**: Installs uBlock Origin on 64-bit Windows systems.
- **uBlockPolicy.reg**: Applies registry policy settings to force the installation of uBlock Origin. Ideal for system administrators or enterprise environments.
- **uBlockUninstall.reg**: Removes the registry entries, effectively uninstalling uBlock Origin.

## 📝 How to Use

1. **Select the Appropriate File**  
   - Use **uBlock32.reg** if you're on a 32-bit version of Windows.
   - Use **uBlock64.reg** if you're on a 64-bit version of Windows.
   - Use **uBlockPolicy.reg** to force the installation via enterprise policy settings.

2. **Applying the Registry File**  
   - Simply double-click the chosen `.reg` file.
   - The system will request administrator rights to apply the changes.
   - Confirm the registry changes when prompted.

3. **Verify the Installation**  
   Open Chrome's extension tab (`chrome://extensions`) and check that uBlock Origin is installed and enabled.

## 🔍 How It Works

This registry method installs uBlock Origin from the Chrome Web Store and ensures it stays updated. There's no need to enable developer mode or manually load the extension, as the files are automatically pulled from the store.

## ⚠️ Warning
 
 **The uninstaller (`uBlockUninstall.reg`) will remove all forced enterprise extensions** managed through the `ExtensionInstallForcelist` registry policy. If other extensions are installed via this method, they will also be uninstalled.
 
## 📜 License

This project is licensed under the [MIT License](LICENSE).
