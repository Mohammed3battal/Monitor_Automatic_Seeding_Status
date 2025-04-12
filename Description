## Script: Monitor Automatic Seeding Progress

**Description**:
This script retrieves real-time stats from `sys.dm_hadr_physical_seeding_stats`, showing the progress of **automatic seeding** in Always On Availability Groups. It includes transfer rates, estimated size, duration, and compression status.

**Columns Explained**:
- `local_database_name`: Name of the database being seeded
- `remote_machine_name`: The partner server participating in seeding
- `role_desc`: Whether the local replica is Primary or Secondary
- `internal_state_desc`: Current seeding state
- `transfer_rate_MB_per_second`: Current data transfer speed
- `transferred_size_MB`: Amount of data already transferred
- `database_size_GB`: Total size of the database
- `is_compression_enabled`: Whether compression is being used
- `start_time`: Local start time of the seeding process
- `estimate_time_complete`: Estimated completion time (converted to local time)

**Use Case**:
Use this script to track live automatic seeding status and performance during AG setup or re-seeding events.

**Requirements**:
- SQL Server 2016 or later
- Always On AG must be configured
- `VIEW SERVER STATE` permission
