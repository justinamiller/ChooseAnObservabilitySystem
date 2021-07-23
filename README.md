# How to Choose an Observability System: Build-vs-Buy


If you run an app on the Internet, you know that availability is key to keeping your users happy and your business performing well. In order to measure availability and performance, modern organizations are turning to Observability as an evolution of traditional monitoring practices. In doing so, there’s a lot to think about:

* Which components do you need to make sure you have complete visibility?
* How do you make sure your system doesn’t miss anything?
* Can we afford to do this?
* Is this even something we have time to do?
* Who makes sure the system is up and reliable?

In this article, I’ll address these questions and help you make the right decisions to get your application observable and reliable quickly. We’ll also discuss the differences between purchasing a solution and rolling your own. While I obviously have a vested interest in you buying a product, there are plenty of circumstances where it makes sense to adopt your own, which I’ll discuss in this article also.

## Which components do you need?
Setting up an observability system has many benefits – visibility into your application, how it impacts your users, faster performance and reduced MTTR, to name a few – but to maximize these benefits you have to make sure that your solution covers the whole world of observability.

These are the components needed to fully realize the benefits of Observability: Infrastructure Monitoring lets you determine the performance and health of the actual infrastructure your app is running on. Application Performance Monitoring monitors your application and its dependencies, making sure that you can see when issues occur and isolate them to particular parts of the stack. Digital Experience Monitoring gives you insight into real user experience and lets you exercise functionality of your application through synthetic testing from around the globe. A log investigation product helps move from “what’s wrong” to “why is it wrong” by enabling quick analysis of and getting insight from application logs. On-call is a necessary component of any system that routes issues to the right team and gives them tools to fix them fast.

Not using all of these components only gives you a partial picture into the life of your application. Finding and integrating these components on your own can be a big chore, and making sure that everything provides a seamless view and lets you share integrated answers with the rest of your team is also crucial. Expecting your team to learn multiple user interfaces and to remember all of their nuances during troubleshooting isn’t realistic.

## How do you make sure you see everything?
These types of tools are complex and require a huge effort to implement. This graphic shows just some of the components of an observability stack:
![observe-landscape](https://user-images.githubusercontent.com/22912437/126797483-fc222750-0eb9-4cb7-b511-a83a6a85aceb.png)


All of these components need to be built, operated, and scaled to keep up with your business. Not getting all of your data into your observability platform can cause you to miss events and never get the clear picture of your application. Missing data defeats the entire point of building an observability service. If you attempt to sample data, it isn’t a matter of if you miss out on something critical, it’s a matter of when. When buying or building such an observability system, you need to make sure it ingests and retains all the data. Further, if you decide to build, you need to take into account that writing, operating, and integrating collectors, data pipelines, storage systems, visualization products, and more is a lot of effort, and that it takes time to make sure that what you implement really offers value to your internal users and helps your application perform better.

## Can we afford this?
One issue that comes up when considering purchasing a product, of course, is the cost of the product. Complex licensing models can lead to unexpected bills, and the siren song of ‘free’ solutions can certainly be appealing. However, it’s important to consider all the costs of any solution, including ones you might adapt from open source or build yourself.

With a homegrown solution, there may be no licensing fee to worry about, but along with considering infrastructure costs, ingress/egress costs and opportunity costs, it is necessary to consider engineering costs and self-maintenance costs. While skilled software engineers can easily implement the basic functionality of an observability system, it’s very important to consider the difficulty in hiring and retaining them, and to consider if having them reimplement a commercially-available product, that isn’t related to your core business, is really the best use of these rare resources. Make sure you take the life-time value and effort of all these costs into account when comparing it to a commercially available solution.

## Is this something we have time for?
In addition to the opportunity costs of having software engineers not working on your most important product, implementing your own system will take time, leaving you blind until your solution is implemented. Finding, evaluating, installing, configuring and tuning all of the disparate components that make up an effective observability system takes a lot of work. The time you spend trying to search for open-source versions of all of the components of a commercial product is far longer than the time it takes to start a trial and integrate data sources into a commercial product.

Further, if you’re experiencing downtime or other issues, you don’t have the luxury of waiting. Your customers aren’t going to sit around while your site performs poorly or generates errors – they’ll be going to a competitor instead.

## Who watches the watchers?
Another advantage of using a cloud-hosted platform rather than building your own is that someone else becomes responsible for ensuring uptime and reliability of your observability system. Observability provides myriad benefits, but also does introduce a single place where you have to go to be informed about your business. If that tool isn’t accessible, you’re flying blind again, and that creates serious problems. If you adopt a self-hosted solution, you have to consider how you’ll make sure the system stays accessible (and where you'll get the resources required to do this,) no matter what.

## Summary
There are advantages and disadvantages to self-hosting an observability system. Advantages primarily include flexibility and licensing costs, where disadvantages include tool sprawl, opportunity costs, and difficulty scaling. Adopting a commercial product does require the product suit your needs and has licensing costs, but does free your engineers to work on your core business, offers an integrated tool for all the observability components, and makes reliability of your observability infrastructure someone else’s problem. 
