# Project Proposal

## Overview
A solution to replace the manual claims process that the AP Department currently uses.

## Objectives
* Handle user sessions and acquire account information from Active Directory
* Determine the distance between travel points for Mileage Claims and calculate the amount to be reimbursed based on said distance and mode of transport.
* Export the relevant data out into an Excel Stylesheet at the end of the month to be inserted into SAP, and eventually Oracle.
* Hide/show information based on user's role or level of access.
* Track if the approved budget for overseas travel has been exceeded in Pre-Approval & Cash Advance.

## Scope
List of forms to be digitalized:
* Pre-Approval & Cash Advance
* Expense Claims (Expense, Mileage, Meal Allowance)
* Marriage, Newborn & Funeral
* Lost Receipt Declaration

## Proposed Solution
A Claims system which utilizes a web interface to interact with end users. The system should also keep track of the progress of claims which are still open, notify and acquire approvals from relevant individuals as the forms progress down their respective information flow. The system should also have a dashboard for the users to track the progress of the claims they have submitted. The solution would also include an interface for administrators to assist with day to day management. The administrator interface would allow for slight changes in configurations. For instance, the administrator would be able to replace a designated recepient for another. 

Since Rapid4 cannot accomplish all of the objectives, the proposed solution will be built from scratch.

## Project Budget
To acquire the distance between two locations, the solution will use Google Maps' [Distance Matrix API](https://developers.google.com/maps/documentation/distance-matrix/start). Google provides us with $200 in monthly credit. With the free credit, the system can make the first 40,000 calls to this API for free and it costs $5 for each subsequent thousandth call. More information on its pricing structure can be found [here](https://cloud.google.com/maps-platform/pricing/sheet/#routes).

Optionally, we could also use Google Maps' [Places Autocomplete API](https://developers.google.com/maps/documentation/javascript/places-autocomplete) to assist with form completion and provide more accurate data to the Distance Matrix API. However, it should be noted that this API is quite expensive and would utilize the same pool of free credit Google provides us with monthly. It costs $2.83 per 100,000 characters. More information on its pricing structure can be found [here](https://cloud.google.com/maps-platform/pricing/sheet/#places).

## Information Flow
### Pre-Approval & Cash Advance
![Flow Chart](https://raw.githubusercontent.com/vinda-ykaseng/ExpenseClaims/master/flowcharts/Pre-Approval%20%26%20Cash%20Advance.png "Pre-Approval & Cash Advance Information Flow Chart")


### Expense Claim
![Flow Chart](https://raw.githubusercontent.com/vinda-ykaseng/ExpenseClaims/master/flowcharts/Expense%20Claim.png "Expense Claim Information Flow Chart")

### Marriage, Newborn & Funeral
![Flow Chart](https://raw.githubusercontent.com/vinda-ykaseng/ExpenseClaims/master/flowcharts/Marriage%2C%20Newborn%20%26%20Funeral.png "Marriage, Newborn & Funeral Information Flow Chart")
                            

## Timeframe
| Deliverable                                       | Estimate Completion Date  |
| ------------------------------------------------- | ------------------------- |
| Pre-Approval & Cash Advance (working prototype)   | 24th August, 2018         |
| Expense Claims              (working prototype)   | 28th August, 2018         |
| Marriage, Newborn & Funeral (working prototype)   | 28th August, 2018         |
| Lost Receipt Declaration    (working prototype)   | 28th August, 2018         |

___

## Key Stakeholders
* Fatim Hamimi
* Yeong Kok Soon