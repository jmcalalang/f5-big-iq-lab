Module 4: DNS Analytics
=======================

This section of the lab is design to present an overview of the DNS statistics that are available in BIG-IQ. While not a complete customer scenario, the UDF environment is built to provide some DNS traffic in order to populate the charts and graphs.

For this lab, the student is not asked to create any configuration, but rather just explore the information available.

Navigate to *Monitoring* > *Dashboards* > *DNS* > *Overview* 
In this view, you can see a general view of DNS traffic. The panels on the right-hand side may be used to limit the view to a particular device, Listener, or Sync Group.

.. image:: ../pictures/module4/Overview.png
  :align: center
  :scale: 50%
  
The Traffic tab shows 6 different charts that provide an aggregate view of DNS traffic and query types across all the BIG-IP DNS devices. It still possible to limit the scope of the charts to a particular device, Listener, or Sync group using the panel on the right.

.. image:: ../pictures/module4/Traffic.png
  :align: center
  :scale: 50%
  
The GSLB tab focuses on the Global Server Load Balancing function. The second chart is very useful in identifying potential GSLB decisions. If for example, there were a large number of Alternate selections it could indicate a problem.

.. image:: ../pictures/module4/GSLB.png
  :align: center
  :scale: 50%
  
The Services tab contains 7 different charts which essentially cover all the services which could be configured in a DNS Profile. Please scroll down to review them all. Again, some of these charts can be indicators of issues in the environment.

.. image:: ../pictures/module4/Services.png
  :align: center
  :scale: 50%
  
The charts on the Attacks and Violations tab indicate Protocol Violations found in both hardware and software. The Hardware Protocol Violations are only implemented on the B2250 blade at this time. And, since we aren't generating bad DNS traffic these charts are empty.

.. image:: ../pictures/module4/Attacks-Violations.png
  :align: center
  :scale: 50%
  
The Top Charts tab provides summary of top source IPs, Domain names, and Wide IP stats. Because of the limited implementation in the UDF environment, there is limit information.

.. image:: ../pictures/module4/TopCharts.png
  :align: center
  :scale: 50%