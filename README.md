## Branch bugbash-2

#### Test Case:

This branch contains 3 valid alert rules in the detections folder:
1. Invalid-BadQuery.json
2. Valid-BuiltInFusion.json
3. Valid-SuccessfulSSHBruteForceAttack.json

#### Testing instructions

- Create the connection for branch `bugbash-2` on the target sentinel workspace
- Upon a successful connection - wait for the action to trigger

#### Expected Result:
- The Workflow should result in Failure, with a message saying 2 of 3 deploymets were successful
- When the workflow finishes, navigate to your analytics blade and verify the 2 valid rules are there

#### For further testing: 
- Fix the invalid rule by changing the query from `BAD QUERY` to `SecurityAlert | take 10` (no need to clone to your local machine, you can edit directly on github), and click **commit changes**.
- Once you commit, verify the workflow is executed and finishes with success