# T3A1 Workbook
### Nicholas Ducker

***


<details>
<summary>Q1</summary>
<br>

  #### Provide an overview and description of a standard source control process for a large project

  Managing a the code of a large scale project is in itself quite a challenging task. Having multiple developers work simultaneously on a code base will inevitably lead to bugs unless each developer explicitly knows what the other developers are doing and how they're doing it. 

  This is where source control steps in. The goal is twofold. Source/version control systems are geared to maintain the integrity of the "Trunk" copy of the project, whilst allowing developers to easily make controlled, reversible, logged changes to the trunk through a variety of different ways.

  For this question, I will describe the Gitflow workflow, which uses Git as its source control system and the Gitflow "wrapper" around the regular Git CLI.
  
  The Gitflow workflow is a great fit for a large project with many developers, as it adds another layer of structure around the "Feature Branching" workflow. In a common feature branching workflow, developers will generally "branch" a copy of the trunk repo onto their machine and work on a new feature. When the new feature is implemented and tested on this branch, the developer then merges is back into the trunk and resolves any conflicts.


  Gitflow breaks these branches up into 5 different types:

  *  Trunk: The stable, released version of the software. There is only one Trunk. Only Hotfix and Develop branches can be branched off this.
  *  Develop: A copy of the Trunk branch. This branch is used to create and integrate Feature branches.
  *  Hotfix: This is the only kind of branch that can be branched off the master more than once. It serves to fix bugs in the current release of the Trunk branch. Any changes here are also pushed into the develop branch.
  *  Feature: The feature branch is branched directly off the Develop branch and is used to add new features to the Develop branch.
  *  Release: The release branch is branched off the Develop branch. Any bug fixes needed are done on this branch before its pushed to the Trunk for release. Any changes here are also merged into the Develop branch.

To further explain this workflow, I've included an diagram below.

![Gitflow workflow diagram](imgs/20180412-git-flow.png)

In the above diagram, we have a stable v1.0 release of the Trunk (or Master) branch. 

A develop branch is created as a direct copy of the current release of the Trunk branch.

Just below the Trunk a Hotfix branch has been created to fix a bug in the existing production software. When this is completed, it is merged back into the Trunk and the production software is re-released and updated at v1.1. This Hotfix is also merged into the Develop branch and should also be merged into any existing feature branches (this is not illustrated on the diagram). Hotfix branches that are completed are deleted.

A Feature branch has also been created off of the Develop branch and is being worked on. When this is complete and has been tested, it is integrated back into the Develop branch. At this stage, the Develop branch is ready for a release, so a Release branch is created. Feature branches that have been completed are deleted.

The Release branch is independently tested for bugs. Any bug fixes on this branch are merged with the Develop and Feature branches. Once the Release is ready, it is merged into the Trunk branch as the next release, in this case v1.2. It is also finally merged back into the Develop branch and deleted. 

Using this approach to software development. A large project can have multiple teams working independently on many parts of the code base with less risk of conflicts emerging or the code base becoming unstable. 

  <details>
  <summary>Resources</summary>
  <br>

    * https://www.atlassian.com/git/tutorials/comparing-workflows
    * https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow
    * https://www.youtube.com/watch?reload=9&v=1SXpE08hvGs
    * https://www.campingcoder.com/2018/04/how-to-use-git-flow/
    
  </details>
   
</details>



<details>
<summary>Q2</summary>
<br>

  #### What are the most important aspects of quality software?

  Reliability: Software should reliably give consistently correct output under any condition. Errors that occur in the software have been planned for and are handled. Users should not wonder whether the program is functioning correctly.

  Maintainability: Software should be created and updated in a way that it is easy to maintain. The code base should be written in such a way that it is relatively easy to add new features or tweak existing ones. The maintenance and modification of the program should be thought of in advance and no two elements should be so tightly tied together than one exclusively relies on the other. Points for future new features should be considered from the outset. 

  Usability: The core functionality of the software should be obvious and easy to use. Common use cases should be catered for and made intuitive for users. The software shouldn't need a lot of configuration or intricate setup from the user. Navigation should be obvious and simple. A common design theme should be used throughout the software. 

  Testability: The core functionality of the software should be testable and the results verifiable. The production software will have its own automated testing suite. The tests for the software should be simple, easy to understand and specific. All business use cases should be tested for thoroughly before release. 

  Portability: 


  <details>
  <summary>Resources</summary>
  <br>

    *  https://www.silasreinagel.com/blog/2016/11/15/the-seven-aspects-of-software-quality/
    *  http://www.chappellassoc.com/writing/white_papers/The_Three_Aspects_of_Software_Quality_v1.0-Chappell.pdf
    *  https://www.softwaretestinghelp.com/what-are-the-quality-attributes/
    *  https://iso25000.com/index.php/en/iso-25000-standards/iso-25010?limit=3&limitstart=0
    
  </details>
   
</details>



<details>
<summary>Q3</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q4</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q5</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q6</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q6</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q7</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q8</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q9</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q10</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q11</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q12</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>



<details>
<summary>Q13</summary>
<br>

  

  <details>
  <summary>Resources</summary>
  <br>

    
    
  </details>
   
</details>
