# PilotIn-Coding-Standards
PHP Coding Standards of Pilot'in

- [Good coding habits](https://gist.github.com/damien-pilot-in/157b0b3bd6f28832ed257d6ea1ab26bc)

## Installation steps

- Having `composer` installed:

[Get Composer](https://getcomposer.org/download/)
- Having `PHP Code Sniffer` installed:

`composer global require "squizlabs/php_codesniffer=*"`
- Having `WordPress Coding Standards` installed:

`composer global require dealerdirect/phpcodesniffer-composer-installer phpcompatibility/phpcompatibility-wp squizlabs/php_codesniffer wp-coding-standards/wpcs`
- **Clone this repo** somewhere on your drive *(or you can just download this repo and unzip it but it's not going to be synced / updated)*
- Get the current path config of **phpcs** using: 

`phpcs --config-show`
- Copy the paths after **"installed_paths:"**
- Paste it somewhere and **append the path of your folder** containing the **"PilotIn"** folder with a **comma**

*For reference, mine looks like this: `C:\composer\vendor/phpcompatibility/php-compatibility,C:\composer\vendor/phpcompatibility/phpcompatibility-paragonie,C:\composer\vendor/phpcompatibility/phpcompatibility-wp,C:\composer\vendor/wp-coding-standards/wpcs,C:\Users\Administrateur\Documents\PLUGINS DEV\PilotIn-Coding-Standards\PilotIn`*

*⚠️ If you have relative paths, replace them by *absolute* paths!*

- Give the new paths to **phpcs** using this command & change `your/paths/goes/here`:

`phpcs --config-set installed_paths your/paths/goes/here`

*Example: `phpcs --config-set installed_paths C:\composer\vendor/phpcompatibility/php-compatibility,C:\composer\vendor/phpcompatibility/phpcompatibility-paragonie,C:\composer\vendor/phpcompatibility/phpcompatibility-wp,C:\composer\vendor/wp-coding-standards/wpcs,C:\Users\Administrateur\Documents\PLUGINS DEV\PilotIn-Coding-Standards\PilotIn`*

- Set the default standard as **PilotIn** using:

`phpcs --config-set default_standard PilotIn`
- Restart your terminal to be sure everything is up to date & try this command to see if everything is set:

`phpcs -i` 

*(You should have **"PilotIn"** showing & you're good to go 🚀)*

## Bonus steps 

If you're using **VS Code**:

- Install `phpcs` & `phpcbf` extensions
- Add this to your vscode settings:
```jsonc
/** Validation PHP */
"php.validate.executablePath": "php.exe",
"php.validate.run": "onType",

/** Formatte le code selon les standards "PilotIn" */
"phpcs.standard": "PilotIn",
"phpcbf.standard": "PilotIn",
"phpcbf.debug": true,
"phpcbf.executablePath": "phpcbf.bat",
```
