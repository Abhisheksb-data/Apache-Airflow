Apache Airflow is an open source platform to programmatically author, schedule and monitor workflows 

AIRFLOW IS AN ORCHESTRATOR

Benefits of Airflow
	• DYNAMIC(python commands)
	• SCALABLE
	• INTERACTIVE (UI,CMD,REST API)
	• EXTENSIBLE(create your own plugin and customize airflow as per your need)

AIRFLOW is NOT a streaming solution or a data processing Framework

AIRFLOW CORE COMPONENTS
	• Web Server(UI for Monitoring)
	• Schedular(to schedule tasks)
	• Metadata Database(for keeping metadata)

MORE COMPONENTS
	• Executer(defines how your tasks are executed)
	• Worker(its where your tasks are Executed)

TYPES Of ARCHITECTURES
	• Single Node
	
	• Multi Nodes(celery)
	• 

CORE CONCEPTS DAGs
	• Directed acyclic graph
	• There is no loops
	Example-
	

	OPERATORS
	• Operators are tasks in your DAGs
	Example - 
	

TYPES OF OPERATORS
	• Action Operators - 
	( allows you to execute certain functions
	 example - Python function - python operator
	                    Bash command - Bash operator
	                    SQL request - Postgres operator  )
	• Transfer Operators 
	( allows you to transfer data from a source to a destination 
	Example - MYSQL to Presto operator(allows you to transfer data from MYSQL to PrestoDB)
	• Sensor Operators
	(used for sensing folder changes to trigger tasks)

	TASK
	• Instance of an operator

    TASK INSTANCE
	• Represents a specific run of a task: DAG + TASK +POINT IN TIME

   DEPENDENCIES
	• 
	• As a good practice use (<<) or (>>) for announcing Dependencies 

WORKFLOW
	• 
	• ALL THE THINGS MENTIONED ABOVE SINCE TASK IN ONE DIAGRAM
![image](https://user-images.githubusercontent.com/93099817/162578050-4b474159-668b-47a5-8ee3-fca7e63ec3a2.png)
