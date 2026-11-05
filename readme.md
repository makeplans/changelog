# MakePlans Changelog

2026-11-03

* Passes, subscriptions, gift cards and coupons are now tabs under Orders. Agenda queues are now tabs in the agenda.

2026-11-02

* Booking site settings are now split into separate pages: Design, Forms, General, Rules and Texts.

* If a booking is removed, expires or loses its slot while the customer pays in the Vipps app, the payment is now cancelled and the customer is not charged.

2026-11-01

* Added a terms page to the booking site, linked from the footer in all themes.

2026-10-30

* Booking CSV exports now include fields from the public booking form and service booking forms.

* Fix bug with the webhooks status indicator on the developer page.

2026-10-29

* Added daily workload: give services workload points and set a daily maximum per resource. The limit applies to bookings from the booking site, not bookings made in the administration system.

* Logos can now be uploaded in WEBP format.

2026-10-28

* Added two-way SMS: customers can reply to SMS when you use a phone number as sender, and you answer from the chat page.

2026-10-25

* Fix bug where validation errors were not shown when adding a customer from the booking or gift card form in the administration system.

2026-10-22

* Fix bug where customers paying for a confirmed booking with the order flow enabled were sent to the front page instead of the payment.

* Amsterdam theme: customers are now sent to Vipps or ID-porten login before the booking form when verification is required.

2026-10-19

* Prevent duplicate Vipps payment requests on double submit.

2026-10-11

* Added passes and subscriptions: sell them on the booking site, and customers pay for bookings with them at checkout. Customers see them on their profile. Subscriptions are used before passes.

2026-10-07

* Slots with no capacity on the booking site now show "Fully booked" or "Waitlist" instead of "0 available", and past slots show "Past". The texts can be customized in the booking site settings.

2026-09-25

* Improved the agenda list with day, week and month navigation, queues for waitlist and unconfirmed bookings, and feeds for latest changes and new reservations. Waitlisted bookings can be promoted or removed directly from the queue.

* Your profile and logout are now in a menu under your avatar in the header.

2026-09-23

* Added WhatsApp: connect your Meta business account, send messages using templates that are submitted to Meta automatically, and chat with customers.

* Fix crash on booking pages when the customer has been deleted.

2026-09-17

* Added booking ratings: include a rating link in a follow-up message and customers can rate the booking on a scale you choose, from 1-2 up to 1-10. Ratings are shown on the booking, in reports and in the API.

2026-09-15

* Zoom meetings and Whereby rooms are now removed when a booking is cancelled or deleted, so old join links stop working.

* Added an MCP page under Developer settings with your endpoint and setup instructions.

2026-09-13

* Added reports for utilization, no-shows, events and timing. Time-series reports can now be shown per day, week or month.

2026-09-12

* Added dark mode to the administration system, with a setting per user.

* Added availability, signup, login and purchase events for Google Tag Manager and Google Analytics on the booking site.

2026-09-10

* Custom text can now be added to the declined booking SMS.

2026-09-08

* Added week view to the Timisoara theme.

2026-09-04

* The event week calendar in the Timisoara theme now shows free capacity when enabled on the service, and the legend lists only bookable services.

2026-09-02

* Added a booking state filter to the agenda, so declined and cancelled bookings can be found. Also added `/bookings/declined` and `/bookings/cancelled` to the API.

2026-09-01

* Added reports: overview, bookings, revenue, resources, services and customers, with filters, comparison with the previous period, and CSV and JSON export.

2026-08-31

* Added customer history: visits, no-shows and total paid are shown on the booking, in the calendar and on the customer page. You can also get a warning when a customer reaches a set number of no-shows.

2026-08-26

* Added custom data for the account: define an account form under Setup and use the values in Liquid templates and the API.

2026-08-25

* Replaced Google reCAPTCHA with ALTCHA, which is self-hosted and sends no customer data to a third party.

2026-08-19

* The opening hours panel in the calendar can now be scoped to a service or resource.

2026-08-17

* Added week calendar for events in the Timisoara theme.

2026-08-16

* The booking confirmation now shows the client address as a Google Maps link.

* Added website to the account settings.

2026-08-15

* Added MCP server: connect AI assistants such as Claude to MakePlans to find available slots, create and manage bookings, and look up customers.

2026-08-14

* The booking form in the administration system now uses the custom booking form for the selected service.

2026-08-13

* The new event form now prefills capacity and booking limits from the service defaults, and suggests a booking window based on your previous events. For recurring events the booking window is adjusted per occurrence.

2026-08-12

* Added waitlist for events: customers can join a waitlist when an event is fully booked and get notified when a spot becomes available. Waitlisted attendees are shown on the event page.

2026-08-10

* Added Albanian locale.

2026-08-06

* Added Unloc integration: door keys are automatically issued to the customer when booking a resource with an Unloc lock, and revoked on cancellation.

2026-07-20

* Added German locale.

2026-07-18

* Added targeted SMS: send SMS to customers filtered by service, date and booking status. Messages support Liquid tags for personalization with a live preview.

2026-07-09

* Added Vipps payment requests.

2026-07-08

* Custom text can be added to payment request SMS and email.

* Fix bug where custom text for the awaiting confirmation SMS was ignored.

2026-07-03

* Upgraded the calendar with improved design and mobile support.

* Resource colors are now shown in the calendar filter dropdown.

2026-06-30

* Customers can now pay for confirmed or completed bookings themselves from the booking site.

2026-06-24

* Added refund support for orders.

2026-06-18

* Day booking now displays overnight stays and uses month view.

2026-06-15

* New phone number input with country selector on all phone fields.

2026-06-03

* Added dictation to booking and customer notes fields.

2026-05-11

* Customers must complete missing profile details before paying with Vipps or FrontGo.

2026-05-04

* Added setting on message templates to skip sending if the booking time has passed.

2026-04-30

* Existing customers can now be linked as children to another customer.

2026-04-12

* Support new 2032-format Norwegian national ID numbers.

2026-04-09

* Added settings for disabling the manual confirmation message. Email is now always sent unless disabled.

2026-03-28

* API: gift card output now includes person_id and purchased_by_person_id.

2026-03-25

* Added language switcher to the booking site.

2026-03-18

* Added Klaviyo integration.

* Added coupon support to checkout.

2026-03-14

* Customers can now edit their profile on the booking site.

2026-03-12

* Added FrontGo as payment provider for orders.

2026-02-21

* ID-porten and Vipps Login can now be used as verification methods in Norway.

2026-02-17

* Added tool for moving bookings between resources.

2026-02-09

* Removed integrations Dokus, iZettle and Fakturo. RIP.

2026-02-03

* Custom forms now support the person object in Liquid tags, and a new terms tag was added.

2026-01-31

* Norwegian national ID numbers are now validated, and date of birth is set automatically from the national ID number.

2026-01-23

* Users now receive an email notification when their email address is changed.

2026-01-21

* It is now possible to book on behalf of others, such as children, on the booking site.

2026-01-16

* Added standalone categories, works as standalone services which are only available via direct link.

2026-01-12

* Added gift cards and products: sell gift cards on the booking site with a cart and checkout flow. Payment with Stripe, Vipps or FrontGo. Gift cards can be redeemed at checkout and are listed on the customer profile.

2025-12-10

* Added room display: a public screen for a resource showing today's bookings, accessible with a token.

2025-11-20

* Added credit card management and customer details to profile pages on the booking site.

2025-11-07

* Added day booking: services can be booked per day, including multiple days.

* Added standalone services.

2025-10-16

* API: bookings now include booked_by_person_id.

2025-10-08

* Added message to customer when booking is awaiting confirmation (opt-in per account).

2025-10-06

* Number of available slots is shown per date on the booking site.

2025-10-05

* Added cancellation settings for services and events.

2025-10-01

* Services can now be ordered within categories.

2025-09-26

* Added Bento integration.

2025-09-24

* Added British English (en-GB) locale.

2025-09-14

* Added refund support for FrontGo.

2025-09-11

* Next available date is listed in the sidebar when creating a new booking.

* Fix bug that made it possible to set empty opening hours, leading to error on the booking site.

* Fix bug that blocked the resource for bookings without a service.

* Added duration display in the timepicker for end time when creating a new booking.

2025-09-08

* Added FrontGo as payment provider.

2025-08-29

* It is now possible for the customer to reschedule their appointment (within cancellation period).

2025-08-25

* Added functionality for adjusting opening hours per provider on a service.

2025-08-21

* Added option for priority strategy on a service. A provider was previously picked by random, new strategies include order and weight.

2025-08-13

* Ensure it is not possible to select disabled slots on the booking site when showing slots in the past.

2025-08-12

* The service setting for blocking resource will now only return slots that are fully available.
This makes it possible to for example have a sauna available for both private and drop-in booking, where the service for private booking will require the resource to be empty when booking a slot.

2025-07-31

* Fixed bug which led to drop-in bookings for more than 1 person were counted as 1 when returning available slots.

2025-07-08

* Added setting to ignore form requirements for existing customers.

2025-05-13

* Ability to show slots from the past to indicate when resource was unavailable.

2025-01-16

* It is now not possible to modify the service for appointments marked as 'busy' as this caused some confusion (it was not intented to have a service for non-customer appointments and it serves no purpose).

2024-11-13

* Fix bug for availability when using fixed slots and the current time was after the first opening hour for today.

2024-08-27

* Verification SMS is now sent using a low-cost provider from a fixed number instead of 'MakePlans'.

2024-08-14

* Integration Confrere is removed because it no longer exists.

2024-08-13

* Preview for custom forms/messages and natural language date input.

2024-08-06

* Added list view for design themes Lviv and Timisoara.

2024-07-15

* Released partner API.

2024-07-12

* Whereby Embedded integration.
* Add video_url for custom messages.

2024-04-15

* Add Italian locale for booking site.

2024-03-21

* New booking site template: Lviv (Slava Ukraini).

2024-03-16

* Event check in for attendees.

2024-03-07

* New booking site template: Timisoara.

2024-01-21

* Added coupon codes for discounts.

2024-01-13

* All changes and actions are now automatically logged and includes metadata for who and how performed the action.
* Added function to change time zone and automatically updated all booking times.

2023-12-28

* A deleted person can now be undeleted.

2023-12-19

* Fix issue with sorting events when printing the calendar.

2023-11-29

* We now require password of at least 8 characters (nist recommendation).

2023-11-21

* Added setting to disable including iCalendar attachment to avoid PII being sent via email.

2023-11-20

* Added custom text when sending mail notification to a user for modification and cancellation.

2023-11-15

* Recurring events now support RDATE/EXDATE iCalendar properties.

2023-11-06

* New default for busy bookings set to 1 hour duration. Previously there was no duration.

2023-09-18

* You can now add a custom reservation form pr service.

2023-08-27

* Added support for using your Plausible Analytics account on the booking site.

2023-07-11

* Updated Google Analytics to version 4 (GTAG) on the booking site. Note: we do not use GA, we offer it as an option to use your own GA account on the booking site.

2023-06-30

* We now allow JavaScript using a Liquid tag on the booking site.

2023-06-14

* CSP now requies iframe or xhr usage to be whitelisted with URL.

2023-06-10

* You can now send from your own email address by verifying your email domain.

2023-04-11

* Implemented Content Security Policy.

2023-02-22

* Added custom ical summary and description text using Liquid
* Added url for booking ical location

2023-02-18

* Send cancellation notification to booked resource.

2023-02-16

* Send modification notification to booked resource.

2023-02-08

* Fix performance issues of large CSV exports.
* CSV export files are now stored privately on AWS S3 instead of attached in the export email. The link to download the file is only accessible for 15 minutes after the export is generated.

2023-01-31

* Fix Stripe descriptor statement for accounts with long name which caused transactions to fail.

2022-12-28

* For easier creation of many resources you can now clone an existing resource. Please note that provided services are not included in the clone.

2022-12-27

* Add custom sender SMS id (paid addon).

2022-10-24

* Support for custom display of events in the calendar. Use Liquid to add the information you want for an event shown in the calendar.

* All third party newsletter subscriptions now require concent from the customer. Automatically added when using the standard booking form but for custom forms use {% raw %}{% opt_in_marketing %}{% endraw %}.

2022-09-23

* It is now possible to specify booking params in a link to the booking site. So from your website you can for example specify the name of the person booking and saved then used in the booking form.

2022-08-09

* Output JSON-LD Schema.org for events and services.

2022-07-28

* Whereby integration now can show Whereby meetings embedded in MakePlans.

2022-07-15

* Support for getting current locale in Liquid rendering

2022-07-11

* Localised CSV exports for date and time formatting. Previously it was ISO8601 it is now in local format to avoid Microsoft Excel parsing issues (please support international standards Microsoft).

2022-06-22

* Support language pr user on the booking site. Visitors can choose language and language is saved to the customer for next visit.

2022-06-12

* Automatic SSL certificates for your custom domain. Just point your DNS to us and we handle the rest.
* New option to restrict bookings on the booking site to only existing customers.

2022-05-24

* Option to automatically create order in 24SevenOffice. Previously this was a manual process.

2022-05-04

* Able to refund Stripe payment from booking page.

2022-05-03

* Option to show availability for each slot/event on the booking site.

2022-04-28

* Saving an object with custom data keys that is not present in the custom form will now be kept. Previously such values were discarded.

2022-04-20

* Option to save billing details to Stripe.

2022-04-16

* Customers are now automatically saved to Stripe. Optional setting to disable this behaviour.

2022-04-06

* A customer can now make a booking for other people, for example a parent can make bookings for their children.

2022-04-04

* Added support for multiple payment providers. When multiple payment providers is configured the customer can choose which payment provider to use.

2022-03-25

* The 24SevenOffice integration now supports price calculation for booking multiple slots.

2022-03-25

* You can now easily see and copy the secret in addition to scanning the QR code when activating 2FA.

2022-03-03

* Custom text to display to user when there is no availability on the booking site.

2021-12-25

* Added Whereby integration

2021-11-13

* Support for SMS notification phone number per resource

2021-11-04

* We are now makeplans.com
* robot@booking.makeplans.com is now used as mailer sender address.
* Stripe secret key is now no longer used, we only use OAuth token (Was not possible to use at the time we released the Stripe integration).

2021-11-04

* Booking notes are now showin the calendar preview

2021-09-05
* Show Zoom join url for event

2021-09-05
* Add support for individual Zoom links (paid plan required)

2021-08-05

* Emails are now sent to the customer after an event is changed or cancelled.
* Fixed bug so that SMS reminder time is changed when event time is changed.
* Web-hook event-delete is triggered.

2021-08-02

* Add custom text to display when the user is waiting for confirmation for a booking.

2021-07-05

* Added Notion integration.

2021-06-25

* It is now possible to save a card when paying for a booking using Stripe. The saved card can be reused for next booking. The customer can also add and remove stored cards on their profile.

2021-06-22

* Added Zoom host start url. The Zoom meeting can now be started by clicking 'Start Zoom meeting' on the booking.
* The event signup form count drop down is now reflected on real time availability. Previously it would give the customer option to select max number attendees but will now be limited to available spots on the event.
* We now send opt-out header for FLoC to Google
* Failed card charges for billing will now be notified to your account email as well as your billing email.

2021-05-28

* Email is sent to customer for recurring bookings with a list of all bookings.

2021-05-26

* Added exports for various booking states - all bookings, active bookings, including cancelled bookings.

2021-05-25

* SMS notification is now sent for booking approvement requests.

2021-05-22

* When changing password other sessions will be logged out.

2021-05-10

* All emails are now sent with sender on bookingbot.makeplans.net

2021-05-06

* Added BestRx integration

2021-04-08

* You will have to login after password reset to ensure 2FA is completed.

2021-04-04

* Added Russian localisation.
* Added Latvian localisation.

2021-03-23

* CSV export will now include custom fields for related objects.

2021-03-18

* No longer tracking users with Google Analytics.
* Email opening is no longer tracked (for example booking confirmation emails).

2021-03-02

* Added terms and conditions on the booking site. Can be shown in the booking form and make it required to accept before making a booking request.

2021-02-23

* Added French localisation.
* Added wildcard in webhook events.

2021-02-22

* Added more advanced messaging with message templates. You can now send multiple reminders and follow up messages after a booking.

2021-02-08

* Added support for Apple Pay when using Stripe.
* Added support for payment request API (stored cards in browser) when using Stripe.


2021-02-07

* You can now see which user that performed the action in the booking log.

2021-02-02

* XML support in the API is deprecated.

2021-01-28

* Added GUI for managing webhooks - no need to contact support for this.
* Possible to disable the API.

2021-01-26

* CSV-export now use regional delimiter.

2021-01-25

* Added Sendy integration.

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