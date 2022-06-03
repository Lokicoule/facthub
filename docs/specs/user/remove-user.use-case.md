# UC_USER_REMOVE_USER

A. Actors

- User

B. Description

User wants to delete his account.

C. Basic Flow

1. Use case begins when Actor navigate to "profile".
2. Actor has to click on remove button and complete a form with his email.
3. Form data is pre-checked by validation form schema and must conform to gql schema.

- a. If pre-check failed, specifics errors should be displayed.
- b. If gql validation failed, graphql error should be displayed
- c. If pre-check and gql validation are successful, data can be send.

4. Actor has to be authenticated (cognito).
5. User account should be deleted from cognito and user datastore.
6. User data should be purged.
7. Use case ends when Actor is redirected to sign in page.
