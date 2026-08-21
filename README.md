# Repository containing all examples and notes for the Github Actions course

* **Workflows**
  * The **top-level automated process** defined in a `.github/workflows/` YAML file.
  * Triggered by repository events like a code `push`, a `pull_request`, or a manual click or a schedule.
* **Jobs**
  * A **group of tasks** that execute on the same virtual machine or container (called a **Runner**).
  * By default, multiple jobs inside a single workflow run **in parallel** (at the same time).
  * You can set up dependencies so one job waits for another to finish.
* **Steps**
  * The **individual, sequential tasks** executed inside a job.
  * They run one after the other on the exact same runner, meaning they can share files and settings.
  * A step can run a raw shell command (`run`) or use a reusable plugin from the community (`uses`).
* **Workflow Runners**
  * Virtual servers that execute jobs from workflows(standard or self hosted).
  * Standard through windows, ubuntu, and mac. Managed service.
  * Self hosted run workflows on any infrastructure
