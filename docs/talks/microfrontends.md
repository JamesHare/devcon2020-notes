# Think Big, Develop Small: Microfrontends

Microservices - An architectural strategy. Distributed. Loosely coupled.

Who uses them? Spotify, Netflix, Ikea, Hellofresh, etc.

"Software architecture is those decisions whichh are both important and hard to change." - Martin Fowler.

Monolithic vs Microservices. Components of the system are broken out and compartmentalized.

Benefits:

* Fault isolation.
* Eliminate vendor or tech lock in.
* Smaller and faster deployments. - You don't have to deploy everything all at once. Upgrade small portions of it at a time.
* Scalability
* Independent Release Cadence
* Choice of programming language

Challenges:

* Comminication complexity and security
* Big money. Investment into hardware and hardware design.
* Debugging can be difficult. Which component do we debug?
* Possible performance issues
* API versioning

So what if the UI had the exact same concept as the backend microservices?

What exactly is a microfront end?
Microservices within the client. Modular components (Apps are a composition of components).

Challenges:

* All components in one app server
* Have to align releases
* slow feature roll out in differetn components
* API calls go thorugh one server
* App service must argragate all services.

Further reading: https://martinfowler.com/articles/micro-frontends.html