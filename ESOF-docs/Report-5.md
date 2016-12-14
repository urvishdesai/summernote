<a name="TOP"> </a>
# Report 5 - Software Maintenance/Evolution 

## Index
1. [Introduction](#Introduction)
2. [Discuss Software Maintainability](#DiscussSoftwareMaintainability)
3. [Report evolution process](#Reportevolutionprocess)
4. [Link to pull request](#Linktopullrequest)
5. [Group Members Identification](#Group)

<a name="Introduction"> </a>
## Introduction

Since Summernote is a project still growing and evolving, there is still a large list of tasks and features to be developed and problems to be corrected. However, the project is open to the development of new features as long 
as it interest for the relevant project. Throughout this report will be described the process of identification, development and submission of a new feature of the Summernote project.

<a name="DiscussSoftwareMaintainability"> </a>
## Discuss Software Maintainability

We have ran the Better Codehub, later we call only BC, tool to check ten guidelines for maintainable software in the Summernote project.

We present below the results this tool provided in the same order presented to us. 

1. :x: Write Short Units of Code
2. :x: Write Simple Units of Code
3. :x: Write Code Once
4. :heavy_check_mark: Keep unit interfaces small
5. :heavy_check_mark: Separate concerns in modules
6. :heavy_check_mark: Couple Architecture Components Loosely
7. :heavy_check_mark: Keep architecture components balanced
8. :heavy_check_mark: Keep your codebase small
9. :x: Automate Tests
10. :heavy_check_mark: Write clean code

We have noticed a compliance classification of 6 out of 10, in such a way that we've got a badge of [![BCH compliance](https://bettercodehub.com/edge/badge/ei12134/summernote)](https://bettercodehub.com) which proves it.

To get more detailed information we provide a [link](resources/BetterCodeHub.pdf) to a pdf file that shows the ten guidelines with a list layout way.

[Go to top](#TOP)
<a name="Reportevolutionprocess">
## Report evolution process

#### Feature decision

The Summernote project repository provides a wide range of issues that are fed by the team members and by the community, as has been mentioned in previous reports. We wanted to chose a feature that was intended about a relatively short time and for that we search about date and with two labels: `feature-request` and `pull-request-wanted`.

After a careful analysis of this list, the group decided to evolve a feature that is based on issue #1885, which is the most recent feature, at the date of this report. The feature-request primarily wants the editor to be able to input colors for its foreground and background by `hexadecimal` format. The feature seemed important and was yet lacking in the original software.

#### Identification of components implementing the feature  

While running the Summernote in the browser, in this case we use Google Chrome, we detect some active components by using the code inspector on that browser. We followed the code inspector and found the code that implemented the current feature. The code is written in Javascript and the color can be applied through a color palette defined in the code. The color could be selected using function with event `click`. Hence, a few changes were required in this code.

#### Implementation of the feature

The feature required only to input color in hexadecimal format. But while searching, we found that we can implement an even better feature that implements html5 colorpicker which will take the input in hexadecimal as well as allow the user to input in the form of a gradient color map.  We observed that only a few additions were required to the code.

Thus, through a thorough analysis of the code, its syntax and indentation, we formulated the code and made it work after several attempts. And hence, the feature was implemented. A preview of the feature can be seen here:

![Feature html5 color input](resources/feature.png?raw=true "Feature html5 color input")

[Go to top](#TOP)
<a name="Linktopullrequest"> </a>
## Link to pull request

After the implementation of the new feature we've made a pull request in order to integrate it into the Summernote library. It has passed all the tests and the coverage of tests has remained the same. The link to our pull request is available and is visible [here](https://github.com/summernote/summernote/pull/2159).

[Go to top](#TOP)
<a name="Group"> </a>
## Group Members Identification 

|               Name              |         Email        | Contribution |
|---------------------------------|:--------------------:|:------------:|
| Artur Sousa Ferreira            | ei12168@fe.up.pt     |      25%     |
| José Filipe de Monteiro Peixoto | ei12134@fe.up.pt     |      25%     |
| Nuno Miguel Rainho Valente      | up200204376@fe.up.pt |      25%     |
| Urvish Sanjay Desai             | up201602683@fe.up.pt |      25%     |

[Go to top](#TOP)