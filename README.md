

### SciData Dataset: Cataloging Scientific Software from 131 Million Repositories - A Comprehensive Dataset of 350K Projects

The proliferation of open-source scientific software for science
and research presents opportunities and challenges. Our dataset
and paper address the critical need to curate a significant corpus of
scientific and research software repositories. Our approach involves
selecting projects from a pool of 131 million repositories from
the expansive World of Code data source followed by extracting
and analyzing README.md files with the assistance of Open AI’s
advanced large language models and classifying these repositories,
with a specific focus on software for scientific applications, projects
associated with research, and research support software. The SciCat
dataset is poised to be a valuable resource for conducting studies
on software relevant to science, shedding light on emerging trends,
prevalent practices, and prevalent challenges in scientific software
development. In addition, it includes data that can be connected
back to the World of Code, Github, and other repositories and
provides researchers with the basis for any number of comparative
studies. Scientific versus nonscientific software.

Description:
The provided dataset includes several columns with various types
of information. Each row in the dataset represents a unique project.
The details of the columns can be seen in Table ??. Finally, our
dataset is available online in the form of a Pickle file (in the repo: SciCat.pkl) and Certain
statistics are shown in Table 2.


### Table 1

| **Field Name**             | **Description**                                                                 |
|----------------------------|---------------------------------------------------------------------------------|
| ProjectID                  | A unique identifier for each project.                                           |
| url                        | A column for the URL of the project, likely on GitHub.                          |
| isScientificAppSoftware    | A boolean column indicating whether the project is scientific application software. |
| mentionsPaperOrFunding     | Indicates if the project mentions a paper or funding.                           |
| isResearchSoftware         | A boolean field to specify if the project is research software.                 |
| isScienceSupportSoftware   | Indicates whether the software supports scientific research.                    |
| keywords                   | A list of keywords associated with the project.                                 |
| shortdescription           | A brief description of the project.                                             |
| fullanswer                 | A longer, more detailed description or answer related to the project.           |
| NumForks                   | Number of forks of the project repository.                                      |
| AuthorsGender              | Provides information on the gender distribution of the project's authors.       |
| NumCommits                 | The total number of commits made in the project.                                |
| NumBlobs                   | The number of blobs (binary large objects) in the project.                      |
| CodeLanguages              | Lists the programming languages used in the project.                            |
| NumActiveMon               | The number of active months of the project.                                     |
| LatestCommitDate           | The date of the latest commit.                                                  |
| EarliestCommitDate         | The date of the earliest commit.                                                |
| CommunitySize              | Size of the community involved in the project.                                  |
| blobId                     | Unique identifier for the blob in the project.                                  |
| commitID                   | Unique identifier for the commit in the project.                                |

*Description of Data Fields in the dataset*

### Table 2

| **Criteria**                                    | **# of Projects** |
|-------------------------------------------------|-------------------|
| Scientific Application Software                 | 14,455            |
| Mentions Paper or Funding                       | 16,661            |
| Research Software                               | 5,750             |
| Science Support Software                        | 186,219           |
| Scientific App and Mentions Paper or Funding    | 6,349             |
| Research Software and Mentions Paper or Funding | 3,323             |
| Research Software or Scientific App and Mentions Paper or Funding | 8,085 |
| Total projects in final dataset                 | 342,656           |

*Number of projects based on different criteria*

### Using Pickle format in python
Please refer to https://wiki.python.org/moin/UsingPickle

