# Functional requirements

- ## UESR AUTHENTICATION AND REGISTRATION
  - user can sign up in the app
  - user can choose the role, while signing up
  - user can delete account and all entities are to be deleted in cascade mode
  - user can autenticate in the app using email + password
- ## CRUD + ROLE SYSTEM
  - user in "USER_MODE" can READ marine data, created by other users in "MARINE_MODE"
  - "MARINE MODE" user can CREATE, DELETE, UPDATE own cargo vessels, ports and cargo routes, as well as READ all marine data
- ## JOURNALLING
  - "MARINE MODE" user's actions, such as CREATE, UPDATE, DELETE are recorded in premanent journal with action type, object id and timestamp fields
  - "MARINE MODE" user can't delete journal, journal deletes itself with user deleteion
- ## APP REQUIREMENTS
  - functions for search in all tables, except user-related
