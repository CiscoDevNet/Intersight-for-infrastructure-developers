# Getting Physical Compute Inventory from Intersight using the Cisco Intersight REST API with the Python SDK

In this lab you learn how to retrieve a list of physical compute inventory from Cisco Intersight. 

## Objectives

The objective of this lab is to show how to:

* Authenticate with the Intersight using the Python SDK API's
* Call the Intersight API to pull a list of physical compute resources

## Prerequisites

Before getting started with this lab, you will need the following:

* An Intersight account (you may also need a Cisco account for credentials)
* API key
* API secret
* Familiarity with Python

### Background

Intersight has many capabilities and one of them is managing on-premises compute resources such as Cisco UCS servers. The process of making UCS servers available to Intersight is known as a claim. Thus, an administrator must first claim UCS servers before they are available as a resource in Intersight. After a UCS servers are claimed, they show up in inventory as physical compute servers.

In this lab we call the Intersight REST API's using Python and retrieve the inventory of physical compute resources claimed in Intersight.

**Next Step: Generate API key and Secret Key and import modules**
