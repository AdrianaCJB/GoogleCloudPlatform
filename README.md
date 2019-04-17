# GoogleCloudPlatform
Repository for issues about gcp components


A few components are:

[1. Airflow and core concepts: ](https://airflow.apache.org/) is a platform to programmatically author, schedule and monitor workflows.

Use Airflow to author workflows as directed acyclic graphs (DAGs) of tasks. The airflow scheduler executes your tasks on an array of workers while following the specified dependencies.

   - [DAG:](https://airflow.apache.org/concepts.html#dags) A Directed Acyclic Graph is a collection of all the tasks you want to run, organized in a way that reflects their relationships and dependencies.
   
   - [Operator:](https://airflow.apache.org/concepts.html#operators) The description of a single task, it is usually atomic. For example, the BashOperator is used to execute bash command.

   - [Task:](https://airflow.apache.org/concepts.html#tasks) A parameterised instance of an Operator; a node in the DAG.

   - [Task Instance:](https://airflow.apache.org/concepts.html#task-instances) A specific run of a task; characterised as: a DAG, a Task, and a point in time. It has an indicative state: running, success, failed, skipped, ...
