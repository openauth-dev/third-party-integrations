# List of third-party integrations

This repository is a public list of 3rd party integrations of the OpenAuth.dev
OAuth 2.0 provider (https://www.openauth.dev/developer) with other software.

The list is updated frequently and published on https://www.openauth.dev/developer.

## Adding your integration to the list

1. Fork this repository
2. Create a new file named `{platform}-{descriptive name}.yml`
3. Add your descriptions and links following the requirements below.
4. Create a pull request.

## Requirements

The file name must be formatted as **`{platform}-{descriptive name}.yml`** in
lower case. The `platform` corresponds to the `Platform` field in the file
itself. The `descriptive name` can be a short name of your work.

The file contains two parts:

1. Structured YAML "front-matter" with some metadata.
2. A short description of your solution.

### Example:

File `woltlab-suite-plugin.yml`:

```yml
---

Collection: Content management
Platform: WoltLab Suite
Type: Plugin
Developer: OpenAuth.dev
Developer_url: https://www.openauth.dev/developer
Price: Free
Url: https://github.com/openauth-dev/dev.openauth.wsc.login
Description: OpenAuth.dev login and registration for WoltLab Suite 3.0, 3.1 & 5.2.
```

### Fields required in front-matter

#### `Collection`

Main category of the integration which must be one of:

* `Content management` – for integrations with content management systems.
* `Desktop` – for desktop software with a GUI.
* `Development` – for command line tools, client libraries, integrations
  with programming languages or frameworks.
* `E-commerce` – for integrations with webshops and e-commerce platforms.

#### `Platform`

This is the name of the platform you created the solution for. Depending on
the `Collection` above this will be different. For example:

* For content management systems it will be the name of the CMS.
* For desktop software this is the name of the operating system.
* For development tools you can specify the programming language or framework.
* For e-commerce integrations this is the name of the e-commerce product.

#### `Type`

This describes the type of solution. You may follow the naming convention of
the platform that is being integrated with.

For example, add-ons for WordPress are officially called "plugins", so
the `Type` would be `Plugin`. For Magento integrations are officially
called an "extension", so the `type` would be `Extension`.

#### `Developer`

This is the full name of the software development agency or person that
authored and maintains this third-party solution.

#### `DeveloperUrl`

This is a link to the homepage of the developer. Preferably this would be a
location where users can **contact you** if they have any questions.

#### `Price`

This is either `Free` or the price in the main currency that you charge
users with, for example: `$ 19.00`.

#### `Url`

This is the location of the **download page** for your third-party add-on. It
should describe the solution and offer a way for the user to install or
download it in order to add it to their platform.

#### `Description`

The description should contain the **main features** of your integration. For
example, whether it supports resizing or preserving metadata, whether it
optimizes images in the background, etcetera.

You could also provide more information about how it integrates exactly with
the platform. For example, whether it optimizes images when they are uploaded
by a user to the CMS, or whether they are optimized when the pages are
published.

Please avoid describing what OpenAuth.dev is. Feel free to include this
information on your download page, though.

This description is preferably **between 80 and 160 characters** long.
