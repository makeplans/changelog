# MakePlans Changelog

2019-05-15

* Added domain, address, email, phone_number and currency attributes to be used in custom messages for account.

2019-05-02

* Service length (example: 45 mins.) is now shown along with title and price on the booking site.
* Forgot password function was case-sensitive resulting in some problems for users who had entered uppercase in their email. This is now fixed.
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