
.. contents:: CONTENTS

==========================================
NBCR software release management process
==========================================

Current release management Status
------------------------------------

+ No current release schedule.
+ Use of differnt repositories  by different groups
+ No formal process, ad-hoc by different groups


Proposed
--------------

#. **Adopt use of revision control system**

   All products and supporting documentation must be in a repository.
   Specific choice is up to each developing team

#. **Establish regular software release cycle** 

   + define regular targeted (+/- week) release dates 2 times per year.
   + define release milestones for each product type ::
   
   		development and testing  
		freeze development  
		packaging  
		deployment  

#. **Identify products types** 

   + roll
   + workflow

   Each release of a product must have a ``Product Release Package`` which includes  

   #. Version
   #. identifiable distro in revision control repo 
   #. what is build and how (README?)
   #. Scripts for automated configuration 
   #. Scripts for automated Installation 
   #. Scripts for setting environment (all needed settings via scirpts, no manual edits)
   #. Unit/regression tests
   #. Documentation: 
  
      + Release Notes  
      + list of required hardware/software dependencies and requirements
      + configuration instructions
      + installation instructions
      + environment setting instructions
      + required infrastructure: what hardware, storage, network, sw license, etc.
      + specific docs for product types
 
#. **Automation**

   Automate much as possible. Standardize  and automate repetitive tasks

   #. build automation 

      + compiling
      + packaging
      + configuration
      + unit test

   #. use transient environments:  

      + everything is defined in a template and is under revision control
      + environment is fully scripted, no manual handling
      + environment is modified only by a versioned script, is automated and is a part of product release package

   #. deployment automation 

      + fully scripted environment
      + deployment is done via versioned script
      + test deployment to guarnatee executability
      + production deployment 

   Build, configure, package, and deploy construct  a ``Deployment Unit``

#. **Archiving** 

   establish what to archive, how often and where.

#. **Define product delivery pipeline**

   build  -> package -> test deployment -> production deploy  -> docucment and archive
