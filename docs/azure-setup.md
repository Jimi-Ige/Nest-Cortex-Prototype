## Ownership and Control
- All Azure resources for Nest Cortex are managed under `jimi@jimiige.com`.
- This ensures that Nest Cortex remains under personal ownership and can transition to the Nest Organization in the future.
- Role-based access will be granted to partner organizations (e.g., Nest and Rise, Inc.) as licensed users.
# Azure Data Lake Setup: Container Configuration

## Containers Created
1. **raw**
   - Purpose: Store unprocessed data such as intake forms and session logs.
   - Access Level: Private (no anonymous access).

2. **processed**
   - Purpose: Store cleaned and validated data.
   - Access Level: Private (no anonymous access).

3. **curated**
   - Purpose: Store dashboard-ready data and analytics.
   - Access Level: Private (no anonymous access).

## Steps to Create Containers
1. Navigate to **Containers** in the Azure Storage Account.
2. Click **+ Container** and configure:
   - Name: `raw`
   - Public Access Level: Private
   - Repeat for `processed` and `curated`.

## Testing the Setup
1. Verified containers by uploading a sample file to the `raw` container.
2. Checked file properties for successful upload and access control.

## Notes
- Hierarchical namespace enabled for folder-like structure in containers.
- Encryption enabled using Microsoft-managed keys.
