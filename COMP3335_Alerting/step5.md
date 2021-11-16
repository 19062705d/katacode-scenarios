# Step 5: Setting up 2MySQL collector
After created the dashboard, we need to create the collector to collect the the information.

1. Open a new terminal. Download the script name as `my2_80.sql`.
`wget https://raw.githubusercontent.com/meob/my2Collector/master/my2_80.sql`

2. Copy the file to the container, you can also rename it.
`docker cp my2_80.sql mysql:/my2sql`

3. Return to the contailer bash and execute my2.sql by root user by using the password we set in step 1.
`docker exec -it mysql/bin/sh`
`mysql < my2.sql -uroot -p12345`

4. Login to MySQL to check the collector.
`mysql -uroot -p12345`
`show database;`
`use my2`
`show tables;`

5. You can study the container by using different command.
`select * from current;`

 
