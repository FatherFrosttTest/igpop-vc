---
title: Provider Directory
---

# Provider Directory Aidbox API Queries
## Practitioner
##### Queries to get Practitioner entity with connected entities(PractitionerRole, Organization, Network, Location, Healthcare Service) by practitioner name, practitioner active flag and organization name

https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService

https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true

https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA

https://fhir.villagecare.org/PractitionerRole?\_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerActive=true&practitionerName=COSTA%20DANIELA&organizationName=FITNESS
____

## Organization
##### Queries to get Organization entity with connected entities(Organization Affiliation, Network) by organization name and organization active flag

https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network

https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network&organizationActive=true

https://fhir.villagecare.org/OrganizationAffiliation?\_include=OrganizationAffiliation:organization,OrganizationAffiliation:network&organizationActive=true&organizationName=SOUTHSIDE%20HOSPITAL
____

## Pharmacy
##### Queries to get Harmacy organization entity with connected entities(Healthcare service, Location) by pharmacy name and pharmacy active flag

https://fhir.villagecare.org/HealthcareService?\_include=HealthcareService:organization,HealthcareService:location&organizationType=pharmacy

https://fhir.villagecare.org/HealthcareService?\_include=HealthcareService:organization,HealthcareService:location&organizationType=pharmacy&organizationActive=true

https://fhir.villagecare.org/HealthcareService?\_include=HealthcareService:organization,HealthcareService:location&organizationType=pharmacy&organizationActive=true&organizationName=STARSIDE%20DRUGS
