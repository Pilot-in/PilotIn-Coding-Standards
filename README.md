# PilotIn-Coding-Standards
PHP Coding Standards of Pilot'in

## Installation steps

- Having `composer` installed: [Get Composer](https://getcomposer.org/download/)
- Having `PHP Code Sniffer` installed:

`composer global require "squizlabs/php_codesniffer=*"`
- Having `WordPress Coding Standards` installed:

`composer global require dealerdirect/phpcodesniffer-composer-installer phpcompatibility/phpcompatibility-wp squizlabs/php_codesniffer wp-coding-standards/wpcs`
- Download the folder **PilotIn** of this repo and put it somewhere on your drive.
- Give the path of this folder to phpcs using:

`phpcs --config-set installed_paths path/of/your/folder`
- Set the default standard as **PilotIn** using:

`phpcs --config-set default_standard PilotIn`
- Restart your terminal to be sure everything is up to date & try this to see if everything is set:

`phpcs --config-show` 
