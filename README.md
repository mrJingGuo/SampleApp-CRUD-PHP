# SampleApp-CRUD-PHP
SampleApp-CRUD-PHP

<p>Welcome to the Intuit Developer's PHP Sample App for CRUD operations.</p>
<p>This sample app is meant to provide working examples of how to integrate your app with the Intuit Small Business ecosystem. Specifically, this sample application demonstrates the following:</p>

<ul>
	<li>Create, Read, Query, Update, Delete, Void entities.</li>
	<li>All operations are performed using QuickBooks PHP SDK.</li>
</ul>

<p>Please note that while these examples work, features not called out above are not intended to be taken and used in production business applications. In other words, this is not a seed project to be taken cart blanche and deployed to your production environment.</p>  

<p>For example, certain concerns are not addressed at all in our samples (e.g. security, privacy, scalability). In our sample apps, we strive to strike a balance between clarity, maintainability, and performance where we can. However, clarity is ultimately the most important quality in a sample app.</p>

<p>Therefore there are certain instances where we might forgo a more complicated implementation (e.g. caching a frequently used value, robust error handling, more generic domain model structure) in favor of code that is easier to read. In that light, we welcome any feedback that makes our samples apps easier to learn from.</p>

## Table of Contents

* [Requirements](#requirements)
* [First Use Instructions](#first-use-instructions)
* [Running the code](#running-the-code)
* [Project Structure](#project-structure)


## Requirements

In order to successfully run this sample app you need a few things:

1. Install PHP SDK. Refer instructions [here](https://developer.intuit.com/docs/0100_quickbooks_online/0400_tools/0005_accounting/0209_php/0002_install_the_php_sdk).
2. A [developer.intuit.com](http://developer.intuit.com) account
3. An app on [developer.intuit.com](http://developer.intuit.com) and the associated app token, consumer key, and consumer secret.
4. One sandbox company, connect the company with your app and generate the oauth tokens.

## First Use Instructions

1. Clone the GitHub repo to your computer
2. Fill in the [`App.config`](CRUD/App.config) file values with the oauth tokens generated while connecting with the company.

## Running the code

This app is directed to provide individual sample code for CRUD operations for various QBO entities.
Each php file can be run individually.

Steps described below is to run the php file for creating a customer.

1. Open the terminal window or command prompt and cd into the CRUD directory `/SampleApp-CRUD-PHP/CRUD`
2. run the command `php CustomerCreate.php`
3. On the console you'll see the log being generated with the new customer id.
4. Request/Response xmls are generated in the [`Logs`](CRUD/Logs) folder

Follow similar steps for other classes.

Note: The sample code has been implemented for US locale company, certain fields may not be applicable for other locales or minor version. Care should be taken to handle such scenarios separately.

## Project Structure

* PHP code for CRUD operations are located under [`CRUD`](CRUD) directory
* PHP code for Helper Classes are located under [`helper`](CRUD/helper) directory
* Request/response xmls are located under [`Logs`](CRUD/Logs) directory

