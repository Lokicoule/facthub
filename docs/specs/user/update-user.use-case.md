# UC_USER_UPDATE_USER

A. Actors

- User

B. Description

User wants to update his profile.

C. Basic Flow

1. Use case begins when Actor navigate to "profile/update".
2. Actor has to complete a form
3. Form data is pre-checked by validation form schema and must conform to gql schema.

- a. If pre-check failed, specifics errors should be displayed.
- b. If gql validation failed, graphql error should be displayed
- c. If pre-check and gql validation are successful, data can be send.

4. Actor has to be authenticated (cognito).
5. Updated email should be propagated to cognito (username) and user datastore.
6. Use case ends when Actor is redirected to Home page.
