# Codespaces LAMP

![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/danielcregg/codespaces-lamp?style=flat-square)

A ready-to-use **LAMP stack** (Linux, Apache, MySQL, PHP) development environment powered by GitHub Codespaces. Fork this repository, open it in Codespaces, and start building PHP web applications instantly -- no local setup required.

## Features

- **Ubuntu 22.04** base image with Apache, MySQL, and PHP pre-installed
- Pre-configured **Dev Container** with automatic service startup
- PHP extensions included: `mysql`, `curl`, `gd`, `intl`, `mbstring`, `soap`, `xml`, `xmlrpc`, `zip`
- VS Code extensions for PHP IntelliSense, Xdebug, Git Graph, and Docker
- Sample landing page displaying PHP environment information

## Prerequisites

- A [GitHub](https://github.com) account
- Access to [GitHub Codespaces](https://github.com/features/codespaces)

## Getting Started

1. **Fork** this repository to your own GitHub account.
2. Click the green **Code** button and select **Open with Codespaces**.
3. Create a new Codespace. The Dev Container will automatically:
   - Build the LAMP stack Docker image
   - Start Apache and MySQL services
   - Forward ports **80** (HTTP) and **3306** (MySQL)
4. Once the Codespace is ready, open the **Ports** tab and click the forwarded port **80** to view the sample page.

## Usage

- Edit or add PHP files in the `public/` directory. Apache serves content from this folder.
- Access MySQL via the terminal using `mysql -u root`.
- The sample page at `public/index.php` displays your PHP version, server software, and document root.

## Project Structure

```
codespaces-lamp/
├── .devcontainer/
│   ├── Dockerfile          # Ubuntu 22.04 + Apache + MySQL + PHP
│   └── devcontainer.json   # Codespaces / Dev Container configuration
├── public/
│   └── index.php           # Sample landing page
├── LICENSE
└── README.md
```

## License

This project is licensed under the [MIT License](LICENSE).
