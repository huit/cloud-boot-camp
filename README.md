Cloud Boot Camp
===============

*Cloud Boot Camp* is a series of training, exercises, and 
projects for HUIT to bring a team of admins and engineers up to speed and ready to
support a large, highly visible online Harvard application.  
This repository holds the centralized documentation, planning, and coordination for
Cloud Boot Camp.

Most of the content for this repository will be captured in the wiki. It will also serve
as an "index" to other repos -- the digital artifacts of this project-based training -- that
will be captured here in th HUIT GitHub org. By capturing this in a central place, it'll be not 
only straightforward to support the platform, but will bootstrap other support efforts and resources
in the future.

# Purpose

Our goals with this initiative and set of exercises are:

* Develop an ability within HUIT to support a set of high-profile sites in AWS by July 26
* Create a cross-discpline team that can handle support concerns at varying levels in the "stack," and of varying complexity
* Engineer supporting services and refine current technology to reduce to a minimum the hands-on support needed for production sites
* Develop a model for supporting production sites in the cloud that will inform ongoing planning around CLoud & Devops in HUIT

Not only do we want to "catch up," at the end we want to lead the way!

# Background Information

This effort represents not only the support of a new platform, but also a new approach to IT. So to properly support 
the platform, you will need to change gears in the way you approach systems and software. 

Many think of the cloud as a new type of service born of the need to reduce power for storage and servers, and to reduce cost. While that plays into it, the primary reason that cloud was developed is to enable automation & agility at the infrastructure level, the sort of things that a DevOps approach looks for. In fact, it more useful to think of cloud as the logical outcome to the pressures applied by DevOps. I.e. *Cloud is a set of technologies that are built to implement DevOps Processes.* 

Given that, the natural way to use the cloud – and to support apps in the cloud – is with DevOps approaches and toolsets. 

So ... time to switch gears.

## Tools

Here is a list of tools you'll want to install and have available as we move forward. (This is not exhaustive, and perhaps not even suffucient. Feel free to contribute). Most of these work better on Mac or Linux, since over the past few years they have become the prefered OS's for devops engineering.

### Basic Tools

* [Homebrew for Mac: Linux/Unix tools](http://brew.sh)
* From [Git](http://gitscm.org) or using `brew install git`
* SSH
* [Python](http://python.org) This is the runtime that the AWS tools are written in
 
On the Mac, Homebrew let's this installation happen quickly & easily. After installing homebrew, make sure that `/usr/local/bin` is the first in your path, then `brew install ...` the rest. Takes 3-5 minutes.

### DevOps Tooling

* [Vagrant](http://vagrantup.com/) ... get the latest (>= v1.6)
* [Virtual Box](https://www.virtualbox.org)

### AWS Tools

* [AWS commandline tools](http://aws.amazon.com/cli/) These are best installed from the command-line using `pip install awscli`
* [Elastic Wolf](https://aws.amazon.com/developertools/9313598265692691) GUI for visibility into your AWS resources.

### Collaboration Tools

* [HipChat](http://chat.huit.harvard.edu) We'll use this for communciation and tracking changes to code and builds in real time.
* Mailing List: TBD


### Extras

If you want to hang with the cool kids, take a look at these tools as well:

* [MOSH](http://mosh.mit.edu) The MObile SHell, let's you reconnect to SSH sessions without interruption. Use (brew to install)
* [SublimeText](http://www.sublimetext.com)
* [Docker](http://docker.io) The next big thing in app deployment (built-in with Vagrant >= v1.6).

 
# Project Exercises

Each of these projects are intended to mimic or augment the application, release tooling, or supporting technology around the application (such as logging. monitoring, instrumentation, and resiliency testing). We break each aspect into self-contained components, define a useful exercise -- simplified in complexity but still transferable to the real world -- around each area. We'll then break into teams and implement.

The artifacts of this work -- all code, data, etc. -- will be captured into git repos within the GitHub org, along with accompanying documentation. 

### The Exercises

- [Deploying a Fault Tolerant LAMP-based Service](/wiki/Deploying-a-Fault-Tolerant-LAMP-based-Service)
- [Downtime-Free Database Upgrades in AWS](wiki/Downtime-Free-Database-Upgrades-in-AWS)
- [[Front a website with CloudFront CDN]]
- [[Automated Continuous Integration: From GitHub Commit to Running Test Service]]
- [[Building a Control Plane for a Dynamic Site]]
- [[Comprehensive Monitoring, Instrumentation and Logging for a Dynamic Site]]


# Resources

### AWS

* [Intro to Amazon EC2 and VPCs](http://prezi.com/fe-v0v8rsldc/intro-to-amazon-ec2-with-simple-vpcs/)
* [Amazon Console](http://console.aws.amazon.com)


### Deployment

* [Nepho](http://github.com/huit/nepho)


### Supporting Services

* [Netflix Open Source Software](http://github.com/netflix/)


### Standards

* http://12factor.net
* [The Twelve Factor App (Presentation)](http://prezi.com/8uldpq91vm4e/?utm_campaign=share&utm_medium=copy)

Blah
