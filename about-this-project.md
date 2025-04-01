---
layout: post
title: "About This Project"
permalink: about-this-project
---

 In the last years, Asia has been experiencing a surge in research production that will considerably change the landscape of computing research. This shift inevitably leads to a greater participation of Asian researchers in accepted papers, citations and program committees. To study these pivotal changes and evaluate international diversity, we have analyzed the past 11 years of 10 international systems research conferences: NSDI, SIGCOMM, EuroSys, ICDCS, Middleware, SOCC, CCGrid, IC2E, IEEE Cloud and EuroPar. Our analysis focuses on accepted papers, Program Committee participation, and citation patterns, grouping the results by country and region. We discover a particularly lopsided international diversity in a subgroup of top-tier conferences (NSDI, SIGCOMM, SOCC) which suggests a greater need for more proactive efforts to attract and embrace diversity and inclusion in accordance with fair open science practices.

## Selected Conferences

- **NSDI** (Symposium on Networked Systems Design and Implementation)
- **SIGCOMM** (ACM SIGCOMM Conference)
- **SoCC** (ACM Symposium on Cloud Computing)
- **EuroSys** (European Conference on Computer Systems)
- **IC2E** (International Conference on Cloud Engineering)
- **ICDCS** (IEEE International Conference on Distributed Computing Systems)
- **Middleware** (International Middleware Conference)
- **IEEE Cloud** (IEEE International Conference on Cloud Computing (CLOUD))
- **CCGRID** (IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing)
- **Euro-Par** (European Conference on Parallel Processing)

We have selected ten conferences related to Cloud Computing research. They represent popular conferences in the field that have been active in the past ten years. According to the [CORE ranking](https://portal.core.edu.au/conf-ranks/) we selected conferences ranked as A*, A, and B. SIGCOMM is ranked A+, and EuroSys, ICDCS, Middleware, CCGRID and NSDI received A rankings during these ten years, while IEEE Cloud and EuroPar were ranked as B. We also included two popular non-ranked conferences like IC2E and SoCC.

## How have we done it?

We have created a [crawler](https://github.com/Marina-LA/Conference-Data-Crawler),  that retrieves information from conference websites and three major research sources: [DBLP](https://dblp.org/), [Semantic Scholar](https://www.semanticscholar.org/), and [OpenAlex](https://openalex.org/). Using the collected data, we explore how the systems research community is adapting to the geo-economic changes and in particular how this is reflected in terms of increasing international participation in research.

The data collected by the crawler has been stored in two databases available [here](https://github.com/Marina-LA/ConferenceData). One is a relational database, and the other is a graph database. The former stores data related to papers published in conferences, while the latter stores data related to citations made by conference papers. We consider citations to include all references listed in a conference paper, which means that citations may include other papers, journal articles, books, and more.

## Who are we?

This project has been carried out by the Cloud and Distributed Systems Lab research group at the Universitat Rovira i Virgili.
