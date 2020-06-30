# Zoho-Books-Linking-Invoice

## Overview
This custom function will create an additonal invoice based on the Event Date of a previous Invoice. Here are some details of how it works:
* The newly created invoice will be of the same amount as the primary invoice
* The Due Date of the newly created invoice will be 14 days before the *Event Date*, unless the event date is less that 14 days out, in which case the due date will be set to the current date.
* This will add a URL of the newly created Invoice on the primary Invoice, and the URL of the primary Invoice on the newly created Invoice.
* This will not work if the items on the Invoice are serialized.

## Setup
To make this custom function work, you will need to add two custom fields in Zoho Books:
* *Event Date* \[Date Type: Date\]
* *Linking Invoice* \[Data Type: URL\]


