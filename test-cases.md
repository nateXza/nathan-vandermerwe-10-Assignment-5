# Test Cases  

## Functional Tests  
| Test Case ID | Requirement ID | Description | Steps | Expected Result |  
|--------------|----------------|-------------|-------|------------------|  
| TC-001 | FR-001 | Upload Valid Image | 1. Log in. 2. Upload JPG image. | Prediction displayed in ≤5 sec. |  
| TC-002 | FR-003 | View Treatment Recommendations | 1. View prediction. 2. Click "Recommendations." | List of treatments with resource links. |  
| TC-003 | FR-005 | Critical Disease Alert | 1. Upload critical disease image. | Expert notified via email. |  

## Non-Functional Tests  
**Performance Test**:  
- Simulate 500 concurrent image uploads.  
- **Expected**: 95% processed within 10 seconds.  

**Security Test**:  
- Unauthorized user attempts to access reports.  
- **Expected**: System blocks access.  
