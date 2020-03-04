# MakePlans Changelog

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