# Project Index: gw4-config-tool
## 1. Core Purpose
The `gw4-config-tool` appears to be a web-based configuration interface, likely for a device or system. It provides a user interface (HTML, CSS, JavaScript) to manage settings, display information, and interact with the underlying system. The presence of `wifi.js`, `advanced.js`, and `equipments.js` suggests configuration of networking, advanced settings, and possibly device management.

## 2. Architecture
The project follows a client-side web application architecture, heavily reliant on HTML for structure, CSS for styling (including `pure-min.css`), and JavaScript for dynamic behavior and logic. It utilizes jQuery for DOM manipulation and event handling, along with jQuery UI for enhanced UI components. Gulp (`gulpfile.js`) is used as a build automation tool, suggesting tasks like minification, concatenation, or asset processing. Localization files (`locale/en.json`, `locale/zh.json`) indicate support for multiple languages.

## 3. Key Files
*   **`config.json`**: Global configuration settings for the tool.
*   **`gulpfile.js`**: Gulp build script for automating tasks like asset compilation, minification, or deployment.
*   **`index.html`**: The main entry point HTML file for the web application.
*   **`index.js`**: Likely the main JavaScript file that initializes the application or handles global logic.
*   **`package.json`**: Defines project metadata and lists Node.js dependencies.
*   **`package-lock.json`**: Records the exact version tree of dependencies installed.
*   **`readme.md`**: Project documentation.
*   **`.github/workflows/main.yml`**: GitHub Actions workflow for continuous integration or deployment.
*   **`.github/workflows/secret-scan.yml`**: GitHub Actions workflow for scanning secrets.
*   **`.gitleaks.toml`**: Configuration for gitleaks, a tool to detect hardcoded secrets.
*   **`css/style.css`**: Custom styles for the application.
*   **`css/pure-min.css`**: Minified Pure.css framework for responsive layouts and UI components.
*   **`html/*.htm`**: Various HTML templates for different views or sections of the configuration tool (e.g., `app.htm`, `wifi.htm`, `advanced.htm`, `gw_console.htm`).
*   **`js/jquery.js`**: The jQuery library, providing a foundation for JavaScript interactions.
*   **`js/jquery-ui/jquery-ui.min.js`**: jQuery UI library for advanced widgets and interactions.
*   **`js/app.js`**: Core application logic and client-side routing or state management.
*   **`js/wifi.js`**: JavaScript logic specific to Wi-Fi configuration.
*   **`js/advanced.js`**: JavaScript logic for advanced settings.
*   **`js/equipments.js`**: JavaScript for managing or configuring equipment.
*   **`js/gw_console.js`**: JavaScript for a gateway console interface.
*   **`js/compat.js`**: JavaScript for compatibility fixes or polyfills.
*   **`js/slip.min.js`**: A minimal library for touch interactions, possibly for sortable lists or swipe gestures.
*   **`js/timeout-signal.js`**: Utility for handling timeouts with `AbortSignal`.
*   **`js/zones.json`**: JSON data file, possibly for timezone information or similar geographic data.
*   **`js/jquery-tagsinput/jquery.tagsinput.js`**: jQuery plugin for tag input fields.
*   **`locale/en.json`**: English localization strings.
*   **`locale/zh.json`**: Chinese localization strings.

## 4. Dependencies
The project relies on Node.js and npm for package management, as indicated by `package.json` and `package-lock.json`. Key client-side JavaScript dependencies include:
*   jQuery
*   jQuery UI
*   Pure.css (CSS framework)
*   `jquery-tagsinput` (jQuery plugin)
*   `slip.min.js` (for touch interactions)
Build-time dependencies managed by `gulpfile.js` likely include Gulp and various Gulp plugins.

## 5. Common Tasks
*   **Updating UI Components**: Modifying existing HTML templates (`.htm` files), adjusting CSS (`css/style.css`, `pure-min.css`), or enhancing JavaScript logic within `js/*.js` files (e.g., `app.js`, `wifi.js`).
*   **Adding New Configuration Options**: Extending `config.json`, adding new fields to HTML forms, and implementing corresponding JavaScript logic to handle input and display.
*   **Implementing New Features**: Creating new HTML views, adding corresponding JavaScript files, and integrating them into the existing application flow.
*   **Bug Fixing**: Debugging issues in JavaScript logic, correcting display errors in HTML/CSS, or resolving data handling problems.
*   **Localization**: Adding new language strings to `locale/*.json` files or modifying existing ones.
*   **Build Process Maintenance**: Updating Gulp tasks in `gulpfile.js` or managing Node.js dependencies in `package.json`.
*   **Dependency Bumps**: Updating versions of client-side libraries or Node.js packages as indicated by the worktree name `dep-bumps`.
