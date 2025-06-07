# Domain Design Exercise – Bank Application

## Domain Objects by Bounded Context

### Customer Management Context

* **Customer**: Contains basic customer details such as ID, name, and address.
* **EmploymentDetails** *(Value Object)*: Includes company name, phone number, salary range, occupation, and designation.

### Account Management Context

* **Account**: Base entity for all accounts. Contains account type, number, branch info, and balance.
* **SavingAccount / CurrentAccount**: Specialized account types extending from Account.
* **Balance** *(Value Object)*: Represents the amount and currency of funds in an account.

### ATM Card Management Context

* **ATMCard**: Represents the ATM card issued to a customer with issue date.
* **CardStatus** *(Value Object)*: Represents the status and expiry of an ATM card.

### Branch Management Context

* **Branch**: Represents a bank branch with name and address.
* **Region** *(Value Object)*: Contains regional classification details.

## Associations

* A Customer has EmploymentDetails and may hold one or more Accounts.
* A Customer may apply for a single ATMCard.
* Each Account is associated with a Branch and has a Balance.
* An ATMCard has a CardStatus.
* A Branch belongs to a Region and serves Customers informally (no direct reference).


