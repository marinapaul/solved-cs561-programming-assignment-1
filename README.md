Download Link: https://assignmentchef.com/product/solved-cs561-programming-assignment-1
<br>
[pdf-embedder url="https://assignmentchef.com/wp-content/uploads/2022/12/file-7.pdf" title="file (7)"]

<strong><em>Objectives</em></strong> In this assignment, you will <em><u>express</u></em> “complex” OLAP queries in SQL. The key point of the

exercise is to observe the complexity of expressing the type of such queries despite relatively

simple ideas of the queries themselves. Your mission (in addition to writing the SQL queries) is to

consider the reasons for the complexity of the <em>expression</em> of these queries.

<strong><em>Description</em></strong> Generate 5 separate reports based on the following queries (one report for query #1, one for

query #2, one for query #3, one for query #4 and another for query #5):
<ol>
 	<li>For each <em>customer</em>, compute the <em><u>minimum</u></em> and <em><u>maximum</u></em> sales quantities along with the</li>
</ol>
<em><u>corresponding products</u></em> (purchased),<em> <u>dates</u></em> (i.e., dates of those minimum and maximum

sales quantities) and the occurrences of the min or max<em><u>states</u></em>, display all.in which the sale transaction s took place. If there are &gt;1

For the same <em>customer</em>, compute the <em><u>average</u></em> sales quantity.
<ol start="2">
 	<li>For <em>each of the 12</em> <em>months</em> (regardless of the year), find the <em><u>most “productive”</u></em> and <em><u>least</u> </em></li>
</ol>
<em><u>“</u></em>corresponding <em><u>productive”</u></em> <em><u>datotal sys</u></em> (those <em><u>ales quantities</u></em>days with most and least <em><u> (i.e., SUMs)</u></em>. total sales quantities) and the
<ol start="3">
 	<li>For each <em>product</em>, find the “<em><u>most favorable</u></em>” <em><u>month</u></em> (when most amount of the product was</li>
</ol>
sold) and the “<em><u>least favorable</u></em>” <em><u>month</u></em> (when the least amount of the product was sold).
<ol start="4">
 	<li>Show for each <em>customer</em> and <em>product</em> combination, the <em><u>average sales quantities for 4</u> </em></li>
</ol>
<em><u>quarters</u></em>, Q1, Q2, Q3 and Q4 (in four separate columns) – Q1 being the first 3 months of

the year (Jan, Feb &amp; Mar), Q2 the next 3 months (Apr, May &amp; Jun), and so on – ignore the

YEAR component of the dates (i.e., 3/11/2001 is considered the same date as 3/11/2002,

etc.). Also compute the <em><u>average for the “whole” year</u></em> (again ignoring the YEAR

component, meaning simply compute AVG) along with the <em><u>counts</u></em> (COUNT). <em><u>total quantities</u></em> (SUM) and the
<ol start="5">
 	<li>For each combination of <em>customer</em> and <em>product</em>, output the <em><u>maximum sales quantities for</u> </em></li>
</ol>
<em><u>NJ</u></em>,<em><u> NY and CT in 3 separate columns</u></em>. Like the first report, display the <em><u>corresponding</u> </em>

<em><u>dates</u></em> (i.e., dates of those corresponding maximum sales quantities). Furthermore, show

the output <em><u>only if maximum for NY is greater than NJ or CT</u></em>.

The following is a sample output – quantities displayed are for illustration only (not the actual

values). <strong><u>For dates (e.g., MAX_DATE, MIN_DATE), you can display ‘month’, ‘day’ and ‘year’</u> </strong>

<strong><u>as 3 separate columns – i.e., you don’t need to concatenate them into MM/DD/YYYY format.</u></strong>

<u>Report #1:</u>

CUSTOMER MIN_Q MIN_PROD MIN_DATE ST MAX_Q MAX_PROD MAX_DATE ST AVG_Q

======== ===== ======== ========== == ===== ======== ========== == =====

Bloom 12 Pepsi 01/01/2006 NJ 2893 Apple 09/25/2001 NY 1435

Sam 1 Milk 02/15/2002 NJ 259 Banana 03/23/2004 CT 56

Emily 2 Bread 07/01/2005 NY 3087 Milk 02/02/2001 NJ 1512

. . . .

<u>Report #2:</u>

MONTH MOST_PROFIT_DAY MOST_PROFIT_TOTAL_Q LEAST_PROFIT_DAY LEAST_PROFIT_TOTAL_Q

===== =============== =================== ================ ====================
<ul>
 	<li>12 497214 31 55526</li>
 	<li>23 1874794 15 23126 3 4 974531 2 19958</li>
</ul>
. . . .

<u>Report #3:</u>

PRODUCT MOST_FAV_MO LEAST_FAV_MO ======= =========== ============

Egg 4 12

Apple 1 11

Banana 3 2 . . . .

<u>Report #4:</u>

CUSTOMER PRODUCT Q1_AVG Q2_AVG Q3_AVG Q4_AVG AVERAGE TOTAL COUNT

======== ======= ====== ====== ====== ====== ======= ===== =====

Sam Pepsi 1923 4241 2383 1325 2988 38848 13

Emily Milk 239 9872 142 2435 2663 21307 8 Helen Bread 2534 981 4239 1987 2781 25032 9 . . . .

<u>Report #5:</u>

CUSTOMER PRODUCT NJ_MAX DATE NY_MAX DATE CT_MAX DATE

======== ======= ====== ========== ====== ========== ====== ==========

Sam Egg 7908 01/11/2001 2405 07/24/2005 1932 11/03/2008

Helen Cookies 392 03/31/2002 1042 09/14/2000 811 07/23/2002
<table>
<tbody>
<tr>
<td width="439"></td>
</tr>
<tr>
<td></td>
<td></td>
</tr>
</tbody>
</table>
Bloom Butter 1045 09/22/2003 2023 03/10/2004 2988 09/11/2006

<strong><em>Grading</em></strong> <strong><u>NOTE: A query with syntax errors will lose 50% of the points for the query</u></strong>.

<strong><em>Submission</em></strong> Submit a file containing all of the 5 queries or 5 separate files with each query in a separate file with your name and CWID on it on Canvas. If you create 5 separate files, please place them in a ZIP file and submit the ZIP file.

Please include a “README” file if any special instructions are required.

You can discuss the “ideas” with your class mates or your friends, but the final queries must be your own work. If I determine that your queries are copies of someone else’s, both you and that someone else will be disciplined (you will receive 0 for the entire assignment) and possibly receive additional penalties for the course.