# Step 5: Setting up 2MySQL collector
After created the dashboard, we need to create the collector to collect the the information.

1. Open a new terminal. Download the script name as `my2_80.sql`.<br>
`wget https://raw.githubusercontent.com/meob/my2Collector/master/my2_80.sql`<br>

2. Copy the file to the container, you can also rename it.<br>
`docker cp my2_80.sql mysql:/my2sql`<br>

3. Return to the contailer bash and execute my2.sql by root user by using the password we set in step 1.<br>
`docker exec -it mysql/bin/sh`<br>
`mysql < my2.sql -uroot -p12345`<br>

4. Login to MySQL to check the collector.<br>
`mysql -uroot -p12345`<br>
`show database;`<br>
`use my2`<br>
`show tables;`<br>

5. You can study the container by using different command.<br>
`select * from current;`

 
