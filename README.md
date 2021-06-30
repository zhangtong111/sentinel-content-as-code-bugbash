## Branch bugbash-4

#### Test Case:

This branch contains a single valid ARM template for a scheduled analytics rule, inside the Templates folder:
![content1](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-4/Images/bb4-content.png)

#### Testing instructions

- Create the connection for branch `bugbash-4` on the target sentinel workspace
![content2](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-4/Images/bb4-connect1.png)

- Upon a successful connection - wait for the action to trigger
![content3](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-4/Images/running.png)

#### Expected Result:
- The Workflow should result in Success, however the rule should not get deployed 
![content4](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-4/Images/success.png)

#### Further Testing
Rename the `Templates` folder to `Detections` (no need to clone to your local machine, you can edit directly on github), and click commit changes.
![content5](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-4/Images/commit.png)

After commiting the change, wait for the action to finish successfully and make sure the rule exists in the analytics gallery
![content6](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-4/Images/gallery.png)
