.. highlight:: rest
.. contents::

Workflow documentation requirements
------------------------------------

For hosting the workflow on NBCR website each workflow must have the following documentation: 

#. In plaintext, using the approved template, a general description of the workflow, a list of parameters, 
   and a description of the workflow's usage.
#. A JPEG image of the workflow
#. And, a list of keywords for the workflow.

Additional documentation should be provided in the download files. Keywords should include the scientific 
uses of the workflow and composite actors used in the workflow.

Workflow versioning requirements
---------------------------------

NBCR distributed workflows are required to use the following versioning method:

Workflow_name.a.b.extension (ex docking_workflow.1.2.tar)

a - this is the primary version number of the workflow. This must be an ascending number with no leading zeros.  
The primary version number represents significant changes in the underlying workflow. This includes but is not 
limited to changes in I/O file format, significant reconfiguration of the actors, or external program dependencies. 
Primary version numbers are not required to be backwards compatible.

b - this is the patch version number of the workflow. This must be an ascending number with no leading zeros.  
The patch version represents small modifications to the code that do not change I/O formats or external program 
dependencies. Patch versions should be compatible within the primary version number. 

Workflow download file requirements
------------------------------------

Workflows will be distributed as tar files containing a minimum of the workflow .car file and a file containing the 
documentation. Both the workflow .car file and the .tar file must use the naming convention with versioning described 
above.
