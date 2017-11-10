# Invoice-Finance-Dapp
Smart Invoice

First experiment of invoices on the Blockchain by EHDA. Please keep in mind that this project was an experimentation and is in no mean intended to be used in a production environment.

Installing the project

Dependencies

First, Install nodejs, then

npm install -G http-server
npm install -G truffle
You will also need to run an ethereum node. Geth can fulfill this purpose.

Running the project

Once you have all the dependencies installed and set up, you can just pursue by cloning this project git clone https://github.com/eulerhermesda/SmartInvoices then typing

cd SmartInvoices
truffle compile
truffle migrate
Copy the address of the Admin contract and open the file app/index.html. Click on the "Connect to account" Link and copy the address of the contract there.

You are all set!

Overview of the project

For an overview of the project please follow this link.

Technical description

The project was designed as follow:

An Admin Contract that is the entry point into the platform. This contract will take care of creating new invoices, following there statuses, building the graph of companies and alerting neighboring nodes.
A Client Contract representing invoices. This contract follows and register the events happening to an invoice.
The representation of an invoice in this experiment is really basic, the experiment focuses more on exploring the interaction between the contracts and the users rather than modeling the exact business process. Our future experiments will also focus on modeling how a real invoice and Trade Financing process would be like.
