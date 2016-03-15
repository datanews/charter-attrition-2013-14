# charter-attrition-2013-14
NYC charter school attrition, and average attrition for traditional public schools in each school district, for July 2013 through June 2014. Calculated from data received from the NYC Department Of Education in response to a FOIL request by WNYC.

Check out our [story and analysis here](http://www.wnyc.org/story/nyc-charter-school-attrition-rates/). 

### Fields
* `dbn`: school's District Borough Number, school code
* `schoolName`: name of school
* `network`: charter network, if any
* `district`: geographic school district

  ### for each group of grades [`K-4`, `6-7`, `9-11`]:
  * `[grades]discharge`: number of students in specified grades, who didn’t leave “same day” or in the first week of September after being admitted, transferring out of the school
  * `[grades]julyOct`: number of students in specified grades, who didn’t leave “same day” or in the first week of September after being admitted, transferring out of the school in July through October
  * `[grades]enrollment`: October 31, 2013 enrollment listed in NYC Department of Education's ["Demographic Snapshot" data](http://schools.nyc.gov/Accountability/data/default.htm) for those grades 
  * `[grades]adjustedEnrollment`: [grades]enrollment + [grades]julyOct
  * `[grades]attritionRate`: [grades]discharge / [grades]adjustedEnrollment
  * `[grades]district`: attrition rate at traditional public schools in the same district, for the same grades
