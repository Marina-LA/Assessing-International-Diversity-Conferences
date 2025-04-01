---
layout: post
title: "Diversity Index"
permalink: /diversity-index
post-image: "/assets/images/Decoration/World_Drawing.png"
description: Discover how the Gini-Simpson index is used to measure diversity in top computer systems conferences. Explore how geographic distribution impacts accepted papers, citations, and program committees, revealing disparities in representation across continents.
---

To quantify the diversity of the conferences, we used the [Gini-Simpson index](https://en.wikipedia.org/wiki/Diversity_index##Simpson_index), a variation of the Simpson diversity index widely used in Biology to measure species biodiversity in a given area. We applied it to determine the diversity of the conferences across four categories (North America, Europe, Asia, and Others) based on the number of papers published by each continent in the different conferences. The "Others" category includes all papers that do not belong to the three aforementioned continents but originate from other regions. This diversity was calculated for three distinct fields: accepted papers, the program committee, and cited papers.

<p>\[
  1 - D = 1 - \sum_{i=1}^{R} p_i^2
\]</p>

The Gini-Simpson index is calculated using the formula shown in the equation above. In this context, the number of available categories corresponds to the three continents considered: North America, Europe, and Asia. Each category has an associated proportion, which represents the share of papers from that continent relative to the total number of papers for a given conference (excluding those without an assigned continent).

This index estimates the probability that two randomly selected papers from the same conference come from different continents. A higher value indicates greater diversity, meaning the papers are more evenly distributed across the three regions. Conversely, a lower value suggests that one or a few continents dominate the conference's publications.

<img src="/assets/images/Diversity-index/GiniSimpsonDiversityIndex.png" alt="Simpson’s Diversity Index for Accepted Papers, Cited Papers and Committee Members" width="500"  style="display: block; margin: auto;">

The table above shows the diversity results obtained, where it is clear that conferences like CCGRID (0.685), ICDCS (0.623), and IEEE Cloud (0.654) have greater diversity in accepted papers compared to conferences like NSDI (0.406) and SIGCOMM (0.482). This seems to indicate that conferences such as ICDCS, CCGRID, and IEEE Cloud have a more balanced geographic distribution of accepted papers, suggesting a more international scope compared to NSDI and SIGCOMM. This behavior is reflected in the graph showing the [continent distribution of the accepted papers]({{ site.baseurl }}{{ site.url }}{{ site.posts | where: "title", "Accepted Papers" | map: "url" | first }}), where it can be observed that conferences like CCGRID and IEEE Cloud have accepted papers more equitably distributed among the continents, while NSDI and SIGCOMM show a strong dominance of a single continent, with North America being predominant, accounting for more than 70% of the accepted papers.

In the cited papers category, the indices are generally higher, which suggests that the academic impact of the conferences transcends the regions where their accepted papers are concentrated. For example, NSDI's index increases from 0.406 to 0.512, reflecting greater diversity in citations than in accepted publications. This trend holds true for all the conferences studied. Finally, the committee members category shows patterns similar to those observed in the accepted papers: conferences such as ICDCS (0.606), IEEE Cloud (0.627), and CCGRID (0.614) have more diverse committees compared to NSDI (0.323) and SIGCOMM (0.434).

Although conferences like CCGRID, ICDCS, and IEEE Cloud have a higher volume of published papers compared to NSDI and SIGCOMM, the diversity index results reflect that the latter have a less equitable distribution among the geographic regions considered. This indicates that, despite handling a smaller number of publications, NSDI and SIGCOMM concentrate most of their papers in one or two predominant regions, which reduces their diversity compared to conferences with a more balanced approach, such as ICDCS, CCGRID, and IEEE Cloud, which demonstrate a more proportional representation across the four categories analyzed.

As observed, some conferences are clearly more diverse than others. One might hypothesize that the location where a conference is held might influence the proportion of papers and members from a particular continent. While a more thorough investigation of the causes of disparity remains an open issue, some preliminary and informal analysis of the various conferences showed that this is not entirely the case.

What is true is that conferences like NSDI and SoCC have only ever been held in North America, which could explain their strong American presence. However, conferences like EuroSys and SIGCOMM challenge this argument. EuroSys is always held in Europe, yet it has a high proportion of American participants. On the other hand, SIGCOMM also moves to other continents, yet it remains predominantly American in representation.
