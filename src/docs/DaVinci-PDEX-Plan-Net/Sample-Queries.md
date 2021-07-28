---
title: Sample Queries
---

# DaVinci PDEX Plan Net API Query Examples

This page contains short descriptions of Practitioner and Organization search queries, lists of search parameters, and sample queries.

## Practitioner

Practitioner query is used to get full information about practitioners.

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService)

It returns a JSON object with a list of all entities of DaVinci PDEX Plan Net Profiles connected with a Practitioner entity:

- Practitioner
- PractitionerRole
- Organization
- Network
- Location
- HealthcareService

#### Search parameters
1. practitionerActive - practitioner active flag
2. practitionerName - practitioner name
3. organizationName - organization name
4. practitionerNetwork - practitioner network code
5. practitionerSpecialty - full practitioner specialty name
6. practitionerType - full practitioner type name
7. practitionerSpecialtyCode - practitioner specialty code
8. practitionerTypeCode - practitioner type code

#### Sample Queries

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY&practitionerType=SPECIALISTS](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY&practitionerType=SPECIALISTS)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY&practitionerType=SPECIALISTS&practitionerSpecialtyCode=30001](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY&practitionerType=SPECIALISTS&practitionerSpecialtyCode=30001)

[https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY&practitionerType=SPECIALISTS&practitionerSpecialtyCode=30001&practitionerTypeCode=SP](https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS&practitionerNetwork=MLTC&practitionerSpecialty=PHYSICAL%20THERAPY&practitionerType=SPECIALISTS&practitionerSpecialtyCode=30001&practitionerTypeCode=SP)
____

## Organization

Organization query is used to get full information about organizations.

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service)

It returns a JSON object with a list of all entities of DaVinci PDEX Plan Net Profiles connected with an Organization entity:

- Organization
- OrganizationAffiliation
- Network
- Location
- HealthcareService


#### Search parameters

1. organizationActive - organization active flag
2. organizationName - organization name
3. organizationNetwork - organization network code
4. organizationType - full organization type name
5. organizationSpecialty - full organization specialty name
7. organizationSpecialtyCode - organization specialty code
8. organizationTypeCode - organization type code

#### Sample Queries

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true)

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH)

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP)

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY)

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE)

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE&organizationTypeCode=AN](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE&organizationTypeCode=AN)

[https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE&organizationTypeCode=AN&organizationSpecialtyCode=66801](https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationActive=true&organizationName=INTERGEN%20HEALTH&organizationNetwork=MAP&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE&organizationTypeCode=AN&organizationSpecialtyCode=66801)
