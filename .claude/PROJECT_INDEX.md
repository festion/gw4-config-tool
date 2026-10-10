# Project Index: festion__gw4-config-tool
## 1. Core Purpose
The `festion__gw4-config-tool` codebase appears to be a web-based configuration utility, likely for a gateway device (indicated by "gw4-config-tool" and files like `gw_console.htm`). It provides a user interface for managing device settings, network configurations (e.g., `wifi.htm`, `wifi.js`), and other advanced options (`advanced.htm`, `advanced.js`). The tool supports multiple languages (English and Chinese locales).

## 2. Architecture
The project is structured as a client-side web application, primarily built with HTML, CSS, and JavaScript. It utilizes jQuery for DOM manipulation and UI components, including jQuery UI and jQuery Tags Input. Pure.css is used for styling, complemented by custom CSS. Internationalization is supported through JSON locale files. The build process is managed by Gulp, indicated by `gulpfile.js`, suggesting tasks like asset compilation, minification, or concatenation. The application likely uses a main `index.html` with various `.htm` files serving as partials or different application views.

## 3. Key Files
*   `./.claude/PROJECT_INDEX.md`: Placeholder for AI-generated project index.
*   `./config.json`: Application configuration settings.
*   `./.github/workflows/main.yml`: GitHub Actions workflow for main branch.
*   `./.github/workflows/secret-scan.yml`: GitHub Actions workflow for secret scanning.
*   `./.gitleaks.toml`: Configuration file for Gitleaks, a secret detection tool.
*   `./gulpfile.js`: Gulp build automation script.
*   `./index.js`: Main JavaScript entry point or application logic.
*   `./js/advanced.js`: JavaScript for advanced configuration functionalities.
*   `./js/app.js`: Core application JavaScript logic.
*   `./js/compat.js`: JavaScript for compatibility layers or polyfills.
*   `./js/equipments.js`: JavaScript related to equipment management.
*   `./js/gw_console.js`: JavaScript for gateway console interactions.
*   `./js/jquery.js`: The jQuery library.
*   `./js/jquery-tagsinput/jquery.tagsinput.js`: JavaScript for tag input functionality.
*   `./js/jquery-ui/jquery-ui.min.js`: Minified jQuery UI library for UI widgets.
*   `./js/slip.min.js`: Minified JavaScript for touch-friendly list reordering.
*   `./js/timeout-signal.js`: JavaScript for handling timeouts or signals.
*   `./js/wifi.js`: JavaScript for Wi-Fi configuration.
*   `./js/zones.json`: JSON data likely related to geographical or network zones.
*   `./locale/en.json`: English language localization strings.
*   `./locale/zh.json`: Chinese language localization strings.
*   `./package.json`: Project metadata and npm dependencies.
*   `./package-lock.json`: Exact dependency versions for npm.
*   `./readme.md`: Project README documentation.

## 4. Dependencies
The project's dependencies are managed via `npm` and defined in `package.json` and `package-lock.json`. Key front-end libraries directly included in the `js/` directory are:
*   jQuery
*   jQuery UI
*   jQuery Tags Input
*   SLIP (touch-friendly list reordering)

Development dependencies, inferred from `gulpfile.js`, likely include Gulp and its associated plugins for build automation.

## 5. Common Tasks
*   **Install Dependencies:** `npm install`
*   **Build Project:** Run Gulp tasks defined in `gulpfile.js`, typically via `gulp <task_name>` (e.g., `gulp build`, `gulp dist`).
*   **Run Development Server:** Likely involves serving `index.html` and associated assets, potentially handled by a Gulp task or a simple static file server.
*   **Localization Updates:** Modify `locale/en.json` and `locale/zh.json` to update or add language strings.
