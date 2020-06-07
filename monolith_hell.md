## Monolith is hell but microservice isn't heaven
#### 8 June 2020

Monolith is past and microservices are the future. There are so many articles proving this single point. 
And I do agree that monolith is hell. If it isn’t now then maybe in the future and yes shifting to microservices paradigm will solve many problems.
Adopting microservices will help you build reliable, scalable, and easily maintainable systems. But make no mistakes that it isn't without any cost.
Shifting from building a monolith to multiple microservices should be based on technical requirements rather than being a trend follower. 

But first let's understand, how monolith becomes hell. Monolith is the single representation of all your business capabilities. 
Monolith systems generally start with a POC of an idea. For example, suppose we need to develop business capability A. 
As a POC we developed a system that delivers the business requirement. Now as the business grows, requirements grow too. 
Now there is a requirement of business capability B which is dependent on A. 
Since we already have a working model of A we introduce another component into the existing, thus giving birth to the monolith hell. 
With the integration of B within A, the following things will happen: 

1. Individual components are now highly coupled.
2. Each component now shares its resources with others because they are part of the same system. 
3. With the increasing capabilities, it will be hard to manage the system because changing one might result in breaking the other.

And then comes the microservices, "The Saviour” (at least based on recent trends).
Microservices is a distributed representation of business capabilities. Each individual capabilities are built as an independent service. 
Microservice forces you to define boundaries of your system via API that can’t be violated. 
So for the above example, there will be two services for each capability i.e. A and B and they both will communicate via some lightweight protocol like REST or gRPC. 
But implementing a microservice architecture will add the following complexities to your system:

1. Dependency Hell: In a microservice architecture, many independent services work in tandem to run business. This introduces a complex dependency model hence increasing multiple points of failure.
2. All complexities of a distributed system, from stable IPC to the operational complexity will get introduced in your system. 
3. Breaking a monolith is always a challenge. If not done right, it will cause more harm in the future if compared to the monolith.

So the real question will always be when to start breaking up from monolith hell? 
Many advocates of microservice architecture emphasized that adding the complexity of microservices should be well thought. 
Because in many cases (almost all initially) following a few monolith principles like well-defined structures with well-defined boundaries can save you from many troubles. 
The added complexity of microservices will impact every aspect of your development cycle i.e. from the design phase till the deployment phase. 
Maintaining a well-coordinated microservices will bring another challenge because of multiple points of failure.

In software architecture, there is no silver bullet. And hence neither does the microservices.
In my opinion, technical requirements along with the business expectations should play a role in deciding between monolith and microservice. 
Microservice will enable parallel development within an organization but if implemented wrong it will introduce all distributed complexity with no added benefit into your system.
