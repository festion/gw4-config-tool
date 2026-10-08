# Project Index: gw4-config-tool
## 1. Core Purpose
The `gw4-config-tool` is a web-based configuration interface, likely for a gateway or similar device. It provides a user interface for managing device settings, network configurations, and other operational parameters through a set of HTML pages, JavaScript logic, and CSS styling.

## 2. Architecture
The project follows a client-side web application architecture, predominantly using static HTML pages (`html/*.htm`, `index.html`) rendered in a browser. JavaScript files (`js/*.js`) handle dynamic content, user interactions, and potentially API calls for configuration updates. jQuery and jQuery UI are utilized for DOM manipulation and enhanced UI components. CSS files (`css/*.css`) provide styling. Gulp (`gulpfile.js`) is used for task automation, suggesting a build process for minification, concatenation, or other asset processing. Localization is supported via `locale/en.json` and `locale/zh.json`.

## 3. Key Files
*   `config.json`: Likely contains application-wide configuration settings.
*   `gulpfile.js`: Defines automated tasks for building, development, or deployment.
*   `index.html`: The main entry point HTML file for the web application.
*   `index.js`: The primary JavaScript file, likely orchestrating the application's initial setup and routing.
*   `js/advanced.js`: JavaScript for advanced configuration functionalities.
*   `js/app.js`: Core application logic in JavaScript.
*   `js/compat.js`: JavaScript for compatibility layers or polyfills.
*   `js/equipments.js`: JavaScript related to equipment management or configuration.
*   `js/gw_console.js`: JavaScript for a gateway console interface.
*   `js/jquery.js`: The jQuery library for DOM manipulation.
*   `js/jquery-tagsinput/jquery.tagsinput.js`: jQuery plugin for tag input fields.
*   `js/jquery-ui/jquery-ui.min.js`: The jQuery UI library for advanced widgets and interactions.
*   `js/slip.min.js`: Likely a utility library, potentially for gesture-based interactions (Swipe, List In Place).
*   `js/timeout-signal.js`: JavaScript for handling timeouts or signals.
*   `js/wifi.js`: JavaScript for Wi-Fi configuration.
*   `js/zones.json`: JSON file likely containing data related to different zones or regions.
*   `locale/en.json`: English localization strings.
*   `locale/zh.json`: Chinese localization strings.
*   `package.json`: Defines project metadata, scripts, and Node.js dependencies.
*   `readme.md`: Project documentation.

## 4. Dependencies
*   **Node.js Dependencies**: Defined in `package.json` and `package-lock.json`, these typically include development tools (like Gulp and its plugins) and potentially server-side utilities if a local development server is used.
*   **Client-side Libraries**:
    *   jQuery (`js/jquery.js`)
    *   jQuery UI (`js/jquery-ui/jquery-ui.min.js`)
    *   jQuery Tags Input (`js/jquery-tagsinput/jquery.tagsinput.js`)
    *   Pure.css (`css/pure-min.css`)

## 5. Common Tasks
*   **Development Server**: Running a local web server to serve the static files during development.
*   **Building/Bundling**: Executing Gulp tasks (via `gulpfile.js`) to process assets (e.g., minify CSS/JS, concatenate files).
*   **Localization**: Adding or updating language strings in `locale/*.json` files.
*   **UI Development**: Modifying HTML, CSS, and JavaScript files to update the user interface and functionality.
*   **Configuration Updates**: Adjusting settings within `config.json`.
