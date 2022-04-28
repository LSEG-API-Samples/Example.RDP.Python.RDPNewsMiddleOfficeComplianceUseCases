# Example.RDP.Python.MiddleOfficeComplianceUseCases

## Middle Office Compliance Use Case Code Samples

1. 	How a user can pass along a large list of CUSIP, ISIN and or SEDOLs and retrieve a company PermID | OrgName and status as an API response or as a bulk file
*Map2kSEDOLs_SymbologyDataLibEndpoint.ipynb and Map2kSEDOLs_SymbologyDataLibSearch.ipynb*
3. 	How a user can make a API Req/Res call for news:                                    *HeadlinesLast24HrsPermidsTopics_NewsRDPAPI.ipynb*

    a) Published in the last 24 hours, where
    
    b) The messages are tagged with PermIds (1, 2, 3, 4)
    
    c) And the messages contain topic codes (x, y or z) 
3.	How a user can make a streaming subscription for news (via AWS message queue):      *sqsQueueSubscribeNewsFiltered * 

    a) Where he messages are tagged with PermIds (1, 2, 3, 4)
     **
    b) And the messages contain topic codes (x, y or z)        
    
    c) And, how the user can pick up the messages from an SQS queue every 24 hours at time (HH:MM:SS) and then delete the messages from the SQS queue (the scheduling is to be handled separately via task scheduler)

