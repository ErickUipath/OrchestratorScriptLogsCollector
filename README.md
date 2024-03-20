PowerShell script has been created to assist in gathering logs from users, who are experiencing issues with the Orchestrator. The script collects the following information:

Application logs
Security logs
System logs
CAPI2 logs (for certificate issues)
Appsettings.Production.json
UiPath.Orchestrator.dll.config
IIS logs from the last 7 days
Output for the Platform Configuration Tool readiness check
Network trace (optional, can be enabled during the script execution)
 
To use the script, it is required to run it as an Administrator on the Orchestrator machine. Find the script at the following location: [Orchestrator Log Gathering .](https://codeload.github.com/ErickUipath/OrchestratorScriptLogsCollector/zip/refs/heads/main)

During the execution, specify the Orchestrator installation path; press enter to use the default path
Subsequently, there will be option to initiate a network trace( Note that this can significantly increase the script's runtime.)
Reproduce the identifiable issue and once done, press enter to continue
The script will then gather all the necessary logs, output the results of the Readiness check, and save everything in an archive. This archive should then be sent back to us for further analysis.
