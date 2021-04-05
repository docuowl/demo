---
Title: Create Task
---

In order to create a Task, one must know the User ID to whom the task will belong
to. Knowing that information, issue a `POST` request to `/users/:id/tasks`, `:id`
being replaced with the user's ID.

#- Attributes
- title `string`
- A descriptive name for the task. For example, `But milk`.

The value returned will represent te internal Task object used by the API,
which will contain two extra fields besides `title`:

#- Attributes
- id `string`
- A unique value to identify this task among all other tasks
- title `string`
- The Task's title
- done `bool`
- Value indicating whether the task has been completed (`true`) or not (`false`)