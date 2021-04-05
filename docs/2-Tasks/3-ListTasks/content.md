---
Title: Listing Tasks
---

The endpoint `/users/:id/tasks` is responsible for listing all tasks for a given
user. It also accepts an optional `status` querystring parameter, used to filter
which kind of tasks to list.

#- QueryString
- status `optional string`
- Optional parameter to only show tasks in a specific condition.
	- Enum values
		- all
		- Shows all tasks, independent of their status.
		- pending
		- Shows only tasks not marked as completed.
		- done
		- Shows only completed tasks.