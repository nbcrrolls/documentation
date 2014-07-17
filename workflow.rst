.. highlight:: rest
.. contents::

Workflow documentation requirements
------------------------------------

For hosting the workflow on NBCR website each workflow must have the following files: 

#. **Required files**

   + workflow PNG image 
   + workflow kar file 
   + text file "description" which contains a describing  of the workflow. 
     Please  see a *description-template* file for a file format and the explanation of 
     the keywords and content. 
   + README file with any additional information about the workflow.
     If there are any extra files intended for download with the workflow  
     they must be listed in README. 
   + Optional: any extra files (documentation, examples, etc.) that will
     be distributed with the workflow. Must be listed in README. 

#. **Versioning convention**

   Each workflow must have a unique version number which is a sequence-based identifier
   in the form of **major.minor[.revision]**:

   + **major** number is increased when there are significant jumps in functionality
   + **minor** number is incremented when only minor features or significant fixes have been added 
   + **revision** number is incremented when minor bugs are fixed. 

#. **Naming convention**

   Each workflow name includes a text written as upper **CamelCase** followed
   by a **_** and a version.  For example: LigandSimulation_1.2.3. 
   

#. **Example**

   The workflow for ligand simulation will have the following files:

   + LigandSimulation_1.2.3.kar
   + LigandSimulation_1.2.3.png
   + description
   + README
   + LigandSimulation_1.2.3.notes (optional file)


Workflow distribution requirements
------------------------------------

Workflows are distributed as tar.gz files which must contain : 

+ workflow kar file 
+ README file
+ any optional files (extra documentation or examples) 

Naming convention: WorkflowName_1.2.tar.gz 
