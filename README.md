# family_educ_impact

Project for Introduction to Data Science class.

Question to be answered:
- Will certain family factors affect their educational approaches?  (specific factors and outcomes TBD?)

Data to be used:
- Parent and Family Involvement in Education study from National Center for Education Statistics
- https://nces.ed.gov/nhes/dataproducts.asp

What do I know about the data so far?
- I have reviewed the Data File Users Manual - including the survey questions, and have noted some questions of interest.
- I have done an initial review of the data file - but not done any parsing of the data.

Why did I choose this topic?
- I have been working in the education sector for 25 years and am interested in education outcomes.  As a parent who has chosen
  to homeschool - I am also interested in how other families have chosen to approach education and how that is related to other family 
  factors - as well as educational and workforce outcomes.

----
8/18/17 Update
- Imported data from data/pfi_pu_pert_ascii.dat into a dataframe (notebooks/Test 1.ipynb)
- This is a fixed length file - so I tried using read_fwf() and having it derive the columns 
  from the data and see how well it guessed at things.
  - It did surprisingly well - but still only found 124 fields out of the 717 defined in the user guide (data/NCES_2012_UsersManual.pdf)
- So my next step is to define the fields I want to extract from the user guide in the read_fwf() and read those columns in and cross-check against the guide and file to determine if I am looking at the right fields.
- Then I will do some profiling of the fields and determine which ones look useful and might have some correlations.  Then determine some specific questions to model and investigate.

