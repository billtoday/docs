# bundle

a bundle is a plan that bundles an app with another app.

Say you have two apps (App-1 and App-2) running in production.

App-1 is an app that shows you stocks at different stock exchanges. It lets you purchase them using APIs of various brokers, so you do not need to use the multiple webapps.

App-2 is another app that creates stock performance reports. It highlights problems in areas where you could have done better by selling earlier or later. It also correlates this data with Twitter trends.

App-1 and App-3 make sense on their own, and you sell them each with their own plan. Since they require different levels of security (App-1 deals with money, App-2 just with data), you develop them in different repos.

But they also make sense as bundle. If both apps use the same bill.today instance for handling plan payments, you can simply tell bill.today the bundle criteria. None of the apps actually needs to know about the bundle pricing, since the apps just know wether the customer in question has purchased a valid plan or not.

