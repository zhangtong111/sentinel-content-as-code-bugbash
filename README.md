## Branch bugbash-2

#### Test Case:

This branch contains a single ARM template for a workbook:
1. workbook.json

#### Testing instructions

- Create the connection for branch `bugbash-3` on the target sentinel workspace
- Upon a successful connection - wait for the action to trigger

#### Expected Result:
- The Workflow should result in Failure, and the workbook should not get deployed