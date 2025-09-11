## Rando Mongo queries:

Find all records after a time stamp

```JavaScript
{createdAt: { $gt: ISODate('2021-05-08T11:54:32.097') }}
```

  

## Helpful JavaScript things

Just a pause in execution

```JavaScript
const wait = (timeToDelay) => new Promise((resolve) => {
  setTimeout(resolve, timeToDelay);
});

...

await wait(3000);
```

  

## Git commands

Local commands to run after changing "master" branch to "main" on GitHub

```Bash
git branch -m master main
git fetch origin
git branch -u origin/main main
git remote set-head origin -a
```

  

## Find top TCP connections on LiquidWeb server

Shell Command to find the top 10 TCP Connection IP sources. For good measure, the IP addresses can be checked on [https://www.abuseipdb.com/](https://www.abuseipdb.com/)

```Bash
[root@host ~]#  grep -r "03/Feb/2025" /var/www/vhosts//buffaloexchange.com/logs/access_ssl_log | awk '{print $1}'|cut -d':' -f1|sort |uniq -c|sort -n|tail -n10
    217 99.138.105.59
    230 66.249.65.237
    356 13.56.238.252
    414 35.88.87.248
    443 195.242.10.185
    577 66.249.65.236
    580 172.16.166.76
   1542 65.2.146.204
   1597 66.249.65.235
 390420 198.23.212.26 
```


## SQL query to insert new payroll scheduling emp roles
``` SQL
SELECT TOP (1000) [Id]
      ,[RowKey]
      ,[RowStatus]
      ,[SortOrder]
      ,[CreatedAt]
      ,[CreatedBy]
      ,[ModifiedAt]
      ,[ModifiedBy]
      ,[EmployeeType]
      ,[Name]
  FROM [BuffEx_PayrollSchedulingDB_Dev].[dbo].[EmployeeRole];


INSERT INTO [BuffEx_PayrollSchedulingDB_Dev].[dbo].[EmployeeRole] (Id, RowKey, RowStatus, SortOrder, CreatedAt, CreatedBy, ModifiedAt, ModifiedBy, EmployeeType, [Name])
values (NEWID(), 0, 0, 80, GETDATE(), 'Jeff Innes Via Direct DB Query', GETDATE(), 'Jeff Innes Via Direct DB Query', 80, 'GA F/T');

INSERT INTO [BuffEx_PayrollSchedulingDB_Dev].[dbo].[EmployeeRole] (Id, RowKey, RowStatus, SortOrder, CreatedAt, CreatedBy, ModifiedAt, ModifiedBy, EmployeeType, [Name])
values (NEWID(), 0, 0, 81, GETDATE(), 'Jeff Innes Via Direct DB Query', GETDATE(), 'Jeff Innes Via Direct DB Query', 81, 'GA P/T');
```


## SQL Query to pull all the SBM Open Orders and needed info

``` SQL
SELECT SBM_ORDER_ID,ORDER_STATUS,DATE_SENT,NUM_BAGS,BAGS_RECEIVED,
DISPOSITION,
PAY_TYPE,
PAYPAL_EMAIL,
SBM_FNAME,
SBM_LNAME,
SBM_ADDRESS,
SBM_APT,
SBM_CITY,
SBM_STATE,
SBM_ZIP,
SBM_PHONE,
SBM_EMAIL,
SBM_COMMENTS,
FIRST_NAME AS CEL_FNAME,
LAST_NAME AS CEL_LNAME,
ADDRESS1 AS CEL_ADDRESS,
ADDRESS2 AS CEL_APT,
CITY AS CEL_CITY,
[STATE] AS CEL_STATE,
ZIP AS CEL_ZIP,
PHONE1 AS CEL_PHONE,
[CELADDY].EMAIL1 AS CEL_EMAIL,
CASE
	WHEN IS_SMS_ENABLED = 1 THEN 'YES'
	ELSE 'NO'
END AS IS_SMS_ENABLED,
CEL_CUSTOMER_ID
FROM [SellByMail].[dbo].[TB_SBM_ORDERS] as O
LEFT JOIN [SellByMail].[dbo].[TB_SBM_ORDER_DETAIL] as OD ON O.SBM_ORDER_DETAIL_ID=OD.SBM_ORDER_DETAIL_ID
LEFT JOIN [SellByMail].[dbo].[TB_SBM_CUSTOMERS] as SBMC ON O.SBM_CUSTOMER_ID=SBMC.SBM_CUSTOMER_ID
LEFT JOIN [Celerant].[dbo].[TB_CUSTOMERS] as CELCUST ON SBMC.CEL_CUSTOMER_ID=CELCUST.CUSTOMER_ID
LEFT JOIN [Celerant].[dbo].[TB_CUST_ADDRESS] as CELCUSTADDY ON SBMC.CEL_CUSTOMER_ID=CELCUSTADDY.CUSTOMER_ID
LEFT JOIN [Celerant].[dbo].[TB_ADDRESS] as CELADDY ON CELCUSTADDY.ADDRESS_ID=CELADDY.ADDRESS_ID
WHERE CLOSED is NULL AND BAGS_SENT = 'Y';
```