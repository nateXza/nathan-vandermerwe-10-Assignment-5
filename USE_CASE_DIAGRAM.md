```mermaid
graph TD
    A[Farmer] -->|Upload Image| UC1[Upload Image for Analysis]
    A -->|View Prediction| UC2[View Disease Prediction]
    A -->|Generate Report| UC3[Generate PDF Report]
    B[Agricultural Officer] -->|Validate Results| UC4[Validate Prediction Accuracy]
    C[Researcher] -->|Download Dataset| UC5[Access Anonymized Dataset]
    D[Government Agency] -->|Monitor Outbreaks| UC6[View Disease Heatmap]
    E[IT Team] -->|Retrain Model| UC7[Update Model with New Data]
    F[System Admin] -->|Manage Users| UC8[Add/Remove Users]
    
    UC1 --> UC2
    UC2 --> UC3
    UC4 -->|Data Validation| UC6
    UC5 -->|Updated Data| UC7
```


Explanation
Actors
Farmer: Primary user who interacts with disease prediction and recommendations.

Agricultural Expert: Validates predictions and updates the disease database.

System Admin: Manages user accounts and generates reports.

Relationships
Process Image via CNN is included in View Disease Prediction.

Notify Expert if Critical extends View Disease Prediction for urgent cases.

Stakeholder Alignment
Ensures real-time disease detection aligns with farmers' needs.

Supports experts in maintaining accurate disease data.
