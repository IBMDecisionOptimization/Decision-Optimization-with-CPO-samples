# IBM® Decision Optimization Modeling with CP Optimizer on DOcplexcloud

Welcome to IBM® Decision Optimization Modeling with CP Optimizer on DOcplexcloud.

This library contains various model examples. For each sample you can find here:
* **documentation** - a pdf file describing the optimization problem and the model
* **model files** - a folder containing the .cpo files

You can solve models with CP Optimizer on DOcplexcloud by uploading a CPO file. The CPO file can contain parameters for solving the problem. You cannot compress a CPO problem file at this time.

All files must be in the same root directory; uploads containing multiple directories are not supported. Problem files cannot connect to an external data source. You cannot drag and drop files directly from an archive viewer into the DropSolve interface. All files must be dropped on the DropSolve interface simultaneously.

Solving with the IBM Decision Optimization on Cloud service (DOcplexcloud) requires that you
[Register for a DropSolve account](https://dropsolve-oaas.docloud.ibmcloud.com/software/analytics/docloud). You can register for the DOcplexcloud free trial and use it free for 30 days.

## Model descriptions

### Flexible job-shop scheduling
How can a manufacturing company complete the processing of orders in minimal time when each order requires the use of a specific machine or a choice of specific machines in a specified sequence?

The Flexible Job-shop Scheduling Problem is as extension of the classical Job-shop Scheduling Problem. In the classical version of the job-shop scheduling problem, a finite set of jobs is processed on a finite set of machines. Each job is characterized by a fixed order of operations, each of which is to be processed on a specific machine for a specified duration. Each machine can process at most one operation at a time. Once an operation initiates processing on a particular machine, the operation must complete processing uninterrupted.

The flexible job-shop scheduling problem allows an operation to be processed by any machine from a specified set. The operation processing time might depend on the allocated machine. The problem is to assign each operation to a machine and to order the operations on the machines such that the maximal completion time (makespan) of all operations is minimized.

This problem is an example of a scheduling problem in which operations are represented by special variables that are called interval variables and interval sequence variables. An interval has a start time, an end time, and a duration. An interval sequence variable (also called a sequence variable) represents a total ordering of the interval variables of the set. There are special constraints for intervals and sequences, including precedence constraints, no overlap constraints, and alternative constraints, which are used to model this problem.

### Job-shop scheduling (FT10)

How can a manufacturing company complete the processing of orders (jobs) in minimal time when each order requires the use of specific machines in a specific sequence?

The Job-shop Scheduling Problem is one of the best-known machine scheduling problems. In the classical version of the problem, a finite set of jobs is processed on a finite set of machines. Each job is characterized by a fixed order of operations. Each operation is to be processed on a specific machine for a specified duration. Each machine can process at most one operation at a time. Once an operation initiates processing on a particular machine, the operation must complete processing on that machine uninterrupted.

The objective of the problem is to find a schedule that minimizes the end time (makespan) of the schedule.

This problem is an example of a scheduling problem in which operations are represented by special variables that are called interval variables and interval sequence variables. An interval has a start time, an end time, and a duration. An interval sequence variable (also called a sequence variable) represents a total ordering of the interval variables of the set. There are special constraints for intervals and sequences, including precedence constraints and no overlap constraints, which are used to model this problem.

### Resource scheduling

How can a manufacturing company complete the processing of tasks in minimal time when each task requires a certain amount of constrained resource?

The Resource Constrained Project Scheduling Problem (RCPSP) is a generalization of the production specific Job-shop, Flow-shop, and Open-shop Scheduling Problems. Given:

    a set of tasks to be performed,
    a set of q resources with given capacities,
    a network of precedence constraints between the tasks, and
    for each task and each resource, the amount of the resource that is required by the task over its execution,

the objective of the RCPSP is to determine a schedule that meets all the constraints and whose makespan (that is, the time at which all tasks are finished) is minimal.

This problem is an example of a scheduling problem in which tasks are represented by special variables that are called interval variables. An interval has a start time, an end time, and a duration. There are special constraints and expressions for intervals, including precedence constraints and resource capacity constraints, which are used to model this problem.


## License

This library is delivered under the  Apache License Version 2.0, January 2004 (see LICENSE.txt).
