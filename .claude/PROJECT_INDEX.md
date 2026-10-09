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
