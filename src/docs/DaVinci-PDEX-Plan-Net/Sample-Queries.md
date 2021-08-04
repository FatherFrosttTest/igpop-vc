---
title: Sample Queries
---

# DaVinci PDEX Plan Net API Query Examples

This page contains short descriptions of Practitioner, PractitionerRole, Organization, and OrganizationAffiliation search queries, lists of search parameters, and sample queries.

## Practitioner

We store information about practitioners in these FHIR Entities:

- Practitioner - basic info about а practitioner. Contains demographics, specialty, language and identifiers like NPI and IRS
- PractitionerRole - central entity to connect practitioner's entities. Also contains info about available time
- Organization - practitioner's place of work
- Network - info about health plans a practitioner is connected with
- Location - practitioner's location info (address) and telecom info (phone, email) 
- HealthcareService - services provided by a practitioner

Practitioner queries examples:

- [Get 100 practitioners (by default)](https://fhir.villagecare.org/Practitioner)
- [Get practitioner by name](https://fhir.villagecare.org/Practitioner?name=GLASSER%20ANN)
- [Get practitioners by language](https://fhir.villagecare.org/Practitioner?communication=es)
- [Get practitioners by specialty](https://fhir.villagecare.org/Practitioner?qualificationName=PHYSICAL%20THERAPY)
- [Get practitioner by identifier](https://fhir.villagecare.org/Practitioner?identifier=1861919391)
- [Get practitioners by language AND specialty](https://fhir.villagecare.org/Practitioner?communication=es&qualificationName=PHYSICAL%20THERAPY)


##PractitionerRole

PractitionerRole is a central entity for a practitioner. It means that this entity contains info about practitioner, network, location, organization and healthcareService. You can use PractitionerRole to search practitioners in the selected network:

1. [Get practitionerRoles by network](https://fhir.villagecare.org/PractitionerRole?practitionerNetwork=MAP)	
2. Get Practitioner Fhir ID from the PractitionerRole entity
```json
"practitioner": {
  "id": "920c870c-2553-4ff0-b255-b2c58504dbce",
  "resource": {
    ...
  },
  "resourceType": "Practitioner"
}
```	
3. [Get practitioner by Fhir ID](https://fhir.villagecare.org/Practitioner?id=b061b7b9-79d6-4cf2-a758-41debb380760)


####Advanced PractitionerRole Queries

Also PractitionerRole entity is used to get all FHIR entities connected with a practitioner in one query. These queries can use multiple search parameters and you can include, exclude and combine them. Also you can control what entities will be returned by including and excluding entities from the _include parameter of these queries.

To add additional entities in the response, like Practitioner or Location you should use _include parameter, e.g.:

- [Get PractitionerRole and Practitioner entities](https://fhir.villagecare.org/PractitionerRole?_include=PractitionerRole:practitioner)	
- [Get PractitionerRole with Practitioner and Location entities](https://fhir.villagecare.org/PractitionerRole?_include=PractitionerRole:practitioner,PractitionerRole:location)		
- [Get PractitionerRole with all entities](https://fhir.villagecare.org/PractitionerRole?_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService)
	
	
Also you can use these search parameters:	

- practitionerName - practitioner name
- organizationName - organization name
- practitionerNetwork - practitioner network code
- practitionerSpecialty - full practitioner specialty name
- practitionerType - full practitioner type name
- practitionerSpecialtyCode - practitioner specialty code
- practitionerTypeCode - practitioner type code

Advanced PractitionerRole queries examples:

- [Get by practitioner name](https://fhir.villagecare.org/PractitionerRole?_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerName=SEQUEIRA%20RODRIGO)
- [Get by network code and practitioner specialty](https://fhir.villagecare.org/PractitionerRole?_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerNetwork=DSNP&practitionerSpecialty=GENERAL%20SURGERY)
- [Get by all search parameters](https://fhir.villagecare.org/PractitionerRole?_include=PractitionerRole:organization,PractitionerRole:practitioner,PractitionerRole:network,PractitionerRole:location,PractitionerRole:healthcareService&practitionerName=SEQUEIRA%20RODRIGO&organizationName=THE%20MOUNT%20SINAI%20HOSPITAL&practitionerNetwork=DSNP&practitionerSpecialty=GENERAL%20SURGERY&practitionerType=SPECIALISTS&practitionerSpecialtyCode=21001&practitionerTypeCode=SP)
___

##Organization

We store information about organization in these FHIR Entities:

Organization - basic info about an organization. Contains name, address, type, specialty, identifiers like NPI and telecom info like phone and email.
OrganizationAffiliation - central entity to connect organization's entities.
Network - health plans an organization is connected with
Location - organization's location (address) and telecom (phone, email) info 
HealthcareService - services provided in an organization

Organization queries examples:

- [Get 100 organizations (by default)](https://fhir.villagecare.org/Organization)
- [Get organization by name](https://fhir.villagecare.org/Organization?name=NORTH%20CENTRAL%20BRONX%20HOSPITAL)
- [Get organizations by address](https://fhir.villagecare.org/Organization?address=BRONX)
- [Get organizations by type](https://fhir.villagecare.org/Organization?type=HS)	
- [Get organization by identifier](https://fhir.villagecare.org/Organization?identifier=1023024882)
- [Get organizations by address AND type](https://fhir.villagecare.org/Organization?address=BRONX&type=HS)


##OrganizationAffiliation

OrganizationAffiliation is a central entity for an organization. It means that this entity contains info about organization, network, location, and healthcareService. You can use OrganizationAffiliation to search organization in the selected network:

1. [Get OrganizationAffiliation by network](https://fhir.villagecare.org/OrganizationAffiliation?organizationNetwork=MLTC)	
2. Get Organization Fhir ID from the OrganizationAffiliation entity
```json	
"organization": {
     "id": "22d99f7c-4dc6-46da-b5f8-1371f6ae8a53",
     "resource": {
		...
     },
     "resourceType": "Organization"
}
```		
3. [Get Organization by Fhir ID](https://fhir.villagecare.org/Organization?id=22d99f7c-4dc6-46da-b5f8-1371f6ae8a53)

####Advanced OrganizationAffiliation Queries

Also OrganizationAffiliation entity is used to get all FHIR entities connected with an organization in one query. These queries can use multiple search parameters and you can include, exclude and combine them. Also you can control what entities will be returned by including and excluding entities from the _include parameter of these queries.

To add additional entities in the response, like Organization or HealthcareService you should use _include parameter, e.g.:

- [Get OrganizationAffiliation and Organization entities](https://fhir.villagecare.org/OrganizationAffiliation?_include=OrganizationAffiliation:organization)	
- [Get OrganizationAffiliation with Organization and HealthcareService entities](https://fhir.villagecare.org/OrganizationAffiliation?_include=OrganizationAffiliation:organization,OrganizationAffiliation:service)
- [Get OrganizationAffiliation with all entities](https://fhir.villagecare.org/OrganizationAffiliation?_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service)

Also you can use these search parameters:	
	
- organizationName - organization name
- organizationNetwork - organization network code
- organizationType - full organization type name
- organizationSpecialty - full organization specialty name
- organizationSpecialtyCode - organization specialty code
- organizationTypeCode - organization type code


Advanced OrganizationAffiliation queries examples:

- [Get by organization name](https://fhir.villagecare.org/OrganizationAffiliation?_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationName=ALWAYS%20HOME%20CARE%20INC)
- [Get by network code and organization specialty](https://fhir.villagecare.org/OrganizationAffiliation?_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationNetwork=MLTC&organizationSpecialty=HOME%20HEALTH%20AIDE)
- [Get by all search parameters](https://fhir.villagecare.org/OrganizationAffiliation?_include=OrganizationAffiliation:organization,OrganizationAffiliation:network,OrganizationAffiliation:location,OrganizationAffiliation:service&organizationName=ALWAYS%20HOME%20CARE%20INC&organizationNetwork=MLTC&organizationType=ANCILLARY&organizationSpecialty=HOME%20HEALTH%20AIDE&organizationTypeCode=AN&organizationSpecialtyCode=66801)