# Public Repo 
It is a public repo to share my own developed codes.
Also I am used to adding useful material that can help a technical professional code, configure or maintain underlying systems.
Please feel free to give feedback.
Thanks


## Installing cloud-iac

### Compatible Python Versions

cloud-iac is known to work with Python versions 3.6, 3.7, and 3.8. Users have reported issues with Python 3.9.

#### Linux / Mac

Create a folder in your home directory called .pip
Create a file called pip.conf inside of the .pip directory
Add the following contents into your pip.conf configuration file:

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
 
