# CMS_Psychiatric_Comorbidity_Lookup
A lookup tool that searches Medicare's list of Psychiatric Comorbidity Diagnosis Codes and returns an object

Since I only just started learnig Javascript less than two weeks ago, I decided to do something simple that I knew I personally 
would find useful in my day-to-day life in the hospital billing world. 

In the hospital billing world, how much a medical provider is paid for an inpatient Psychiatric stay is affected by whether or 
not a bill has a "Comorbidity Diagnisis Code" on it. How much this affects Medicare's payment is affected both by whether or not it 
is on the comorbidity code list and its type.

Long story short: This tool was designed so a provider can put in put in the diagnosis codes they billed and see if their payment 
from medicare will be affected by the codes billed. It searches the array and returns the code, its description, whether or not it's a
comorbidity code, and its type as an object as in the example below:

{ ICD_10_CM_DIAGNOSIS: 'F71',
  DESCRIPTOR: 'Moderate intellectual disabilities',
  Yes: 'Yes',
  Type: 'Developmnt Disabil' }

The array was downloaded as a spreadsheet publicly available on the Medicare website and was converted first to a csv, and 
then to a JSON file type. 
