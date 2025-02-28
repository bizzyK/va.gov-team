# DRAFT

This is a folder for the Cerner integration work. 

# Cerner Integration Status

 ![image](https://user-images.githubusercontent.com/72028011/204892453-26fb3347-cc14-4bb0-8853-9833501dcd7d.png)

| Product  | Status |  Note(s) |
| ------------- | ------------- | ------------- |
| Patient Check-in (PCI)  | SVD  | Waiting for task order to be funded. |
| VEText (part of PCI)  |  SVD | Waiting for task order to be funded. |
| Applications for Visit Summaries (AVS) | SVD  | Waiting for task order to be funded. |
| MyHealtheVet (MHV) |  | ------------- |
| [Clinical Decision Support Platform](https://github.com/department-of-veterans-affairs/cdsp-program) (CDSP) | ATC | ------------- |
| [Covid-19 Patient Manager](https://github.com/department-of-veterans-affairs/covid-patient-manager/) (CPM) | ATC | ------------- |
| [Lung Cancer Screening](https://github.com/department-of-veterans-affairs/lung-cancer-screen-and-track) (LCS) |  | ------------- |
| Precision Oncology (PO) |  | ------------- |

# Cerner Environments
- Dev Sandbox: C1941 https://cernabcn.cernerworks.com/Citrix/ProdWeb/
- Stage: B1930
- Prod: P0630

# Requesting Access to Cerner Environments
Placeholder 
- C1941 Access

# Fundamental Documents

[VA.gov Health Products: Cerner API Requirements](https://github.com/department-of-veterans-affairs/va.gov-team/files/10126803/2020-January-Cerner.API.Documentation.Revision.1.docx)

# Cerner Integration Points

## Covid-19 Patient Manager
- Create CPM FHIR app deployed as a Cerner mPage component 
- Integrated CPM within Provider Workflow mPages
- Reads Cerner vital signs, specific labs, imaging using FHIR Observation 
