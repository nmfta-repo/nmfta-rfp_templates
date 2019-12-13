# NMFTA Request For Proposal Contract Template Language Documents

A template for Motor Freight Carriers to use in procuring telematics systems and ensuring that these systems fulfill cybersecurity requirements.

![NMFTA Logo](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/image1.png)

This repository hosts a *Template Request for Proposals* and some associated documents; all documents are licensed under the [Creative Commons `BY-NC-ND` 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/):

[![License: CC BY-NC-ND 4.0](https://licensebuttons.net/l/by-nc-nd/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-nd/4.0/)

* `TEMPLATE Request for Proposals.docx` --  the template *Request for Proposals* capturing contract details and expectations for proposals from vendors
* `TEMPLATE Request for Proposals Appendix I - Requirements Questionnaires.xlsx` -- the template requirements questionnaires for completing with functional & technical requirements for the project as well as collecting ready-made sets of cybersecurity requirements.
* `Request for Proposals Appendix II - Cybersecurity Requirements Matrix.xlsx` -- the complete list of cybersecurity requirements with details and validation steps
* `TEMPLATE Proposals Assessment.xlsx` -- the template proposals assessment for completing with assessments of the vendor (response) proposals

# Download

[Download the latest (v1.0) release of these RFP Templates here](https://github.com/nmfta-repo/nmfta-rfp_templates/releases/download/v1.0/nmfta-rfp_templates-v1.0.zip)

# Contributors

The Request For Proposal Contract Template Language project was made possible through the generous contributions of
thought leadership and technical expertise of many collaborators across the heavy vehicle cyber security community,
working to push the industry forward and make it more resilient. Though some of our contributors wish to remain
anonymous, we are deeply grateful to everyone who has given their time and energy to make this a reality.


| **Fleet Managers**   | **Telematics Providers** | **Independents**                                                |
|:--------------------:|:------------------------:|:---------------------------------------------------------------:|
|                      | Derek Held, Zonar Systems| Altaz Valani, Security Compass                                  |
|                      | Geotab                   | Mr. Mark Zachos, President, DG Technologies                     |

![Zonar Systems](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/zonar-logo-RGB-750.png) ![Geotab](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/geotab-logo_full-colour-rgb_resized.png) ![Security Compass](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/securitycompass-logo-resized.jpg) ![DG Technologies](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/dg-logo.png)

# Usage

These documents are intended to be used by motor freight carriers in procuring telematics systems in the Request for Proposal (RFP) phase. The workflow of a motor freight carrier and a vendor engaging in an theoretical RFP process is depicted below. In the sections that follow the intended use of each of the documents and templates in this repo is described within the context of this theoretical RFP process.

![RFP Overview](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/overview.PNG)

## `TEMPLATE Request for Proposals.docx`

![TEMPLATE Request for Proposals use](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/template_rfp.PNG)

Users should rename this to `<COMPANY> <PROJECT> Request for Proposals.docx` and fill-in the highlighted passages as needed. then attach `Request for Proposals Appendix II - Cybersecurity Requirements Matrix.xlsx` and `<COMPANY> <PROJECT> Request for Proposals Appendix I - Requirements Questionnaires.xlsx` to the package sent to vendors.

## `TEMPLATE Request for Proposals Appendix I - Requirements Questionnaires.xlsx`

![TEMPLATE Requirements Questionnaire use](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/template_questionnaire.PNG)

Users should rename this to `<COMPANY> <PROJECT> Request for Proposals Appendix I - Requirements Questionnaires.xlsx` then

1. Extend the functional and technical requirements tables in the eponymous excel tabs.
2. Fill-in the cybersecurity requirements tab by collecting groups of cybersecurity requirements from the *Cybersecurity Shortlists* tab.

## `TEMPLATE Proposals Assessment.xlsx`

![TEMPLATE Proposal Assessment use](https://raw.githubusercontent.com/nmfta-repo/nmfta-rfp_templates/master/media/template_assessment.PNG)

Users should rename this to `<COMPANY> <PROJECT> Proposals Assessment.xlsx` then complete the cells of the spreadsheet by referring to vendor (response) proposals. Finally, use the completed sheet to find the most suitable proposal.

# How to Make Contributions

The NMFTA would like these templates to be as useful as possible. We are open to refining them based on your feedback and/or changes which you would like to see made to the templates. However, the NMFTA, does not want these requirements or templates to be 'forked' or other custom versions of the requirements or templates to be proliferated. This is the reason for the [Creative Commons `BY-NC-ND` 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/) license of all the materials here.

The NMFTA will take your request for changes in whatever form is most convenient to you; an email or phone call is sufficient. The following steps are for those users who wish to propose concrete changes to the documents but also for reference by those at the NMFTA that will otherwise make the changes which are requested by our users.

## Instructions to Prepare Changes to the Files

For changes to `TEMPLATE Request for Proposals.docx` or `TEMPLATE Proposals Assessment.xlsx` : make them directly in those files and create a pull request.

For changes to either `TEMPLATE Request for Proposals Appendix I - Requirements Questionnaires.xlsx` or `Request for Proposals Appendix II - Cybersecurity Requirements Matrix.xlsx` the source spreadsheet, `src/Source Sheet for Edits - Shortlists and Requirements Matrix.xlsx` should be edited and the contents of both `TEMPLATE Request for Proposals Appendix I - Requirements Questionnaires.xlsx` or `Request for Proposals Appendix II - Cybersecurity Requirements Matrix.xlsx` should be regenerated:

1. Make edits to `src/Source Sheet for Edits - Shortlists and Requirements Matrix.xlsx`
	* NB: for any changes to the `Matrix` tab category assignments (columns J,K,L,M); the column A must be manually updated to reflect the state in those columns
	* NB: do not delete any blank rows in the `CyberReq Shortlist - Sorted` tab. These have important formulas in them to pull in data from the requirements matrix.
3. Copy and paste _as-values_ the contents of the `Matrix` tab columns A-I into the file `Request for Proposals Appendix II - Cybersecurity Requirements Matrix.xlsx` tab `Cybersecurity Requirements`
4. Copy and past _as-values_ the contents of the `Printable Matrix` tab into the file `Request for Proposals Appendix II - Cybersecurity Requirements Matrix.xlsx` tab of the same name.
4. Copy and paste _as-values_ the contents of the `CyberReq Shortlist - Sorted` tab into the `TEMPLATE Request for Proposals Appendix I - Requirements Questionnaires.xlsx` `Cybersecurity Shortlists` tab.
5. Remove blank rows from the `Cybersecurity Shortlists` tab.
6. Copy and paste _as-values_ the contents in the `Cybersecurity Shortlists` tab under *Cloud or Back-end* to the default content in the tab `Requirements Questionnaires`
7. Commit the changes and make a pull request.
