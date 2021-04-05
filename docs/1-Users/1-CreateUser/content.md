---
Title: Create User
---

Users can be created by issuing a `POST` request to the `/users` endpoint. An
user is required to have a `name`. Users with same name are allowed to coexist.

#- Attributes
- name `string`
- Name of the user being created

API will return the new user record, using the provided name, and a generated ID:

#- Response Values
- ID `string`
- Unique ID for the created user
- name `string`
- The user's name, as provided through the request