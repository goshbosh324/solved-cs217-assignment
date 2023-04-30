Download Link: https://assignmentchef.com/product/solved-cs217-assignment
<br>
<ul>

 <li>The dashboard is based on aggregated data of the Covid 19 cases transmitted to the RKI by the health authorities in accordance with the IfSG</li>

 <li>The current status (00:00) is displayed with the data and the changes in cases and deaths from the previous day are displayed</li>

 <li>The data source contains the following parameters:</li>

</ul>

<table width="540">

 <tbody>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Object_Id</strong></td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>State_Id</strong>: Id of the federal state of the case with 1 = Schleswig-Holstein to 16 = Thuringia</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>State</strong>: Name of the federal state</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>District</strong>: Name of the district</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Age_Group</strong>: Age group of the case from the 6 group 0-4, 5-14, 15-34, 35-59, 60-79, 80+ and unknown</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Sex</strong>: Gender of the case M0 male, W = female and unknown</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Number_of_Cases</strong>: Number of cases in the corresponding group</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Number_of_deaths</strong>: Number of deaths in the corresponding group</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Reporting_date</strong>: the date when the health department became aware of the case</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>District_Id</strong>: ID of the district of the case in the usual coding 1001 to 16077 = LK Altenburger Land</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Last_Updated</strong>: Date when the data record was last updated</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>New_Case</strong>:&#x25aa;       0: Case is included in the publication for the current day and in the one for the previous day&#x25aa;      1: Case is only included in the current publication&#x25aa;       -1: Case is only included in the previous day’s publication&#x25aa;       This results in: number of cases in the current publication as a sum (number of cases), if new case in (0.1); Delta on the previous day as the sum (number of cases) if new case in (-1.1)</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>New_Death</strong>:&#x25aa;       0: The case is one death in the publication for the current day and in the one for the previous day&#x25aa;       1: The case is a death in the current publication, but not in the previous day’s publication&#x25aa;       -1: The case is not a death in the current publication, but it was a death in the previous day’s publication&#x25aa;       -9: The case is not a death in either the current publication or that of the previous day&#x25aa;       this results in: number of deaths in the current publication as a total (number of deaths) if new death in (0.1); Delta on the previous day as total (number of deaths) if new death in (-1.1)</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>Reference_Date</strong>: date of illness or, if this is not known, the reporting date</td>

  </tr>

  <tr>

   <td width="33">◦</td>

   <td width="506"><strong>New_Recovered</strong>:</td>

  </tr>

 </tbody>

</table>

1

&#x25aa;       0: The case is recovery in the publication for the current day and in the one for the previous day

&#x25aa;       1: Case is recovered in the current publication, but not in the previous day’s publication

&#x25aa;       -1: The case is not recovered in the current publication, but was recovered in the previous day’s publication

&#x25aa;       -9: The case is neither in the current publication nor in that of the previous day recovered

&#x25aa;       This results in: number of geneses of the current publication as the sum (number of geneses) if new geneses in (0.1); Delta on the previous day as sum (number of generations) if new generation in (-1.1)

◦ <strong>Number_of_recovered</strong>: Number of recovered in the corresponding group

◦ <strong>Disease_Onset</strong>: 1 if the reference date is the onset of illness, 0 otherwise

◦ <strong>Age-group2</strong>: Age group of the case from 5-year groups 0-4, 5-9, 10-14, …, 75-79, 80+ and unknown