<p align="center"><a href="https://console.platform.sh/projects/create-project/?template=https://raw.githubusercontent.com/platformista/sobki/refs/heads/main/template-definition.yaml&utm_campaign=deploy_on_platform?utm_medium=button&utm_source=affiliate_links&utm_content=https://github.com/platformista/sobki/blob/main/template-definition.yaml" target="_blank" title="Deploy with Platform.sh"><img src="https://platform.sh/images/deploy/deploy-button-lg-blue.svg"></a></p>


# Sobki Profile Bootstrap - Platform.sh and Upsun Template

This repository provides a [Platform.sh](https://platform.sh) template for deploying the [Sobki Profile Bootstrap](https://www.drupal.org/project/sobki_profile_bootstrap) Drupal distribution, with full support also for [Upsun](https://upsun.com), the latest product by Platform.sh. The template includes all necessary configuration for deploying to both **Platform.sh** and **Upsun**, ensuring a seamless and scalable setup for either platform.

## Project Overview

**Sobki Profile Bootstrap** is a custom Drupal profile designed to accelerate the development of mobile-responsive websites by providing a default Bootstrap-powered theme and essential configurations out of the box. The Sobki profile combines a modern front-end framework with core Drupal functionality, offering an efficient starting point for developers.

Key features of Sobki Profile Bootstrap:

- **Bootstrap Integration**: The profile is built on top of the popular Bootstrap framework, ensuring responsive design and mobile-first layouts.
- **Pre-configured for Development**: Sobki comes with a ready-made setup that includes default content types, views, and blocks, which significantly reduce initial development time.
- **Flexible and Extendable**: The profile can easily be extended with custom themes, modules, and configurations to meet specific project needs.
- **Multilingual Support**: Sobki also includes default configurations for multilingual support, making it easy to create sites in multiple languages.

This template streamlines the deployment process for both **Platform.sh** and **Upsun**, allowing developers to focus on site development and customisation rather than infrastructure concerns.

## Features

- **Pre-configured for Platform.sh and Upsun**: Includes all necessary files to integrate and deploy the Sobki Profile Bootstrap on either Platform.sh or Upsun with minimal setup.
- **Scalable Architecture**: Supports multi-tier environments, including separate development, staging, and production branches.
- **Environment-specific Configuration**: Leverages both Platform.sh and Upsun’s capabilities for different environment configurations, allowing for seamless testing and deployment.
- **Integrated with Platform.sh and Upsun Services**: Preconfigured database and cache services (MySQL, Redis) for optimised performance on both platforms.

## Getting Started

### 1. Create a new Project on Platform.sh or Upsun

For Platform.sh:
Ensure you have the [Platform.sh CLI](https://docs.platform.sh/development/cli.html) installed and authenticated.

```bash
platform create
```

For Upsun:
Ensure you have the [Upsun CLI](https://docs.upsun.io/cli.html) installed and authenticated.

```bash
upsun create
```

### 2. Initialize the production environment with the template

For Platform.sh:

```bash
platform environment:init https://github.com/platformista/sobki
```

For Upsun:

```bash
upsun environment:init https://github.com/platformista/sobki
```

### 3. Access Your Application

Once deployed, you can access your Drupal installation via the generated URL provided by either Platform.sh or Upsun.

## Customization

Feel free to modify the `sobki_profile_bootstrap` profile to meet your specific needs. You can:

- Add additional modules to `composer.json`.
- Update configuration in the `config/sync` directory.
- Customise the `settings.platform.php` or `settings.upsun.php` files for further environment-specific tweaks.

## Services

The following services are included in this template by default:

- **MySQL**: Default database service for Drupal.
- **Redis**: For caching and performance optimisation.

Modify the `.platform/services.yaml` (Platform.sh) or `.upsun/config.yaml` (Upsun) file to adjust service specifications as necessary.

## Known Issues

Please refer to the [Sobki Profile Bootstrap issue queue](https://www.drupal.org/project/issues/sobki_profile_bootstrap) for known bugs or issues with the profile itself. For Platform.sh or Upsun-specific issues, review the respective documentation or contact their support:

- [Platform.sh documentation](https://docs.platform.sh/)
- [Upsun documentation](https://docs.upsun.com/)

## Contributing

Contributions to this template are welcome! Please open a pull request or submit an issue for any feature requests, bugs, or suggestions.

## License

This template is open-source and available under the [GPLv2](LICENSE.txt) license.
