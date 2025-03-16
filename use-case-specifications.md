 
Detailed specifications for critical use cases.  
  

# Use Case Specifications  

## 1. Upload Crop Image  
**Actor**: Farmer  
**Precondition**: Farmer is logged in; device has internet connectivity.  
**Postcondition**: Image processed, prediction displayed.  
**Basic Flow**:  
1. Farmer clicks "Upload Image."  
2. System validates image format (JPG/PNG).  
3. Image sent to CNN model for analysis.  
4. Prediction displayed with confidence score.  

**Alternative Flows**:  
- **Invalid Format**: System rejects upload and prompts for valid file.  
- **Processing Error**: System notifies farmer and logs the issue.  

## 2. View Disease Prediction  
**Actor**: Farmer  
**Precondition**: Image uploaded and validated.  
**Postcondition**: Prediction result stored in database.  
**Basic Flow**:  
1. System processes image using CNN.  
2. Displays disease name, confidence score, and treatment options.  
3. Farmer acknowledges result.  

**Alternative Flow**:  
- **Critical Disease Detected**: System alerts Agricultural Expert automatically.  
