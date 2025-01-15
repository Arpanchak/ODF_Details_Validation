# ODF Validation Automation Script
## Disclaimer
This code will only work if:
- Ceph health is **OK**
- StorageCluster is in a **Ready** state
## Overview
This script automates the validation steps for ODF (OpenShift Data Foundation), ensuring a comprehensive check of the cluster’s health and configuration. 
### Automated Validation Steps:
1. **Cluster Details Check** 
   - Verifies general cluster information.
2. **Node Check-up** 
   - Ensures all nodes are in a healthy and ready state.
3. **Version Check-up** 
   - Confirms that the installed ODF version matches expectations.
4. **Pods Check-up** 
   - Checks the status of all relevant pods.
5. **Ceph Health Check-up** 
   - Validates that the Ceph cluster is healthy (status: **OK**).
6. **Storage Cluster Check-up** 
   - Ensures that the StorageCluster is in a **Ready** state.
7. **Ceph Image Check-up** 
   - Validates the ceph image used for monitoring.
8. **CSV (Cluster Service Version) Check-up** 
   - Confirms that the Cluster Service Version is deployed and healthy.
9. **PV Status Check** 
   - Checks the PV status.
10. **PVC (Persistent Volume Claim) Status Check** 
    - Verifies that all Persistent Volume Claims are bound and healthy.
11. **NooBaa Status Check** 
    - Ensures the NooBaa service and resources are functional.
---
## Prerequisites
- Ensure that the ODF cluster is installed and configured.
- Verify that the Ceph health is **OK**.
- Confirm that the StorageCluster is in a **Ready** state.
---
## How to Use
1. Clone the repository:
  -  git clone https://github.com/Arpanchak/ODF_Details_Validation.git
2. Go into this folder:
  -  cd ODF_Details_Validation
3. Run this command:
  -  bash cluster_validation.sh
