## Requirements Table
Building tables to support managing system development is a key approach to staying organized. Just as a tool chest and the tools it holds need to be kept in a organized state so does information about game rules, Commercial Off The Shelf (COTS) parts used, etc need to be kept digitally / virtually organized. It can be helpful to summarized a rule, give it a category, cite its identifier, cite its page number, cite a document / file name, and track if it is being met. 

In the real world this information will come from multiple documents, some might be contract based from a customer (they aren't going to buy if the system cannot do X), some might be regulatory based due to the end used (for example a medical device), some might be regulatory based due a shipping method (for example shipping lithium batteries to get your product to the customer), some might be environmental (the customer plans on using the device in the rain), and some might be from a component you plan to use (for example this sensor must be mounted in a specific orientation). Not all of these will be listed in a document there are often items which are driven from the objective. For example the user anticipates using it in the rain, but they didn't specify what ingress protection rating would be appropriate as they don't know enough about that aspect of the solution. 

The objective is to:
1. Provide a short & quick to read summary of the requirement.
2. Provide a way to look up the full context of the requirement. 

### Example of Requirements Table
| ID No. | Type | Requirement | Ref / Source | Page No. | Meet (Yes / No) |
| --- | --- | --- | --- | --- | --- |
| 1 | Size | Max size (LxWxH) to be 28 in x 30 in x 40 in | 2.3.4 | 10 | Y |
| 2 | Weight | Total max mass including payload to be 5 kg | 12.2.1 | 20 | Y |
| 3 | Power | May have no more than 2x 12v batteries | 2.2.3 | 9 | N |
| 4 | Power | Battery chemistry to be nonspillable lead acid | 2.2.4 | 9 | Y |
| 5 | Motors | No more than 5 motors | 4.2.1 | 15 | N |
| 6 | Budget | BoM for  COTS  parts to total no more than $500.00 | 2.5.1 | 12 | Y |
| 7 | Size | System can expand up to 4 in on a single side. | 2.3.5 | 11 | Y |
| 8 | Power | System must run for 15 minutes. | 1.10.1 | 3 | N |

### Example Files 
- [ODS](RequirementsTable.ods)
- [CSV](RequirementsTable.csv)
