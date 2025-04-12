# Blackgate's Local Supabase Instance

This README provides instructions for deploying a local Supabase instance using Docker and loading tables via the SQL editor.

## Prerequisites

- Docker and Docker Compose installed on your system.
- `tableDef.sql` file containing the SQL query for table definitions.

## Deployment Instructions

1. **Clone the Supabase Docker Repository**  
    Clone the official Supabase Docker repository or set up your own Docker Compose file for Supabase.

    ```bash
    git clone https://github.com/supabase/supabase.git
    cd supabase/docker
    ```

2. **Start the Supabase Instance**  
    Run the following command to start the Supabase instance:

    ```bash
    docker-compose up -d
    ```

    This will start the Supabase services, including the database, API, and authentication.

3. **Access Supabase Locally**  
    Once the services are running, you can access the Supabase dashboard at `http://localhost:54323`.

## Loading Tables via SQL Editor

1. **Open the SQL Editor**  
    Navigate to the SQL editor in the Supabase dashboard.

2. **Load the `tableDef.sql` File**  
    Copy the contents of the `tableDef.sql` file into the SQL editor.

3. **Run the SQL Query**  
    Execute the SQL query to create the necessary tables in your local Supabase instance.

## Stopping the Supabase Instance

To stop the Supabase instance, run:

```bash
docker-compose down
```

## Additional Notes

- Ensure that port `54323` is not blocked by your firewall or used by another service.
- Modify the `docker-compose.yml` file if you need to customize the configuration.
