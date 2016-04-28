# Docs @ bill.today
docs for bill.today

## About bill.today
### What is bill.today?
bill.today allows your applications to focus on getting its job done, without having to worry about payment.  
All your app does is running a simple check for the appId against the bill.today server and you get back a json object that tells you only what you need to now:


bill.today server supports multiple apps at the same time. We recommend one bill.today instance per company.
If apps use a similar user identifier (like an email address), it is easy to setup plan bundles accross different apps.


### Payment providers
Supported payment providers are PayPal and Stripe.

## Docs Overview:
| Section | Description |
| --- | --- |
| [bts (bill.today server module)](docs/bts/index.md) | the bts package is the heart of the bill.today software stack. It manages payments, invoice creation and plan bundles |
| [billtoday (npm client module)](docs/billtoday/index.md) | the billtoday package gives your app easy payment superpowers. |
| [Legal](docs/legal/index.md) | Considerations for running the bill.today stack in production. |
