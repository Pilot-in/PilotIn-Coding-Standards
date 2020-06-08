# PilotIn-Coding-Standards
PHP Coding Standards of Pilot'in

## Installation steps

- Having `composer` installed:

[Get Composer](https://getcomposer.org/download/)
- Having `PHP Code Sniffer` installed:

`composer global require "squizlabs/php_codesniffer=*"`
- Having `WordPress Coding Standards` installed:

`composer global require dealerdirect/phpcodesniffer-composer-installer phpcompatibility/phpcompatibility-wp squizlabs/php_codesniffer wp-coding-standards/wpcs`
- Download this repo and put it somewhere on your drive.
- Get the current path config of **phpcs** using: 

`phpcs --config-show`
- Copy the paths after **"installed_paths:"**
- Paste it somewhere and **append the path of your folder** containing the **"PilotIn"** folder with a **comma**

- Give the new paths to **phpcs** using this command & change `your/paths/goes/here`:

`phpcs --config-set installed_paths your/paths/goes/here`
- Set the default standard as **PilotIn** using:

`phpcs --config-set default_standard PilotIn`
- Restart your terminal to be sure everything is up to date & try this command to see if everything is set:

`phpcs -i` 

*(You should have **"PilotIn"** showing)*
