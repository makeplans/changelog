# MakePlans Changelog

2021-01-21

* Use of Stripe without our Stripe Connect integration is deprecated due to security concerns. We no longer store Stripe secret keys as a result of this change.
* You can now refund the paid amount for a booking using Stripe.

2021-01-15

* SMS reminders are now sent for last minute bookings.

2021-01-14

* Support for RTL-languages.
* Added Hebrew.
* Added RFC pagination HTTP headers.

2021-01-13

* Added Bahasa Malayu.

2021-01-07

* Added Spanish locale.
* Added Danish locale.

2020-12-02

* Check and require valid ISO 3166-1 alpha-2 country code for person.

2020-11-28

* Added ability to specify time between available slots instead of being just based on service length.

2020-11-18

* Added Polish language support on the booking site.

2020-11-09

* Added slot availability metadata in HTML data attributes on the booking site.

2020-10-29

* Service and event description page on the booking site.
* Added description (from service or event) to the Liquid booking info for use in outgoing messages.

2020-10-28

* Fixed bug: occupied appointment in calendar would not block availability when resource had capacity larger than 1.

2020-09-30

* Added invoiced_at as a field in the bookings CSV export.

2020-09-13

* Added event description to custom messages event object.
* Added event description to iCalendar description field.

2020-09-11

* Added title to booking.

2020-09-09

* Updated calendar with new look and performance improvements.

2020-08-20

* Added support to do refunds with Vipps-integration.

2020-06-17

* Added setting for hiding service from the booking site.

2020-06-14

* When creating new booking the resources connected to a service will be highlighted in the drop-down. It is still possible to select any resource but it is now easier to see the most relevant.
* Merging of two customers can now be done based on national id number. Previously it was only possible based on email and phone number.

2020-06-09

* Deleted customer will now be reactivated when trying to create a new customer with the same email or phone number.

2020-06-04

* Added setting to not include iCalendar attachment in booking emails.

2020-06-03

* App secret is generated and used for verifying payloads from MakePlans in webhooks. Available under account settings.

2020-05-27

* Added Zoom integration.

2020-05-24

* Automatic purge data. You can set a relative date for purging private data (customers and bookings).

2020-05-20

* Design template 'Warsaw' is now deprecated.
* Updates to a booking now triggers a new appointment URL in Confrere.

2020-05-18

* User permissions is now available. As an administrator you can set access roles for other users.

2020-05-06

* Added mail notification for a specific resource so you can be notified for new bookings for only resource (before all new bookings were sent to the account mail notification address).
* You can now add a custom order reference to the MakePlans invoice we generate for your account.

2020-05-03

* Payment Request API supported for Stripe payments. Customers can now pay with cards added to their browser.

2020-04-30

* Added security.txt for responsible disclosure.

2020-04-24

* 'Remember me' is now limited to 2 months. Before it would not expire.

2020-04-23

* Logged in sessions will be reset when password is changes. So you need to login again on other devices when you change your password.
* Now required to verify with password to disable two factor authentication.

2020-04-20

* Added Czech locale for the booking site.

2020-04-05

* Control whether email notification for a new booking is sent to admin in the administration system.

2020-04-04

* Added sender info setting for outgoing emails so you can specify a different sender than the account email.
* Added css body class indication for each specific page on the booking site.

2020-04-03

* Icalendar attachment is now included in the admin notification email.

2020-04-02

* Improved validation of date of birth for customer.
* Added phone number validation for customers added via administration system.
* Added validation for Norwegian fødselsnummer (social security number) on the booking site.

2020-03-16

* Added functionality to send SMS to all customers.

2020-03-10

* Added beta support for Vipps payments for Norwegian clients.
* Previously confirmation emails was not send when a booking was done without a service. Now a confirmation email is sent.

2020-02-26

* Custom data for all objects (booking, resource, service, category) is now shown on the info page for each object.

2020-02-17

* Fix validation bug where validation when a new customer was stored with local phone number and an existing customer had same phone number but already stored in full e.164 format. This caused errors such as 'invalid customer' when saving a new booking.

2020-02-15

* Autocomplete hints for passwords in forms.

2020-02-10

* Liquid output of event title now gives full title including service title. Title for the individual event is available using 'event.event_title'.
* Fix bug that did not convert date of birth to local date format when merging two customers.
* Cancelling booking at the payment step did previously not delete the booking but left it at a incomplete state (awaiting_payment) for it to be expired at a later time. This is now fixed and the booking is deleted immediately.

2020-02-07

* Total purchase price is shown when buying SMS in bulk.

2020-02-05

* Disable browser autocomplete for unique fields such as phone number and email.
* Fix double form submit bug when creating new customer via new booking page.

2020-02-03

* Fix availability bug when opening hours spanned over multiple days

2020-01-28

* Showing booking count in admin notification email.

2020-01-22

* Added booking count to custom form.

2019-12-11

* Added functionality for cancelling bookings for customer on booking site. Cancellation period rules can be set on the booking site settings.

2019-11-25

* Fix error with iCalendar attachment when booking is not booked with any service (booking made by administrator).

2019-11-07

* 'My page' on the booking site now supports email login as well.

2019-11-05

* 'My page' on the booking site. Customer can login using SMS code to see their bookings. This have resulted in an extra HTML `<section>` below the `<header`. If you are using a custom CSS it might affect how it is displayed.
* Search for people now supports partial phone number and email query (for example 'gmail.com' or '4848') instead of just exact match.

2019-11-01

* Added notes, created_by and updated_by to the booking export.

2019-10-30

* Fixed bug when cancelling a double booking. It would fail when being cancelled and had to be deleted. Now it can be cancelled. Cancel culture has officially reached MakePlans.

2019-10-28

* Fixed display bugs in service and category listing on the booking site. If you are using a custom CSS it might affect how it is displayed.
* Added footer for privacy policy and support links on the booking site.

2019-10-25

* Add iCalendar download when viewing booking on the booking site.

2019-10-14

* Anonymized IP for Google Analytics

2019-09-18

* Added booking cancelled web hook event

2019-09-16

* Added selected option for select input in Liquid forms

2019-09-13

* Fixed bug with 24SevenOffice integration that didn't update invalid bookings after invoice created in 24SevenOffice.

2019-09-12

* It is now possible to pause your account subscription.

2019-09-06

* Added chat widget for support.

2019-09-05

* All Stripe transactions now support PSD2 SCA.

2019-06-18

* Real-time response for 24SevenOffice integration progress.

2019-05-21

* Added SMS purchasing for volume discount.

2019-05-15

* Added domain, address, email, phone_number and currency attributes to be used in custom messages for account.

2019-05-02

* Service length (example: 45 mins.) is now shown along with title and price on the booking site.
* Forgot password function was case-sensitive resulting in some problems for users who had entered upper-case in their email. This is now fixed.
* The input for two factor authentication code is now focused when loading the page to save you a click.

2019-04-25

* Much faster generation of available times for accounts with many bookings.

2019-04-19

* iCalendar-attachment is now added to the cancellation email so any added appointment in external calendars will be updated with cancellation status.
* From address for all emails changed to bookingbot@makeplans.net. Due to increased verification at mail servers such as Gmail we will now not specify your account email as sender. The reply-to address is set as your account for all emails except verification. To use a custom from address please contact us. You will need to change your DNS records to be able to use a custom from address.

2019-04-18

* Link to open Stripe and Braintree transaction when a booking is paid with a card.

2019-04-16

* Added Apple touch icons for icon when adding to home screen.