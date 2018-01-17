# OpenStack

*Openstack* is a free and open source platform that build and manage private and public cloud. It is used to handle core cloud computing model like Compute, Networking, Identity, Storage and Image services. In virtualization, resources such as CPU, RAM and other facilities are bundled up and split by a hypervisor. Openstack is accessed either by web based dashboard through command line or by RESTful web services. 

Openstack was released on 21st Oct. 2010 i.e. 7 years back. Its latest stable release is Pike released on 31st Aug. 2017 i.e. 3 months back. Openstack is written in python. 

Openstack has a modular structure with different components of openstack that satisfy different requirements. Some of them are mentioned below.
Nova (Compute )
It provides a platform which are going to run our guest machine. It provides a control panel for the hypervisor. Each hypervisor require a separate nova instance. Nova support almost all the hypervisors known.

**Swift (Object Storage )**    
It provides cloud storage eg. Google Drive or Dropbox where they are not individually addressable objects. It is build for scale and optimization of durability, availability and concurrency across the data set. It is a deal with data that needs to store unstructured data that grow without bound. Files are stored in segments and manifest file tracks it.

**Cinder (Block Storage)**
It is also a storage module eg. external hard disk or USB device. It is slower than swift and has low latency. Cinder images are stored in our shared storage environment for readily availability. 

**Glance (Image Service)**
It is a image repository that store and manage our guest images, disk images, snaps, etc. It has pre built VM templates. Instance are booted from glance image registry. Custom images can be created and uploaded.

**Neutron (Networking)**
It was formally called as Quantum and provides networking as a service.It allows tenants to build rich network topologies and configure advanced networking policies.

**Horizon (Dashboard )**
It is  a dashboard of Openstacks, eyes and ears. It provides a web based user interfaces to openstack services including Nova, Swift, Keystone.

**Ceilometer (Telemetry)**
This component is responsible for metering information. It can be used to generate bills according to the statistics of usage. Administrator can have separate alarm clocks that can trigger on performance of statistics.

**Heat (Orchestration)**
It provides a human and machine accessible service for managing the entire lifestyle of infrastructure and application within the openstack cloud. It contains human readable templates with simple instructions that is read by heat engine.

**Keystone**
It authenticates and authorizes all the services of the openstack services. It is the end point catalog for all services.

All the above components make up the openstack. As openstack is free and open source, it allows anyone to add additional components to openstack to fulfil its requirements. The main element in openstack is Keystone. Every component plays a vital role in the scenario with different requirements and specifications. 

Openstack has different *distributions*. Some of them are as follows.

1. Bright Computing 
2. Canonical
3. IBM
4. Red Hat
5. Suse
6. Oracle
7. VMWare Integrated OpenStack
8. Mirantis

Though many vendors provide their own OpenStack variations, it's an open source project managed by The OpenStack Foundation. That means that even though there are a bunch of different distributions on the market, they're all derived from the same source code. It also means that you could download, install, and manage an entire OpenStack-based cloud deployment using in-house resources.

