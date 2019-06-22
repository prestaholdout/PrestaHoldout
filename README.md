About PrestaHoldout
--------

The objective of this Prestashop 1.6 fork is to fix bugs, backport Thirty Bees and Prestashop 1.7 bugfixes and some non-backwards-compatibility-breaking Prestashop 1.7 improvements, update the baked-in dependencies, and add support for newer PHP versions, while preserving full module and theme interoperability by not modifying any API signature or expected function or method result.

The target audience is Prestashop 1.6 store maintainers who are holding out until the next major Prestashop version that provides a stable API, i.e. after the migration to Symfony is completed.


Current Status
--------

This fork is currently experimental, please don't use its code (especially in production!) until this notice is removed.


Versioning
--------

Since this is aimed at patching current PrestaShop 1.6 installations, the versioning must provide not only information about our custom code, but also about the minimum required version of Prestashop, and the Prestashop code version in our patches. The minimum required version of Prestashop will be the latest version that requires any upgrade SQL queries or PHP scripts (currently 1.6.1.17), and our patches will include any updates made by Prestashop since then, so you don't have to use the Autoupgrade module every time Prestashop releases an updated version.

Thus, releases will be versioned in the following way: PRESTAHOLDOUT_MAJOR_VERSION.PRESTASHOP_BASE_PATCH_VERSION.PRESTASHOP_LATEST_PATCH_VERSION.PRESTAHOLDOUT_MINOR_VERSION

For example, the 1.17.24.2 release will be from the 1.x branch of PrestaHoldout, will require at least Prestashop 1.6.1.17, and will include all Prestashop updates up to 1.6.1.24, as well as our updates for PrestaHoldout minor version 2. Major version 0 is reserved for "vanilla updates" that include only PrestaShop code, so by applying PrestaHoldout 0.17.24.x you will be only updating your store's files to match Prestashop 1.6.1.24, without any extra code and without having to run the autoupgrade module.


Releases
--------

The releases will be made as zip patch files that contain only those Core files that have been changed with respect to the minimum required PrestaShop version, so you can just unzip and upload in place of your store's current files (please back those up first). If you're running a Prestashop version previous to the minimum required one, you will need to use the Autoupgrade module first to update to at least the minimum, but preferably the latest 1.6 -- just don't upgrade to 1.7 by mistake!
