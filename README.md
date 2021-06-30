## Branch bugbash-3

#### Test Case:

This branch contains a single ARM template for a workbook in the Detections folder:
![content1](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-3/Images/bb3-content.png)

#### Testing instructions

- Create the connection for branch `bugbash-3` on the target sentinel workspace
![content2](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-3/Images/bb2-content.png)

- Upon a successful connection - wait for the action to trigger
![content3](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-3/Images/bb3-content.png)

#### Expected Result:
- The workflow should result in failure, and the workbook should not get deployed
![content4](https://raw.githubusercontent.com/erant10/sentinel-content-as-code-bugbash/bugbash-3/Images/failure.png)
