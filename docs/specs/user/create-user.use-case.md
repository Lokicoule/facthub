# UC_USER_CREATE_USER

A. Actors

- User

B. Description

User sign in for the first time since he/she signed up.
Some data will be used by invoice and delivery-note generators.

C. Basic Flow

1. Use case begins when Actor sign in for the first time.
2. Actor has to complete a form
3. Form data is pre-checked by validation form schema and must conform to gql schema.

- a. If pre-check failed, specifics errors should be displayed.
- b. If gql validation failed, graphql error should be displayed
- c. If pre-check and gql validation are successful, data can be send.

4. Actor has to be authenticated (cognito).
5. [BR_USER_CREATE_USER_ID](#brusercreateuserid)
6. Use case ends when Actor is redirected to Home page.

---

# Business Rules

### BR_USER_CREATE_USER_ID

Should we keep the same id between user and aws (congito) services ?
The technical choice will be take soon.

- Extract id from cognito User contained by Apollo Context

or

- Let mongodb generate it
