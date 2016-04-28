# bundle

a bundle is a super plan that bundles two or more plans. A bundle can bundle super plans and app-specific plans.

## Example:
Say you have two apps (App-1 and App-2) running in production.

App-1 is an app that shows you stocks at different stock exchanges. It lets you purchase them using APIs of various brokers. This is much easier than using multiple applications for the individual brokers.

App-2 is another app that creates stock performance reports. It highlights problems in areas where you could have done better by selling earlier or later.

Both apps make sense on their own, and you sell them each with their own plan. Since they require different levels of security (App-1 deals with money, App-2 just with data) you develop them in two repos. This means each app has its own code base.

Still they also make sense together. If both apps use the same bill.today instance for handling plan payments, you can simply tell bill.today some bundle criteria. None of the apps actually needs to know about the bundle, since the apps just know wether the customer in question has purchased a valid plan or not.

