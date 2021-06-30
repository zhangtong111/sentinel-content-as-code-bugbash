## Branch bugbash-2

#### Test Case:

This branch contains 2 valid alert rules and 1 invalid rule in the detections folder:
![content1](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-2/Images/bb2-content.png)

#### Testing instructions

- Create the connection for branch `bugbash-2` on the target sentinel workspace
![content2](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-2/Images/bb2-connect.png)

- Upon a successful connection - wait for the action to trigger
![content3](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-2/Images/running.png)

#### Expected Result:
- The Workflow should result in Failure, with a message: *1 of 3 deploymets failed*
![content4](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-2/Images/failed.png)

- When the workflow finishes, navigate to your analytics blade and verify the 2 valid rules are there
![content5](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-2/Images/rules2of3.png)

#### For further testing: 
- Fix the invalid rule by changing the query from `BAD QUERY` to `SecurityAlert | take 10` (no need to clone to your local machine, you can edit directly on github), and click **commit changes**.
![content6](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-2/Images/edit.png)

- Once you commit, verify the workflow is executed and finishes with success, and make sure the fixed rule exists in the analytics gallery 