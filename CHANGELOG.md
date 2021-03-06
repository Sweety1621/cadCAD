# Changelog:
### August 17,  2020
Hot Fix: Missing required positional argument: 'configured_N'

### August 5, 2020
* Experiment Class: Representation of an experiment as one or more configured System Models

### June 22, 2020
* Bug Fix: Multiprocessing error for Windows

### June 19, 2020
    
### New Features:
##### [Local Execution Mode](documentation/Simulation_Execution.md)
* Default parallelization of Monte-Carlo / Stochastic simulations
* **Backwards Compatible** with given legacy modes names

##### [cadCAD Post-Processing Enhancements](https://github.com/cadCAD-org/cadCAD/blob/master/documentation/Simulation_Execution.md#execute-simulation-produce-system-event-dataset)
* Returns single dataset as three types depending on execution mode:
    * Local Mode:
        * 2d List
* Changes:
    * Returning a single dataset was originally specified at the project’s inception instead of multiple per simulation
* [System Configuration Conversions](documentation/System_Configuration.md)
    * System Configuration as List of Configuration Objects
    * System Configuration as a Pandas DataFrame
    * System Configuration as List of Dictionaries

**Backwards compatibility:**
* Expandable state and policy update parameter space enables changes to the parameter space of updates while 
supporting backwards compatibility
* Legacy execution modes supported

### May 29, 2020
* Packaging: Add [Nix](https://nixos.org/) derivation and shell for local development and distribution of cadCAD package 
using Nix. Nix is a powerful package manager for Linux and other Unix systems that makes package management reliable and reproducible, allowing you to share your development and build environments across different machines.
