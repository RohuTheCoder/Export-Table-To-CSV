# Export-Table-To-CSV
<p>Hi, in this tutorial I am going to show you how you can export PostgreSQL data to a CSV file.</p>
<p>To copy data out first connect to your PostgreSQL via tool like PGAdmin</p>
<img src="sample images/table.png" width="450">
<p>Using the query tool run the commands given below.</p>
<h4>COPY [Table Name] TO '[File Name]' DELIMITER ',' CSV HEADER;</h4>
<code><pre>COPY company_data TO 'C:\Users\Public\company_data.csv' DELIMITER ',' CSV HEADER;</pre></code>
<p>Besides exporting full tables you can also export the results of a query with the following format where [Query] and [File Name] are your query and output file name respectively.</p>
<h4>COPY ([Query]) TO '[File Name]' DELIMITER ',' CSV HEADER;</h4>
<code><pre>COPY (SELECT * FROM company_data;) TO C:\Users\Public\company_data.csv' DELIMITER ',' CSV HEADER;</pre></code>
<p>We have successfully exported PostgreSQL table to CSV file.</p>
<img src="sample images/csv.png" width="450">
