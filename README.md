# PostgreSQL Backup, Recovery and Streaming Replication Lab

## Project Overview

This project demonstrates practical PostgreSQL database administration skills using PostgreSQL 18.6 and the command-line interface (CLI).

The lab covers five important database backup, recovery and replication activities.

## Practical Activities Completed

### 1. Logical Backup and Restore
- Created a PostgreSQL database named `bootcamp`.
- Created and populated a `students` table.
- Used `pg_dump` to create a logical backup.
- Used `pg_restore` to restore the database.
- Verified the restored records.

### 2. WAL Archiving
- Configured `wal_level` to `replica`.
- Enabled `archive_mode`.
- Configured the `archive_command`.
- Verified successful WAL archiving.

### 3. Physical Base Backup
- Used `pg_basebackup` to create a physical database backup.
- Verified the backup directory and database files.

### 4. Point-in-Time Recovery (PITR)
- Recorded a recovery target timestamp.
- Simulated accidental data deletion.
- Configured recovery using archived WAL files.
- Recovered the database to the selected timestamp.
- Verified that the original five student records were restored.

### 5. Streaming Replication
- Created a replication user.
- Configured PostgreSQL authentication.
- Created a standby server using `pg_basebackup`.
- Configured the standby on port `5433`.
- Verified streaming replication from the primary server on port `5432`.
- Inserted a test record on the primary and confirmed that it appeared on the standby.

## Technologies Used

- PostgreSQL 18.6
- SQL
- PostgreSQL Command Line Tools
- Windows PowerShell
- Git and GitHub

## Project Outcome

All five practical activities were completed successfully. The final streaming replication test confirmed that data inserted into the primary database was successfully replicated to the standby server.

## Evidence

Screenshots of the commands, configurations and verification results are provided in the `screenshots` folder.

## Author

Bhan Gatdet Pal
