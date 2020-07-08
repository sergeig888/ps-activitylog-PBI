# ps-activitylog-PBI
## PowerShell code snippets for leveraging Power BI Activity Log events for common admin tasks

 These sample PowerShell script code fragments are intended to help flatten the curve when learning how to use Activity Log API in Power BI service. 

These samples can help Power BI tenant admins learn how to parse data out of most popular Acitivity Log events using PowerShell. Familiarity with [Power BI Admin API](https://docs.microsoft.com/en-us/rest/api/power-bi/admin) and [Power BI PowerShell modules](https://docs.microsoft.com/en-us/powershell/power-bi/overview?view=powerbi-ps) is desirable. PS modules need  to be installed prior to executing these script blocks. See dedicated to [Activity Log](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-auditing) doc for more details. Note that the event activities have [documented](https://docs.microsoft.com/en-us/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide) lag of up to 30 min. Typical for average use Power BI production tenant lag is between 15-22 min for an activity to show up in the output of this script. This is work in progress and this release is initial beta version of the script.  

## How to use this sample

Requirements:
* Install [Power BI PowerShell modules](https://docs.microsoft.com/en-us/powershell/power-bi/overview?view=powerbi-ps)
* User of the PS script has to login using Connect-PowerBIServiceAccount commandlet and provide Power BI tenant Admin credentials when prompted. Tenant Admin access scope is required to access Activity Log API. Users without tenant Admin privileges will not be able to successfully execute code fragments in this script. All code fragments and scenarios are annotated with "how to" instructions and common gaps/issues to watch out for.
