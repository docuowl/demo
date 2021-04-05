---
Title: Marking as Complete
---

Marking a task as completed consists in issuing a `PATCH` request to `/users/:uid/tasks/:id`, 
which will mark a task with id `:id` belonging to User `:uid` as done.