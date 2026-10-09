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
# Project Index: festion__gw4-config-tool
## 1. Core Purpose
The `festion__gw4-config-tool` project is a web-based configuration interface designed to manage settings for a GW4 (Gateway 4) device or system. It provides a user-friendly frontend for various configurations, including advanced settings, authentication, certificate management, Wi-Fi parameters, and console access.

## 2. Architecture
This project is structured as a client-side web application, built with a traditional HTML, CSS, and JavaScript stack. It heavily utilizes jQuery for DOM manipulation and event handling, along with jQuery UI for enriched user interface components. Specific UI elements are enhanced with `jquery-tagsinput`. Styling is managed through `style.css` and a minimal CSS framework (`pure-min.css`). The application supports internationalization via JSON files in the `locale` directory. Build and automation tasks, such as asset processing and minification, are handled by Gulp, as indicated by `gulpfile.js`.

## 3. Key Files
*   `config.json`: Stores application-wide configuration parameters.
*   `css/style.css`: Contains custom CSS rules for the application's visual design.
*   `gulpfile.js`: Defines automated build tasks and development workflows (e.g., linting, minification, concatenation).
*   `html/`: Directory containing various HTML partials or views for different sections of the configuration tool (e.g., `advanced.htm`, `app.htm`, `wifi.htm`).
*   `index.html`: The main entry point of the web application.
*   `index.js`: Likely the primary JavaScript file responsible for application initialization or routing.
*   `js/`: Directory containing core JavaScript logic and third-party libraries.
    *   `js/app.js`: Contains main application logic.
    *   `js/advanced.js`, `js/equipments.js`, `js/gw_console.js`, `js/wifi.js`: Modules for specific functional areas.
    *   `js/jquery.js`, `js/jquery-ui/jquery-ui.min.js`: Core jQuery and jQuery UI libraries.
    *   `js/jquery-tagsinput/jquery.tagsinput.js`: A plugin for creating tag input fields.
    *   `js/compat.js`: Possibly contains compatibility fixes or polyfills.
    *   `js/slip.min.js`: A utility for reordering lists with touch and mouse.
    *   `js/timeout-signal.js`: Manages timeouts for operations.
    *   `js/zones.json`: A data file, likely containing configuration or options related to geographical or network zones.
*   `locale/en.json`, `locale/zh.json`: JSON files providing localized strings for English and Chinese, respectively.
*   `package.json`: Manifest file listing project metadata, scripts, and npm dependencies.
*   `package-lock.json`: Records the exact dependency tree and versions.
*   `readme.md`: Provides general information, setup instructions, and usage details for the project.
*   `.github/workflows/main.yml`: GitHub Actions workflow for continuous integration, building, and deployment.
*   `.github/workflows/secret-scan.yml`: GitHub Actions workflow for scanning secrets using Gitleaks.
*   `.gitleaks.toml`: Configuration file for the Gitleaks secret detection tool.

## 4. Dependencies
The project relies on Node.js and npm for managing development and client-side dependencies. Key client-side JavaScript libraries include jQuery, jQuery UI, and `jquery-tagsinput`. Gulp and its associated plugins are used for task automation during development and deployment. Specific dependency versions are locked in `package-lock.json`.

## 5. Common Tasks
Common tasks for this codebase typically involve:
*   **Setup**: Running `npm install` to install all necessary project dependencies.
*   **Development**: Executing Gulp tasks (e.g., `gulp build`, `gulp watch`) to compile assets, run a local development server, or automate other development-related processes.
*   **Linting/Quality Checks**: Running commands (possibly defined in `package.json` scripts or Gulp tasks) to check code style and identify potential issues.
*   **Building**: Initiating a build process via Gulp to prepare static assets for deployment, which may include minification and concatenation.
*   **Version Control**: Committing changes, with security scanning for secrets enforced by `.gitleaks.toml` and potentially integrated into pre-commit hooks or CI.
*   **Continuous Integration**: Automated builds, tests, and secret scanning orchestrated by GitHub Actions workflows (`main.yml`, `secret-scan.yml`) on code pushes or pull requests.
