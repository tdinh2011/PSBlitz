# PSBlitz
Since I'm a big fan of [Brent Ozar's](https://www.brentozar.com/) [SQL Server First Responder Kit](https://github.com/BrentOzarULTD/SQL-Server-First-Responder-Kit) and I've found myself in many situations where I would have liked a quick way to easily export the output of sp_Blitz, sp_BlitzCache, sp_BlitzFirst, sp_BlitzIndex, sp_BlitzLock, and sp_BlitzWho, to Excel and saving to disk execution plans identified by sp_BlitzCache and deadlock graphs from sp_BlitzLock, I've decided to put together a PowerShell script that does just that.

## What it does

## What it runs

## Paramaters
| Parameter | Function|
-----------------------
-ServerName - accepts either [hostname]\[instance] (for named instances) or just [hostname] for default instances
-SQLLogin   - the name of the SQL login used to run the script; if not provided, the script will use integrated security
-SQLPass    - the password for the SQL login provided via the -SQLLogin parameter, omit if -SQLLogin was not used
-IsIndepth  - Y will run a more in-depth check against the instance/database, omit for a basic check
-CheckDB    - used to provide the name of a specific database to run some of the checks against, omit to run against the whole instance

## Default check vs. in-depth check

