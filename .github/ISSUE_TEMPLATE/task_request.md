name: Task Request
description: Create a new task
title: "[Task]: "
labels: ["task"]

body:
  - type: input
    id: task-name
    attributes:
      label: Task Name
      description: What is the task name?
      placeholder: ex. Add login page
    validations:
      required: true

  - type: textarea
    id: task-description
    attributes:
      label: Task Description
      description: Describe what needs to be done.
      placeholder: Explain the task details.
    validations:
      required: true

  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: Select task priority.
      options:
        - Low
        - Medium
        - High
    validations:
      required: true

  - type: checkboxes
    id: confirmation
    attributes:
      label: Confirmation
      options:
        - label: I confirm that this task is clear.
          required: true