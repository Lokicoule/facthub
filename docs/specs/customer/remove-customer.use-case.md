# UC_CUSTOMER_REMOVE_CUSTOMER

A. Actors

- User

B. Description

User wants to delete one or many of his referential customer.

C. Basic Flow

1. Use case begins when Actor navigate to `/customers` or `/customers/view/:id`.
2. Actor has to click on remove button.
3. Actor has to be authenticated (cognito).
4. The customer(s) should be `ONLY` deleted from CUSTOMER referential document.

- From `/customers` [BR_CUSTOMER_REMOVE_CUSTOMERS](#brcustomerremovecustomers)
- From `/customers/view/:id` [BR_CUSTOMER_REMOVE_CUSTOMER](#brcustomerremovecustomer)

5. Use case ends when Actor is redirected to sign in page.

# Business Rules

## BR_CUSTOMER_REMOVE_CUSTOMER

- Remove customer from id
- Return customer data on success

## BR_CUSTOMER_REMOVE_CUSTOMERS

- Remove customers from array
- Return true if all customers are removed else return false.
