Spiceworks Cloud Integration Platform Documentation
===================================================

The purpose of this document is to provide API and system level documentation for building a Cloud Integration using the Spiceworks Plugin Platform. It will be broken down into multiple README files based on topic, usually covering one specific API and its examples. In this document, we will cover:

1. What is Spiceworks?
2. What is a Spiceworks Plugin?
3. How does the Cloud Integration Platform work?

What is Spiceworks?
-------------------

Spiceworks is a systems management application and help desk installed inside of a user's network, behind their firewall. Many IT professionals use Spiceworks as their sole IT management application on their network. It has many network scanning, detection, monitoring, alerting, and reporting features for network and systems management.

Spiceworks is built as a web application that is accessed via the browser. It is built with Ruby on Rails and is packaged as a standalone service that runs on a Windows machine.

What is a Spiceworks Plugin?
----------------------------

Because Spiceworks is a web-based application, the best way to modify or extend the application via "plug-in" technology is through Javascript. A Spiceworks plug-in is a collection of Javascript files, HTML fragments, CSS, and images that are used to modify or extend Spiceworks behavior or its user-interface (and often times both).

A Spicework plugin's javascript can be added to the applications page via a &lt;script&gt; tag. This javascript will leverage javascript-based plug-in APIs to access the services provided by the Spiceworks platform. Because it runs in the browser, it also allows the plug-in author to modify the DOM structure to introduce new UI elements where necessary.

How does the Cloud Integration Platform work?
---------------------------------------------

Any service provider that wants to build an integrated application within Spiceworks will use the plug-in tools and APIs provided, and will be distributed through the Spiceworks network. To understand how the Cloud Integration platform operators, its important to understand the common elements of what a data integration would look like between Spiceworks and a Service Provider. Every integration has the following common elements:

1. External Service Provider Account Authentication
2. Data storage, data reporting
3. Data collection
4. Monitoring and Alerting
5. UI and module integration (tickets, purchases, etc)

Essentially all integrations can be boiled down to these common components. Defining the parameters and behaviors of these components is then all that is necessary to build a functional integration.