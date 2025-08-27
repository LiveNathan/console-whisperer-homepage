
# Project Overview

This project is a static website for "Console Whisperer". It's built using HTML, CSS, and JavaScript, with webpack as the build tool. The website provides download links for the Console Whisperer application for different operating systems (Windows, macOS, Linux) and architectures (Intel, ARM).

The main page (`index.html`) contains the layout and a script to detect the user's operating system and architecture, dynamically showing the most relevant download button.

# Building and Running

*   **Development:** To run the website in a development environment with live reloading, use the following command:

    ```bash
    npm start
    ```

*   **Production Build:** To create a production-ready build of the website in the `dist` directory, use the following command:

    ```bash
    npm run build
    ```

# Development Conventions

*   The main application logic is contained within `index.html`.
*   The entry point for webpack is `js/app.js`, which is currently empty.
*   Static assets like CSS, images, and vendor JavaScript files are located in the `css`, `img`, and `js/vendor` directories, respectively.
*   Webpack configuration is split into three files:
    *   `webpack.common.js`: Base configuration for both development and production.
    *   `webpack.config.dev.js`: Development-specific configuration, including `webpack-dev-server`.
    *   `webpack.config.prod.js`: Production-specific configuration, including `HtmlWebpackPlugin` and `CopyPlugin` for creating the final distributable files.
