# Development of Forecasting Support System, Stage I
The aim of the project is to develop an R Shiny application that would allow analysing data (downloaded from SQL) and produce point and interval forecasts for specified temporal and cross-sectional levels of data for the specified forecast horizon.

The Forecast Support System (FSS) is focused on working with the admittance of patients in hospitals, but can be extended to work with other data. The main advantage in focusin on this data is because it has many frequencies (the data is recorded, when patients come) and many categories (sex and age groups, types of disease etc). This allows developing a system that can be easily extended and applied to other forecasting related problems, such as demand forecasting for retailers, energy forecasting, tourism forecasting etc.

The final aim of the project is to develop a FSS constructor, which could be deployed in any organisation with a minimum knowledge of R from the admin team.

The project will be carried out in three stages over the three years:

1. The first one is to take place in 2020, and will be focused on the development of R Shiny application based on the existing forecasting packages and the connection between the R Shiny and the SQL database.
2. The second stage will introduce the more complicated interactions between the users and the FSS, allowing amending the produced forecasts and prediction intervals and add explanatory variables.
3. On the final stage, the constructor will be created, allowing to deploy the FSS in any organisation and define which functionality to have.

The project is done with the support from South Tees Hospitals NHS Foundation Trust in England, which will provide the data and access to the database for the purposes of development and installation of the FSS.

The final system will be modular, allowing adding ore removing modules, based on the needs of users.



---------------

# Old stuff
This repository is a boilerplate repository that helps you prepare your proposal for the [R Consortium](https://www.r-consortium.org).

## Background 
Set up in 2015, the R Consortium is an organisation set up to help support the R Foundation, the R Community, and R users.

> The primary purpose of the R Consortium (collectively, the “Purpose”) is to: 
>
>(a) advance the worldwide promotion of and support for the R open source language and environment as the preferred language for statistical computing and graphics (the “Environment”);
>
>(b) establish, maintain, seek support for, and develop infrastructure projects and technical and infrastructure collaboration initiatives related to the Environment, and such other initiatives as may be appropriate to support, enable and promote the Environment; 
>
>(c) encourage and increase user adoption, involvement with, and contribution to, the Environment; 
>
>(d) facilitate communication and collaboration among users and developers of the Environment, the R Consortium and the R Foundation for Statistical Computing (the “R Foundation”); 
>
>(e) support and maintain policies set by the Board; and 
>
>(f) undertake such other activities as may from time to time be appropriate to further the purposes and achieve the goals set forth above.  
>
>In furtherance of these efforts, the R Consortium shall seek to solicit the participation of all interested parties on a fair, equitable and open basis.
> *[R Consortium Bylaws, Section 1.4](https://www.r-consortium.org/about/governance/bylaws)*

Delivery of the technical aspects for R Consortium's projects is overseen by the Infrastructure Steering Committee (ISC). The ISC is set up to receive, select, and manage projects that deliver upon the aims of the Consortium. The ISC will have an ongoing call for proposals and will select proposals to move into project stage approximately every six months. Within the process notes, it does say that if a proposal is unlikely to get funded then the proposers will be notified as soon as possible, partially so that re-submission can happen in the event fixable issues.

## Proposals
Here we detail useful guidance notes on making proposals to the ISC but you should always consult the [ISC Proposal page](https://www.r-consortium.org/about/isc/proposals) as there could be updates.

- Try to complete as many of the sections of this boilerplate document as possible. Each section is included either for practical purposes or has been specifically requested by the ISC
- Add relevant additional sections, like the letter of support from an R Core member if you want a change to R itself
- Proposals should be 2-5 pages when in PDF form
- You *can* submit a proposal on your own, but it's really recommended to get engagement from the community (and the ISC) first
- Proposals should be emailed to [proposal@r-consortium.org](proposal@r-consortium.org)

## Making your proposal
This is a boilerplate repository that you will need to fork, title appropriately and start filling in.

- Use the github [fork command](https://github.com/stephlocke/isc-proposal#fork-destination-box)
- Go to the repository settings and change the name to reflect your proposal
- Create a new Rstudio project from version control and use the git URL for the repo
- Write an overview of the proposal instead of this boilerplate for the README
- Start completing the relevant Rmd pages of the proposal
- Use `ghgenerate.R` to build the document
- Regularly commit and push the changes to github
- Solicit feedback and contributions from others

### Automatically generate your proposal
You can configure this to produce the needed documents and publish them to the github.io for browsing and posterity. This assumes a reasonable amount of comfort with using Travis-CI but if you're not, please check out my [post on auto-deploying documents](http://itsalocke.com/automated-documentation-hosting-on-github-via-travis-ci/) for background.

- Turn on [Travis-CI](https://travis-ci.org) for the repository
- Add an environment variable called GH_TOKEN to the travis environment, set the value to an OAuth key generated by github to allow "public repo" privileges only
- Amend the `.push_gh_pages.sh` and `ghgenerate.R` with the details of your repository and preferred commit details
- Use the gh-pages branch to host your proposal online and to retrieve the HTML or PDF variants for emailing


## License
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">ISC Boilerplate</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/stephlocke" property="cc:attributionName" rel="cc:attributionURL">Stephanie Locke</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/RConsortium/isc-proposal" rel="dct:source">https://github.com/RConsortium/isc-proposal</a>.
