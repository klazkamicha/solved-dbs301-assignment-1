Download Link: https://assignmentchef.com/product/solved-dbs301-assignment-1
<br>
<ol>

 <li>Display the employee number, full employee name, job and hire date of all employees hired in May or November of any year, with the most recently hired employees displayed first.

  <ul>

   <li>Also, exclude people hired in 2015 and 2016.</li>

   <li>Full name should be in the form “Lastname, Firstname”  with an alias called “Full Name”.</li>

   <li>Hire date should point to the last day in May or November of that year (NOT to the exact day) and be in the form of [May 31&lt;st,nd,rd,th&gt; of 2016] with the heading Start Date. <strong><em>Do NOT use LIKE operator. </em></strong></li>

   <li>&lt;st,nd,rd,th&gt; means days that end in a 1, should have “st”, days that end in a 2 should have “nd”, days that end in a 3 should have “rd” and all others should have “th”</li>

   <li>You should display ONE row per output line by limiting the width of the Full Name to 25 characters. The output lines should look like this line (4 columns):</li>

  </ul></li>

</ol>

<table>

 <tbody>

  <tr>

   <td width="129">174</td>

   <td width="131">Abel, Ellen</td>

   <td width="78">SA_REP</td>

   <td width="189">[May 31st of 2016]</td>

  </tr>

 </tbody>

</table>




<ol start="2">

 <li>List the employee number, full name, job and the modified salary for all employees whose monthly earning (without this increase) is outside the range $6,000 – $11,000 and who are employed as Vice Presidents or Managers (President is not counted here).

  <ul>

   <li>You should use Wild Card characters for this.</li>

   <li>VP’s will get 25% and managers 18% salary increase.</li>

   <li>Sort the output by the top salaries (before this increase) firstly.</li>

   <li>Heading will be like Employees with increased Pay</li>

   <li>The output lines should look like this sample line (note: 1 column):</li>

  </ul></li>

</ol>

Emp# 124 named Kevin Mourgos who is ST_MAN will have a new salary of $6960

<ol start="3">

 <li>Display the employee last name, salary, job title and manager# of all employees not earning a commission OR if they work in the SALES department, but only if their total monthly salary with $1000 included bonus and  commission (if  earned) is  greater  than  $15,000.

  <ul>

   <li>Let’s assume that all employees receive this bonus.</li>

   <li>If an employee does not have a manager, then display the word NONE</li>

   <li>This column should have an alias Manager#.</li>

   <li>Display the Total annual salary as well in the form of $135,600.00 with the</li>

   <li>heading Total Income. Sort the result so that best paid employees are shown first.</li>

   <li>The output lines should look like this sample line (5 columns):</li>

  </ul></li>

</ol>

<table>

 <tbody>

  <tr>

   <td width="107">De Haan</td>

   <td width="110">17000</td>

   <td width="96">AD_VP</td>

   <td width="94">100</td>

   <td width="120">$216,000.00</td>

  </tr>

 </tbody>

</table>




<ol start="4">

 <li>Display Department_id, Job_id and the Lowest salary for this combination under the alias Lowest Dept/Job Pay, but only if that Lowest Pay falls in the range $6000 – $17000. Exclude people who work as some kind of Representative job from this query and departments IT and SALES as well.

  <ul>

   <li>Sort the output according to the Department_id and then by Job_id.</li>

   <li>You MUST <strong>NOT </strong>use the Subquery method.</li>

  </ul></li>

 <li>Display last_name, salary and job for all employees who earn more than all lowest paid employees per department outside the US locations.

  <ul>

   <li>Exclude President and Vice Presidents from this query.</li>

   <li>Sort the output by job title ascending.</li>

   <li>You need to use a Subquery and Joining.</li>

  </ul></li>

 <li>Who are the employees (show last_name, salary and job) who work either in IT or MARKETING department and earn more than the worst paid person in the ACCOUNTING department.

  <ul>

   <li>Sort the output by the last name alphabetically.</li>

   <li>You need to use ONLY the Subquery method (NO joins allowed).</li>

  </ul></li>

 <li>Display alphabetically the full name, job, salary (formatted as a currency amount incl. thousand separator, but no decimals) and department number for each employee who earns less than the best paid unionized employee (i.e. not the president nor any manager nor any VP), and who work in either SALES or MARKETING department.

  <ul>

   <li>Full name should be displayed as Firstname Lastname and should have the heading Employee.</li>

   <li>Salary should be left-padded with the = symbol till the width of 15 characters. It should have an alias Salary.</li>

   <li>You should display ONE row per output line by limiting the width of the Employee to 25 characters.</li>

   <li>The output lines should look like this sample line (4 columns):</li>

  </ul></li>

</ol>

<table width="566">

 <tbody>

  <tr>

   <td width="169">Jonathon Taylor</td>

   <td width="116">SA_REP</td>

   <td width="229">=======  $8,600</td>

   <td width="51">80</td>

  </tr>

 </tbody>

</table>




<ol start="8">

 <li>“Tricky One”Display department name, city and number of different jobs in each department. If city is null, you should print Not Assigned Yet.

  <ul>

   <li>This column should have alias City.</li>

   <li>Column that shows # of different jobs in a department should have the heading # of Jobs</li>

   <li>You should display ONE row per output line by limiting the width of the City to 24 characters.</li>

   <li>You need to show complete situation from the EMPLOYEE point of view, meaning include also employees who work for NO department (but do NOT display empty departments) and from the CITY point of view meaning you need to display all cities without departments as well.</li>

  </ul></li>

</ol>