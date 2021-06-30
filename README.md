## Branch bugbash-4

#### Test Case:

This branch contains a single valid ARM template for a scheduled analytics rule, inside the Templates folder:
1. ValidAnalyticsRule.json

#### Testing instructions

- Create the connection for branch `bugbash-4` on the target sentinel workspace
- Upon a successful connection - wait for the action to trigger

#### Expected Result:
- The Workflow should result in Success, however the rule should not get deployed 

#### Further Testing
Rename the `Templates` folder to `Detections` (no need to clone to your local machine, you can edit directly on github), and click commit changes.
After commiting the change, wait for the action to finish successfully and make sure the rule exists in the analytics gallery 