# RealTimeReddDewatering
Code to automate a dewatering report
Files needed for this script include:

 * Shallow redd dewatering estimates from CDFW Upper Sacramento River Basin Salmonid Monitoring (calfish.org),
 * Dates and KES flows for proposed alternative flow regimes,
 * Real time KES flow data to date available from [SacPAS](https://www.cbr.washington.edu/sacramento/tmp/riverinventoryyears_1662742689_602.html) or [USBR](https://www.usbr.gov/mp/cvo/vungvari/sactemprpt.pdf)
  
To run this script:

 * Step 1: Save each Excel spreadsheet as a .csv file in the working directory (currently I:/Lisa/Redd Dewatering/Real-time Estimates), with dates [//]: in %m/%d/%Y format:,
    + Redds.csv (3 columns: Estimated.Date.of.Emergence, Status, & ACTUAL.or.ESTIMATED..DEWATER.FLOW) #note that column names may need to be edited
    + kesFlow.csv (no. columns = 1 + no. alternatives:  Date,  AltN...n) #again, note that column names may need to be edited
    + realFlow.csv (2 columns: Date & KES_Flow)

 * Step 2: Add the most recent redd count and date of count, and date of latest emergence/dewatering data to line first chunk of r code (above). Count and date are found on the Reports sheet of YYYY_WR_INTERNET_CARCASS-REDDS_counts_as_of_m-dd-yy.xlsx file on [calfish.org](https://gcc02.safelinks.protection.outlook.com/?url=https%3A%2F%2Fwww.calfish.org%2FProgramsData%2FConservationandManagement%2FCentralValleyMonitoring%2FCDFWUpperSacRiverBasinSalmonidMonitoring.aspx&data=05%7C01%7Clelliott%40usbr.gov%7C689ebb9a6c8243b4f96c08da90f5c542%7C0693b5ba4b184d7b9341f32f400a5494%7C0%7C0%7C637981682646098788%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C3000%7C%7C%7C&sdata=A1eQkWPxbkXxnzEvc2K8%2FTmslZ8H8zvxdks3%2F78Yrvw%3D&reserved=0),

* Step 3: Knit script: When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. ##AT THE MOMENT THE KNIT OPTION MAY NOT WORK TO PDF. IT WILL WORK TO KNIT TO AN HTML BUT DO NOT PUBLISH THE HTML YET PLEASE. PRINTSCREEN TO CREATE A PDF.
