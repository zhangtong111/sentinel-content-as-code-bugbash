## Branch bugbash-1

#### Test Case:

This branch contains 3 valid alert rules in the detections folder:
![content](https://github.com/erant10/sentinel-content-as-code-bugbash/blob/bugbash-1/Images/bugbash1?raw=true)

#### Testing instructions

- Create the connection for branch `bugbash-1` on the target sentinel workspace
- Upon a successful connection - wait for the action to trigger

#### Expected Result:

- When the workflow finishes, navigate to your analytics blade and verify the 3 rules above are there

#### For further testing: 
- Make a small change in 1 of the rules on this branch (no need to clone to your local machine, you can edit directly on github), and click **commit changes**.
- Once you commit, verify the workflow is 