# UC_TRANSPORTER_REMOVE_TRANSPORTER

A. Actors

- User

B. Description

User wants to delete one or many of his referential transporter.

C. Basic Flow

1. Use case begins when Actor navigate to `/transporters` or `/transporters/view/:id`.
2. Actor has to click on remove button.
3. Actor has to be authenticated (cognito).
4. The transporter(s) should be `ONLY` deleted from TRANSPORTER referential document.

- From `/transporters` [BR_TRANSPORTER_REMOVE_TRANSPORTERS](#brtransporterremovetransporters)
- From `/transporters/view/:id` [BR_TRANSPORTER_REMOVE_TRANSPORTER](#brtransporterremovetransporter)

5. Use case ends when Actor is redirected to sign in page.

# Business Rules

## BR_TRANSPORTER_REMOVE_TRANSPORTER

- Remove transporter from id
- Return transporter data on success

## BR_TRANSPORTER_REMOVE_TRANSPORTERS

- Remove transporters from array
- Return true if all transporters are removed else return false.
