<!--
  Replace the title, group members, research question and "About this
  project" below with your own project description. Keep the "Cloning" and
  "Reproducing" sections, and update them if you change how the project
  runs. Keep it short — a few lines per section is enough. This README is the
  front page of your repo, not the report itself (that's in report/);
  it just orients anyone (including us, grading) opening the repo for the
  first time.
-->

# Your Project Title

**Group members:**

- Andrei Dunuta
- Teodora Costache
- Filip Gawrylczyk

**Research question:** RQ 3. Do schools with similar test results give similar secondary-school advice?

**Level:** Inference 

## About this project

Our main goal is to find out if schools with the same test results give the same advice about which school the child should go to, while also seeing if school weights could explain these differences.
We first operationalized test result as the percentage of children in each school that passed the reference levels for reading and math.
Then we grouped advice into VWO and VWO/HAVO, HAVO and HAVO/VMBO and VMBO, PRO and VSO, so that we don't have too many levels. We also grouped schools on school weights as low, medium and high weights.
The first plot shows test results and school advice, and what the spread looks like between schools. Through this plot we found out that schools vary quite a bit with their school advice, even accounting for test results. 
The second and third plots how school weights influence that advice. We found out that they definitely do, but also most likely school weights are also correlated with test results, therefore we needed to look at the interaction, not just these two relationships.
The fourth plot shows us exactly that. It shows how many children were given specific advice based on school test results, but this time the results were grouped per school weights - low, medium and high. Based on this plot we can see that school weight significantly impacts what advice someone gets. 
Low school weight schools give more VWO advice, and less VMBO advice accounting for schools' test results compared to medium and high school weight schools. Meanwhile, high school weight schools give more VMBO advice and less VWO advice controlling for test results.


## Cloning this project

To get a copy of this project on your own computer, as an RStudio project:

1. On this repository's GitHub page, click the green `<> Code` button, choose **HTTPS**, and copy the URL.
2. In RStudio, make sure no project is open (top right: `Project: (None)`).
3. Go to `File` > `New Project` > `Version Control` > `Git`, paste the URL into `Repository URL`, choose where the project should live on your computer, and click `Create Project`.

RStudio opens the project, with a `Git` tab next to your `Environment` pane. Full instructions (including how to set up Git and GitHub on your computer first) are in the course's [Working with Git](https://ann1ejohansson.github.io/data-visualization-2026/documents/git-workflow.html) tutorial.

## Reproducing this project

1. Open the project in RStudio (double-click its `.Rproj` file, or clone it as described above).
2. Run `scripts/00-packages.R` to install and load the packages this project uses.
3. Run `scripts/01-get-data.R` once to download the data into `data/raw/`.
4. Knit `report/DV-Assignment2-Part2-GroupX.Rmd` (the final report). Knitting runs both scripts above for you.
