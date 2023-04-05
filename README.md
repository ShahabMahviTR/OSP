# Public Repo 
It is a public repo to share my own developed codes.
Also I am used to adding useful material that can help a technical professional code, configure or maintain underlying systems.


## Installing cloud-iac

### Compatible Python Versions

cloud-iac is known to work with Python versions 3.6, 3.7, and 3.8. Users have reported issues with Python 3.9.

[global]  
extra-index-url = https://<ArtifactoryUsername>:<APIKey/AccessToken>@tr1.jfrog.io/artifactory/api/pypi/pypi/simple

Note that your Artifactory username is your UID, prefixed with a "c" for contractors and "x" for extranet users (but never "u"). Examples include "6029881", "c602988" and "x602989". The API key is retrieved by logging into TR Artifactory and going to "Edit Profile".
Proceed to the Install section. 

 
#### Windows

    Create a folder in your home directory (c:\users\<employeeid>) called pip.
    Create a file called pip.ini inside of the pip directory.
    Add the following contents into your pip.ini configuration file:

    [global]
    extra-index-url = https://<ArtifactoryUsername>:<APIKey/AccessToken>@tr1.jfrog.io/artifactory/api/pypi/pypi/simple

    Proceed to the Install section.
 
### Install

To install, run the following command:

    pip install --upgrade cloud-iac
 

to install a specific version, assuming you know the version number, run this command:

    pip install --upgrade cloud-iac==x.x.x
 

 
### Cumulus
		a. Assign the AWS Account to  ${AssetId}-PowerUser2
		b. Install Python 3.7.9
		c. Install NodeJS
		d. Install AWS CDK
		e. Cloud-Tool (quick start guide)
			i. Go to your home directory and create a folder called pip
			ii. Inside of the folder create a file called pip.ini as below:
				[global]
				extra-index-url=https://<employee-id>:<APIKey>@tr1.jfrog.io/tr1/api/pypi/pypi-local/simple
			Replace <employee-id> with your own and modify <APIKey> according to JFrog Artifcatory described below.
			iii. Now you need to create a folder in your home directory as .venv
			iv. Change folder to .venv and run the following command
				python -m venv cloud-tool
			v. In the same directory (.venv) you should now be able to see a new folder called cloud-tool. Now run the following batch script:
				cloud-tool\Scripts\activate.bat
			vi. The prompt should have been prefixed with cloud-tool.
			vii. Install cloud-tool by the following command
				(cloud-tool)$ pip install --upgrade cloud-tool
			viii. Make sure you have the correct version of the cloud-tool now:
				(cloud-tool)$ cloud-tool --version
				8.4.0
			ix. And make sure AWS CLI is installed correctly:
				aws --version
			x. you can login to cloud-tool (you need to enter your M Account)password via CyberArk:
			(cloud-tool)$ cloud-tool login
			
			Using default region (us-east-1) and profile (default) from /Users/dan/cloudtool_defaults
			
			MGMT Password: (Copy/paste or enter your CyberArk password)
			
			...
			[127]: tr-ihn-prod (728595430554): human-role/a205654-PowerUser2 (GitHub Enterprise Cloud for TR)
			[128]: tr-ihn-prod (728595430554): human-role/a206614-PowerUser2 (SparkPost)
			[129]: tr-legal-sandbox (036263847021): human-role/202133-PowerUser (Judicial Workbench (JWB))
			[130]: tr-legal-sandbox (036263847021): human-role/202133-ReadOnly (Judicial Workbench (JWB))
			[131]: tr-legal-sandbox (036263847021): human-role/a202133-PowerUser2 (Judicial Workbench (JWB))
			[133]: tr-sap-preprod (100918290719): human-role/205334-ReadOnly (SAP S/4 Hana)
			
			Role selection: 128
			
			----------------------------------------------------------------
			Your new access key pair has been stored in the AWS configuration file /Users/dan/.aws/credentials under the default profile
			Note that it will expire at 2022-02-09 22:39:33+00:00.
			After this time you may safely rerun this script to refresh your access key pair.
			To use this credential call the AWS CLI with the --profile option (e.g. aws --profile default ec2 describe-instances).
			----------------------------------------------------------------
			
		f. Access to Artifactory
			i. Go to JFrog page

			ii. Use SAML SSO to login
			iii. You should now be able to see list of artifacts

			
	2. Cloud-iac (quick start guide)
	In VS Code terminal, issue the following command:
		pip install --upgrade cloud-iac
		
	To make sure you have installed cloud-iac correctly, use the following command as can be seen in the print-screen
		pip show cloud-iac
		

	3. DataDog
![image](https://user-images.githubusercontent.com/63318092/230209511-d832c2b9-cd20-4147-b57b-275f29836d16.png)

