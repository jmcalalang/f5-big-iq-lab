Module 5: BIG-IQ Application Templates & Deployment with AS3 using the API (new 6.1)
====================================================================================

**[New 6.1.0]**

|diagram_as3_bigiq|

Overview
--------

In this module we will explore how to use F5's **AS3** extension
with **BIG-IQ 6.1**.

**Application Services 3 Extension** (referred to as AS3 Extension or more often simply AS3) is a flexible, 
low-overhead mechanism for managing application-specific configurations on a BIG-IP system.
AS3 uses a declarative model, meaning you provide a JSON declaration rather than a set of imperative commands.

The declaration represents the configuration which AS3 is responsible for creating on a BIG-IP system.
AS3 is well-defined according to the rules of JSON Schema, and declarations validate according to JSON Schema.
AS3 accepts declaration updates via REST (push), reference (pull), or CLI (flat file editing).

**BIG-IQ** is a a key component of F5 BIG-IP Cloud Edition™. This new solution
provides DevOps and application teams with self-service management of F5 application
services, along with per-app manageability and analytics. 

While working through this module we will be focusing on L4-L7 deployments
(Virtual Servers, Pools, etc).

`AS3 documentation on BIG-IQ integration with AS3`_

.. _AS3 documentation on BIG-IQ integration with AS3: https://clouddocs.f5.com/products/extensions/f5-appsvcs-extension/latest/userguide/big-iq.html

Layer 4-7 Application Service Delivery
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

L4-7 Application Service Delivery is accomplished by:

-  Providing **templates** within **BIG-IQ 6.1** as a Service Catalog. With **BIG-IQ 6.1**, you will have access to 
   the traditional templates provided with **BIG-IQ 6.0** but you'll be able to create new kind of templates to consume 
   **AS3**. 

.. note:: Moving forward, BIG-IQ will invest on AS3 Templates more than on existing BIG-IQ templates.

-  Utilizing BIG-IQ's **Role Based Access Control (RBAC)** to divide
   workloads based on user functions.

The labs in the module will focus on the high level features in place to
achieve full L4-7 automation.

In this Module, we will provision **BIG-IQ 6.1** to deploy and modify the AS3
declarations.

The focus of Module 5 was to demonstrate application deployment directly to the BIG-IP. 
**BIG-IQ 6.1** will allow the administrator to restrict access an interface and API for users based 
on their current role within the organization.

For example, in Module 5, we pushed AS3 declarations, updated pool members, and
provided the user access to modify the full AS3 declaration. This approach would
provide each user the same administrative priviledges and may not scale within
organizations with separate user functions.

To solve this problem, **BIG-IQ 6.1** allows the administrator to create
**Templates** which can provide further **Abstraction** of the AS3 declarations.
The administrator can enforce specific Tenants or parameters to be used based on
the user running the template. This abstraction allows the templates to be
integrated directly into the relevant CI/CD toolchains and workflows.

.. toctree::
   :maxdepth: 1
   :glob:

   lab*


.. |diagram_as3_bigiq| image:: ../pictures/module5/diagram_as3_bigiq.png
   :scale: 70%
