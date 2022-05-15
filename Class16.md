# Class16 Reading Notes

### Reading
[What is Serverless Computing?](https://www.ibm.com/cloud/learn/serverless)

Serverless is a cloud computing execution model that 

Automatically provisions the computing resources required to run application code on demand, or in response to a specific event;
Automatically scales those resources up or down in response to increased or decreased demand;
Automatically scales resources to zero when the application stops running. 

This gives developers more time to develop and optimize their front-end application code and business logic. And with serverless, customers never pay for idle capacity. They pay only for the resources required to run their applications, and only when those applications are running.

The term **'serverless'** describes the customer's experience with those servers: they are invisible to the customer, who doesn't see them, manage them, or interact with them in any way.

### Serverless vs. FaaS (function as a service)
Serverless and **function as a service (FaaS)** are often conflated. But FaaS is actually a subset of serverless - it's the compute paradigm central to serverless, wherein application code or containers run only in response to events or requests. Serverless includes FaaS plus all the other associated resources and cloud services and resources supporting the code - e.g. storage, databases, networks, API gateways, authentication - for which configuration, management and billing of services are invisible to the user.

### PRO's
<ul>
<li>As noted above, serverless enables development teams to focus on writing code, not managing infrastructure.</li>
<li> serverless customers pay for execution only.</li>
<li>Serverless is a polyglot environment, enabling developers to code in any language or framework</li>
<li>serverless can be both faster and more cost-effective than other forms of compute</li>
<li>Serverless application development platforms provide near-total visibility into system and user times, and can aggregate that information systematically.</li>
</ul>

### CON's

<ul>
<li>t does not offer the same savings for workloads characterized by predictable, steady or long-running processes; in these cases a traditional server environment might be simpler and more cost-effective.</li>
<li>sometimes need to start up from zero to serve a new request</li>
<li>teams may find it difficult or impossible to monitor or debug serverless functions using existing tools or processes.</li>
<li>deeply integrating with the native managed services of a specific cloud platform is where much of the value of cloud can be found; for others, this cloud lead to material lock-in risks that need to be mitigated.</li>
</ul>

### Additional Resources
[venv - Creation of Virtual Environments](https://docs.python.org/3/library/venv.html)

[Vercel - Get Started](https://vercel.com/docs/get-started)

[http.server](https://pymotw.com/3/http.server/index.html)

[Requests](https://docs.python-requests.org/en/latest/)

[Python & APIs](https://realpython.com/python-api/)

### Videos
[What is Serverless?](https://www.youtube.com/watch?v=vxJobGtqKVM)

### Bookmark and Review
[Serverless Functions](https://vercel.com/docs/concepts/functions/serverless-functions)

[Effective Python Environment](https://realpython.com/effective-python-environment/)

----

## Things I want to know more about

----
[Home](https://github.com/MISalz/401_Reading_Notes/blob/main/README.md)