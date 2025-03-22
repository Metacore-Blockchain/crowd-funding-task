
### CrowdFunding Smart Contract Functions 


This document provides a structured breakdown of the functions used in the crowdfunding smart contract. Each function is categorized based on its purpose and includes visibility, modifiers, parameters, and return types.

Note:
Implement code on remix and write hard copy of code as well.

1. startCampaign  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _name (string), _description (string), _goalAmount (uint256), _deadline (uint256)  
   - Returns: None  

2. cancelCampaign  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

3. pauseCampaign  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

4. resumeCampaign  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

5. extendDeadline  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256), _newDeadline (uint256)  
   - Returns: None  

6. updateCampaignMetadata  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256), _newDescription (string)  
   - Returns: None  

---

### Contribution Functions  

7. contribute  
   - Visibility: public  
   - Modifiers: payable  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

8. getContributorDetails  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256), _contributor (address)  
   - Returns: amountContributed (uint256)  

9. getTotalContributions  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256)  
   - Returns: totalContributed (uint256)  

---

### Fund Handling Functions  

10. withdrawFunds  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

11. claimFunds  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

12. refundContributors  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256)  
   - Returns: None  

13. ownerWithdrawFees  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256), _feeAmount (uint256)  
   - Returns: None  

---

### Campaign Status Functions  

14. setFundingGoal  
   - Visibility: public  
   - Modifiers: None  
   - Parameters: _campaignId (uint256), _goalAmount (uint256)  
   - Returns: None  

15. checkFundingStatus  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256)  
   - Returns: isFunded (bool)  

16. isCampaignSuccessful  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256)  
   - Returns: success (bool)  

17. getRemainingTime  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256)  
   - Returns: timeLeft (uint256)  

18. getCampaignDetails  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256)  
   - Returns: name (string), goal (uint256), raised (uint256), active (bool), deadline (uint256)  

19. getAllCampaigns  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: None  
   - Returns: campaigns (array of Campaign structs)  

20. getCampaignOwner  
   - Visibility: public  
   - Modifiers: view  
   - Parameters: _campaignId (uint256)  
   - Returns: owner (address)  
