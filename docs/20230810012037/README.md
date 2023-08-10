# 20230810012037
# X-ray of X-as-a-Service

Infrastructure Stack
#===================#
| Application       |
| Data              |
| Runtime           |
| Container         |
| OS                |
| Virtualization    |
| Server            |
| Infrastracture    |
| Facilities        |
#===================#

The stack above consists all the elements of running both
hardware and software, end to end. As you go top-to-bottom,
depending on the service model, each element represents
a part either you or a vendor manages.

* On-prem servers are basically full self-service, 
	you take all the responsibility.

* Data center hosted services deal with facilites,
	so you do not have to worry about ISP, power,
	physical security, personnel and such.

* Infrastructure as a Service takes care up until virtualization part.
	You consume at OS level. e.g. AWS EC2, DO Droplet

* Platform as a Service provides runtime services. Mostly preferred
	for/by developers to run apps without too much hassle.
	e.g. Vercel, Heroku

* Software as a Service, as the name implies, provides full service.
	As an end user, you do not have to worry about anything rather
	than using software itself. e.g. Office365, gDrive, etc.
