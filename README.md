## Recon_website
Description of what the recon website is 

Remember that Martin works on the catches, Miel works on the taxon extents. 

allocation tables go to v_fact tables to integrate them altogether. 

When allocating catches are put into marine layers. I believe they do this by using the simple
area cell assignment 

Simple area cell assignment is used in the allocation. 

In the recon website, you will only check the distribution tab to check for 
how the extents look. 

You can search using taxon key, common name or scientific name. All the information in recon website is in Prod sau int.
Any information entered into the recon website will automatically 
show up in the Prod sau int database in Dbeaver

To check the extents click view distribution or extent. 



### How the data cycles in databases during allocation
Allocation run goes: Prod sau_int --> Merlin --> QA sau --> Prod sau
Merlin doesn't use the tables in Prod sau (web). It is a copy of QA sau, Martin verified.



### Where to get the latest updated catches 
You can find this in QA sau. 
QA sau.v_fact_table if you need only all the catches without the cells.
QA sau.cell_catch if you need all the catches along with the cells. 
Martin talked about the area table. This table I presume contains the area in m2 of the half degree cells. 



### About the price table: The case of Robin Gutting map request asking initially for 
### price per cell

I was only able to give Robin the catch sum per cell in her area of interest. She did 
ask about the 'real value for 2010' but prices in SAU are still being worked on. There is 
a price per species and this changes per year (e.g. $1 for taxon key 1111). The price 
changes also depending on the end use (end use e.g. discards). So if you have 4,000 tonnes 
for this cell you can multiply that with the base price for that species. But like I said 
this is still in the works.


## Discussion on what to do with the taxon records 
You have to create the following: 
### Genera list 
        The genera list consists of species less than 10,000 tonnes over a period of 67 years.
        or a total of 67 years of catch. All species less than 10,000 tonnes are included in the 
        Genera list. 
        
        For the genera prioritize those which have a higher catch but less number of species in them. 

### Species list 
        The species list consist of greater than or equal to (>=) 10,000 tonnes. You will get this 
        queried and create this. All species >=10,000 tonnes will need to be shown as species extent.

### Family 
        The family list consists of exploited species. Check the DB and look for the importance field. 
        Take all which are tagged as 'commercial'. This list from FB and SLB will be synced with the one in 
        SAU. You take only those which SAU has. If it occurs in SAU then prioritize that. 
 
 ### For those without AquaMaps
  We will set aside the list which do not have AquaMaps and make sure by next year this will have maps then. 
  The distribution and all the information needed for an AquaMaps to be created should be done so that it can 
  be run. These will be bumped up to the Genus level if it doesn't have extents yet. 
  You have to make a table to show which species need to be completed. 
  
  ### Creation of tracking sheets 
  This will need to be submitted to MLDP on a monthly basis. How the distribution is coming along. Which one has extents, which has 
  none, which needs to be completed for AquaMaps generation, which has already AquaMaps. 
 
 ### By the way the checking of the taxon extents should be done before the 2018 allocation run 
 the 2018 allocation run will be done in April so everything should be in before the mid March 
 so that Miel will have time to work on the extents. The taxon extent need to be checked. This came up because of the 
 gaps in Exocoetidae extent. It has missing distribution in the Atlantic parts. The map is not from Aquamaps 
 and is not updated. So all extents need to be updated.  
 
 ### AquaMaps 
 Learn to program so you can shadow Nina. By October onwards there will be no Minderoo or big 
 deliverables.  
 Beth and Armi expected to learn the AquaMaps process. 
 
 
