---
layout: post
title: OpenStack-ManageIQ-issues
author: Soniya Vyas
tags: [Issue, OpenStack]
---

## OpenStack and ManageIQ:-

ManageIQ can manage a variety of external environments, known as *__providers__* and *__managers__*. A provider or manager is any system that ManageIQ integrates with for the purpose of collecting data and performing operations.

In ManageIQ, a *__manager__* is an external management environment that manages more than one type of resource. One example of a manager is OpenStack, which manages infrastucture, cloud, network, and storage resources.

In ManageIQ, an OpenStack is a virtual infrastructure environment that you can add to a ManageIQ appliance to manage and interact with the resources in that environment. They can be either discovered automatically by ManageIQ, or added individually.

## OpenStack Pike

It's the 16th release of most Openstack, showcases the increased composability with enhancements to ironic bare metal, Cinder block storage and Neutron services. Although Pike introduces many features its installation with ManageIQ is tedious, since till date it is not a stable version.
When it comes to integration of OpenStack(Pike) with ManageIQ,it throws the following error:-
>No Information after adding OpenStack provider

When I tried to figure out the error, I observed that OpenStack-fog library is not [supported](https://github.com/fog/fog-openstack/blob/master/supported.md) by the pike which is indeed used by ManageIQ.So we need to comeback to the earlier stable release of OpenStack viz. Ocata or Newton.The Ocata worked fine with ManageIQ integration in our case.


