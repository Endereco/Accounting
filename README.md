# Accounting

Generates Id's for transactions and counts transactions.

A transaction is a set of method calls from one specific service client. Each client starts a transaction of its own when the page is loaded. That transaction has an id and a counter.

This service creates a list of those transactions and their counters and passes it to doConversion logic when a conversion event happens.

Conversion event is something that is considered a success. e.g. a registration, a user updating its address, a user entering his address in checkout etc.

When this event happens the system should go through the transaction list and send doAccounting for each of them to Endereco Service. After that the list should be deleted.

## Installation

In order to pull the latest version:

### npm (preferred)

```
npm i @endereco/accounting
```

### github

```
git clone https://github.com/Endereco/Accounting.git
```

Then include Accounting.js in `<header>` or before config.

## Configuration

// TODO give an example @ilja
