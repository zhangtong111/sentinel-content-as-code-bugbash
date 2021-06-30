## Branch bugbash-1

#### Test Case:

This branch contains 3 valid alert rules in the detections folder:
![content1](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-1/Images/bugbash1.png)

#### Testing instructions

- Create the connection for branch `bugbash-1` on the target sentinel workspace
![content2](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-1/Images/bb1-connect.png)

- Upon a successful connection - wait for the action to trigger
![content3](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-1/Images/running.png)

#### Expected Result:

- When the workflow finishes, navigate to your analytics blade and verify the 3 rules above are there
![content4](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-1/Images/3rules.png)

#### For further testing: 
- Make a small change in 1 of the rules on this branch (no need to clone to your local machine, you can edit directly on github):
    - open the file on github
    ![content5](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-1/Images/openfile.png)

    - click the pencil icon and make desired change on the template (e.g. set enabled to `false`)

    - click **commit changes**.
    ![content6](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-1/Images/confirmedit.png)

- Once you commit, verify the workflow is triggered 
- Make sure the workflow finishes running successfully, and return to the analytics gallery to verify your change has been applied 