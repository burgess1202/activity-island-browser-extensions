# Activity Island Browser Extensions

Browser extensions for the **Activity Island** widget on Seelen UI.

These extensions send browser download and observable upload progress to the local Activity Island service. Media playback, camera status, and microphone status do not require a browser extension.

## Downloads

Download the latest extension packages from the [Releases page](../../releases/latest).

Available packages:

- `activity-island-transfer-bridge-chrome.zip`
- `activity-island-transfer-bridge-firefox.xpi`

## Chrome Installation

Chrome uses an unpacked extension because this extension is not currently distributed through the Chrome Web Store.

1. Download `activity-island-transfer-bridge-chrome.zip` from the latest release.
2. Extract the ZIP file to a permanent folder, for example:

   ```text
   Documents\Activity Island Extension\Chrome
   ```

3. Open Chrome.
4. Enter the following address in the address bar:

   ```text
   chrome://extensions/
   ```

5. Enable **Developer mode** in the upper-right corner.
6. Select **Load unpacked**.
7. Select the extracted extension folder.
8. Open or restart Activity Island.
9. Confirm that Chrome is shown as **Extension connected**.

Do not delete or move the extracted folder after installation. Chrome needs that folder to load the extension.

### Updating Chrome

1. Download the latest Chrome ZIP.
2. Extract it and replace the files in the existing extension folder.
3. Open `chrome://extensions/`.
4. Find **Activity Island Transfer Bridge**.
5. Select the reload button.

## Firefox and Zen Installation

Firefox-compatible browsers require a Mozilla-signed XPI for permanent installation.

Only install `activity-island-transfer-bridge-firefox.xpi` when the release notes indicate that the file has been signed by Mozilla.

1. Download the signed Firefox XPI from the latest release.
2. Open Firefox or Zen Browser.
3. Open **Add-ons and themes**.
4. Select the settings button with the gear icon.
5. Select **Install Add-on From File**.
6. Select the downloaded XPI file.
7. Confirm the requested permissions.
8. Open or restart Activity Island.
9. Confirm that Firefox is shown as **Extension connected**.

If Firefox reports that the extension is unverified or cannot be installed, the downloaded XPI has not been signed by Mozilla.

## Updating Firefox

Download and install the latest signed XPI from the Releases page. Firefox will replace the existing version when the new package uses the same extension ID and a higher version number.

## Removing the Extension

### Chrome

1. Open `chrome://extensions/`.
2. Find **Activity Island Transfer Bridge**.
3. Select **Remove**.
4. You may then delete the extracted extension folder.

### Firefox or Zen

1. Open **Add-ons and themes**.
2. Find **Activity Island Transfer Bridge**.
3. Open its menu and select **Remove**.

## Privacy

The extension communicates only with the Activity Island service running locally on your computer.

It is used to provide:

- Browser download progress
- Observable file upload progress
- Actions that return to the related browser tab
- Access to the downloaded file in File Explorer

The extension does not send browsing activity, file contents, or transfer information to an external server.

## Troubleshooting

### Activity Island shows “Extension unavailable”

Check the following:

- Activity Island and its local service are running.
- The extension is enabled in the browser.
- The browser was restarted after installation.
- The Chrome extension folder has not been moved or deleted.
- A signed XPI was used for Firefox or Zen.

### Chrome removed or disabled the extension

Open `chrome://extensions/` and load the extracted folder again using **Load unpacked**.

### Firefox refuses to install the XPI

The XPI probably has not been signed by Mozilla. Download a release explicitly marked as signed, or wait for the extension to become available through Mozilla Add-ons.

## License

This project is available under the [MIT License](LICENSE).
