# CLCAPIPullAllServers

Code repository for a PowerShell script to generate a report of CenturyLink Cloud Virtual Machines for a given customer account.

Author: Matt Schwabenbauer

Date: October 5, 2016

Matt.Schwabenbauer@ctl.io

### About this repository

This script is written to run on Windows Operating Systems and generates a CSV file with the results. The file will be opened automatically and its location on the hard drive will be printed in the PowerShell console.

### Running the script

After downloading the script, dot source the file wherever it is located on your hard drive. For example: ./"c:/users/administrator/downloads/CLCAPIPullAllServers.ps1". Alternative, you could export the function contained in the script and import it as a module. This is the best option if you plan on repeatedly using this functionality.

Once the script is properly sourced, it can be run. Example: >CLCAPIPullAllServers -alias MSCH -APIKey 'XXXXXXXXXXXXXXX' -APIPass 'XXXXXXXXXXXXX'

Please note that all of the parameters for this script are optional. If you run the script without parameters, you will be prompted for the subject account alias, API Key and API password in the PowerShell console.

### Authentication

In order to run this script, you need a CenturyLink Cloud v1 API key and password. This can be found after logging in to the CenturyLink Cloud Control Portal at control.ctl.io and navigating to settings > API. If you do not see any API user information, you can click the button "Create Api User" to create a new API user, or contact your account administrator if you do not have permissions to create an API user. If you experience an error, please reach out to our support team at help@ctl.io

### Support

This code is presented as is and is open to contribution from the community.

Feature requests and enhancements can be suggested to Matt.Schwabenbauer@ctl.io. Any future development is not guaranteed.