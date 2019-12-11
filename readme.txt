Cloned from https://github.com/strangerstudios/pmpro-set-expiration-dates on 12/11/2019

=== Paid Memberships Pro - Set Expiration Dates Add On ===
Contributors: strangerstudios
Tags: paid memberships pro, pmpro, memberships, ecommerce, expiration
Requires at least: 3.5
Tested up to: 5.2.2
Stable tag: .4.4

Set a specific expiration date (e.g. 2013-12-31) for a PMPro membership level or discount code in YYYY-MM-DD format.
Enter "Y" for current year, "Y2" for next year. "M", "M2" for current/next month.
If the expiration date has already passed and "Y" is used, "Y" will start at the next year.

This expiration date will override any expiration period set on the level.

== Description ==
This plugin requires Paid Memberships Pro to function.

== Installation ==

1. Upload the `pmpro-set-expiration-date` directory to the `/wp-content/plugins/` directory of your site.
1. Activate the plugin through the 'Plugins' menu in WordPress.
1. Change the expiration date on the edit levels and edit discount code pages.

== Changelog ==

= .5.1 =
* BUG FIX: Fixed issue where expiration dates like 2019-07-29 would be converted to 2019-07-31 when used.

= .4.3 =
* BUG FIX: Added back the code to make sure dates like 2019-02-31 are converted to 2019-02-28

= .4.2 =
* BUG FIX: Fixed bug where some dates were not correctly pushed to next month.
* ENHANCEMENT: Added ability to pass a date to pmprosed_fixDate() to set expiration dates from instead of using current date.

= .4.1 =
* BUG FIX: Better handling of Y1 and M1. A date like Y1-12-31 no longer is pushed out to next year.
* ENHANCEMENT: Created a test file here (https://gist.github.com/ideadude/f94f4440ab109fe894a4a45bd9b64734) to make sure future updates don't break functionality for date formats.

= .4 =
* BUG FIX/ENHANCEMENT: Accepting Y1 and M1 in addition to Y and M in dates.

= .3.1 =
* BUG: Fixed warning if the $level passed into the pmpro_after_checkout hook was empty.

= .3 =
* BUG: Fixed bug when using PayPal Standard.
* BUG: Fixed bug with dates near the end of the month.

= .2 =
* Now showing Membership expires on {date} and checkout page when a set expiration date is set. (Thanks, Tania)
* Fixed bug when applying discount codes

= .1.1 =
* Fixed a warning.
* "Y" variable now starts from the next year if the expiration date has already passed.

= .1 =
* Initial commit.
