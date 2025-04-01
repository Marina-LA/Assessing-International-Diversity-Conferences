---
layout: post
title: "Obtained Data"
permalink: /obtained-data
post-image: "/assets/images/Decoration/Top_Drawing.png"
description: Get to know the data used for the analyses. In this section, the data obtained will be detailed, along with some of the challenges we faced while collecting them.
---

To conduct this study, papers have been collected from the year 2012 to 2023. These papers belong to 10 different conferences (NSDI, SoCC, Middleware, EuroSys, ICDCS, CCGRID, Euro-Par, SIGCOMM, IEEE Cloud, and IC2E). Below, more details will be provided on the amount of data collected for the accepted papers, citations, and Program Committee members.

# Accepted Papers

The accepted papers are the papers that have been published in each of the conferences. These data have been obtained using the crawler. In total, 6,800 papers have been collected over the 11 years studied from the 10 conferences. The table below details the number of papers obtained for each conference in each of the 10 years studied.

<img src="/assets/images/Obtained-data/TotalAcceptedPapers.png" alt="Number of Accepted Papers for each Conference"  style="display: block; margin: auto; max-width: 100%">

## Accepted Papers Missing Data

Although in most cases it has been possible to obtain all the necessary data for the accepted papers, there have been situations where obtaining some of these data was not possible. Consequently, when assigning a paper to a continent, there are cases where this assignment could not be made due to missing data. The table below details the percentage of papers from each conference that do not have any assigned continent. As a result, in the subsequent analyses, this percentage of papers will not be taken into account.

<img src="/assets/images/Obtained-data/MissingAcceptedPapersData.png" alt="Percentage of Papers with Missing Data" width="20%" style="display: block; margin: auto;">

# Citations

For this study, we have considered cited papers as any document that has been cited or referenced in the accepted papers of the conferences. For this reason, we are not only referring to conference papers but also to journal articles, books, etc.

A total of 160,666 citation data points have been collected from all the accepted papers of the 10 conferences. The table below provides a detailed view of the number of citation data points obtained for each year in the 10 studied conferences. It is important to note that some citation data may be counted twice if they were cited in different years and different conferences. However, for the analyses conducted, papers that were repeated within the same conference in different years were counted only once.

<img src="/assets/images/Obtained-data/TotalCitations.png" alt="Number of Citations for each Conference"  style="display: block; margin: auto; max-width: 100%">

## Citations Missing Data

As observed, there is a large amount of citation data, making it very challenging to obtain complete information for each of them. As a result, the percentage of citation data lacking the necessary details for further analysis is very high.

To mitigate this issue, we implemented two additional steps.

### First Step

First, we aimed to ensure that the number of accepted papers without citation data was less than 10%. In most conferences, this requirement was met, except for one: NSDI. To address this, we chose to exclude papers from different years, ensuring that the number of accepted papers lacking citation information for certain years remained below 10%.

For this reason, the accepted papers from the years 2014, 2015, and 2022 of NSDI were excluded from the citation analysis.

After implementing this change, the number of available citation data points was reduced to 124,228. Even with this dataset, the percentage of citation data lacking sufficient information for analysis remained very high. The table below shows these percentages for each of the 10 conferences.

<img src="/assets/images/Obtained-data/MissingCitationsData.png" alt="Percentage of Papers with Missing Citations" width="20%" style="display: block; margin: auto;">

### Second Step

As seen in the previous table, the percentage of citation data lacking sufficient necessary information remained very high (over 30% in several conferences). Therefore, we opted to study the data distribution in a small sample of incomplete data.

The steps we followed were:

1. A random sample of 10% of the citation data that did not meet the requirements was selected. That is, citation data lacking the necessary information for the study. This was done only for the year 2023 for the NSDI and ICDCS conferences.

2. The missing information for this 10% sample was manually collected.

3. The distribution of these data was analyzed using the [Chi-Square Godness-of-Fit](https://en.wikipedia.org/wiki/Goodness_of_fit) method to evaluate whether the data followed a similar distribution.

The results showed that this small data sample did follow the expected distribution (i.e., the distribution observed in the rest of the data for which we do have complete information). Therefore, we concluded that the results obtained in the citation analysis are valid despite the small issue of missing data. Even if we had access to the missing data, the results would still follow the same distribution.

# Program Committee

The collection of program committee data has been more challenging. Although it was possible to automate the process, it was carried out manually. Consequently, there may be minor errors in the data due to human error. However, these data have been reviewed multiple times to minimize such errors.

Another issue encountered during data collection was that, in some cases, it was impossible to obtain any information about the program committee of a conference for a specific year.

In total, 12,147 program committee members have been collected. The table below provides a more detailed view of the number of program committee members obtained for each conference.

<img src="/assets/images/Obtained-data/TotalPCMembers.png" alt="Total Number of Program Committee Members per Conference" width="20%" style="display: block; margin: auto;">

## Committee Members Missing Data

For some program committee members, it was impossible to obtain all the necessary information for the desired analyses, as it could not be found. However, the only conference where the percentage of missing data exceeds 10% is Euro-Par, while for the rest of the conferences, this value does not exceed 1-2%.

<img src="/assets/images/Obtained-data/MissingProgramCommitteeMembers.png" alt="Percentage of Members without data" width="20%" style="display: block; margin: auto;">