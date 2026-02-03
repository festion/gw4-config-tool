Done. I have analyzed the repository and generated the `PROJECT_INDEX.md` file in the `.claude/` directory.
 application for configuring and managing April Brother BLE (Bluetooth Low Energy) gateways. It allows users to scan for gateways on a local network, view their status, and configure settings such as Wi-Fi connectivity, MQTT brokers, and firmware updates.

## Directory Structure
- `css/`: Contains all stylesheets, including the PureCSS framework and custom styles.
- `html/`: Holds additional HTML partial views loaded into the main interface for specific tasks (e.g., Wi-Fi setup, advanced configuration).
- `js/`: Core client-side JavaScript logic.
  - `jquery-ui/`, `jquery-tagsinput/`: Third-party jQuery plugins.
  - `app.js`, `wifi.js`, `advanced.js`: Feature-specific logic for the renderer process.
- `locale/`: Internationalization files for different languages (en.json, zh.json).
- `images/`: Static image assets like logos.
- `.github/workflows/`: CI/CD pipeline definitions for automated builds.

## Key Files
- `index.js`: The main entry point for the Electron application (main process). It handles window creation and native OS interactions.
- `index.html`: The main HTML file that serves as the user interface (renderer process).
- `package.json`: Defines npm dependencies, metadata, and scripts for running, building, and packaging the application.
- `gulpfile.js`: Contains Gulp tasks for automating asset management, such as copying library files.
- `js/app.js`: Likely contains the primary application logic for the renderer process, handling UI events and gateway communication.
- `css/style.css`: The main custom stylesheet for the application's look and feel.

## Architecture Patterns
- **Electron Application:** The application follows a standard Electron architecture with a main process (`index.js`) managing the application lifecycle and renderer processes (HTML/CSS/JS) building the UI.
- **jQuery-based Frontend:** The UI is built with HTML and heavily relies on jQuery and jQuery-UI for DOM manipulation, event handling, and UI widgets.
- **Asynchronous Communication:** The application communicates with gateways over the network asynchronously. It also uses Electron's `ipcMain` and `ipcRenderer` for communication between the main and renderer processes.
- **Feature-based File Structure:** JavaScript logic is separated into files based on application features (e.g., `wifi.js`, `advanced.js`, `gw_console.js`).

## Entry Points
- To run the application in development mode, use the command `npm start`.
- The application starts by executing `electron .`, which loads `index.js`.
- `index.js` creates a `BrowserWindow` and loads `index.html` as the main user interface.

## Dependencies
- **Electron:** The core framework for building the cross-platform desktop application.
- **jQuery / jQuery-UI:** Used for DOM manipulation and building the user interface.
- **serialport:** Node.js package for accessing serial ports, likely used for initial device configuration via a direct cable connection.
- **i18next / jquery-i18next:** Libraries used for implementing internationalization (i18n).
- **electron-builder:** A tool to package and build a ready-for-distribution Electron app for different platforms.
- **Gulp:** A toolkit for automating build processes and managing asset pipelines.

## Common Tasks
- `npm install`: Installs all necessary dependencies.
- `npm start`: Runs the application in development mode.
- `npm run lib`: Executes the Gulp task to copy required library files into the `js/` and `css/` directories.
- `npm run dist:win` / `dist:osx` / `dist:deb`: Packages the application for Windows, macOS, or Debian-based Linux distributions, respectively.
