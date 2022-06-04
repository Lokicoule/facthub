# UC_PRODUCT_UPDATE_PRODUCT

A. Actors

- User

B. Description

User wants to update one of his product.

C. Basic Flow

1. Use case begins when Actor navigate to `products/update/:id`.
2. Actor has to update the form
3. Form data is pre-checked by validation form schema and must conform to gql schema.

- a. If init state equals final state, nothing happen
- b. If pre-check failed, specifics errors should be displayed.
- c. If gql validation failed, graphql error should be displayed
- d. If pre-check and gql validation are successful, data can be send.

4. Actor has to be authenticated (cognito).
5. `ONLY` referential Product document is updated
6. Use case ends when Actor is redirected to last page (`/products/view/:id`).
