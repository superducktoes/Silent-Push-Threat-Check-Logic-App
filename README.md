# Silent-Push-Threat-Check-Logic-App

Logic app for Azure using Silent Push ThreatCheck for additional enrichment

ACCESS_KEY is for ThreatCheck API token
API_KEY is for Silent Push API token

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fsuperducktoes%2FSilent-Push-Threat-Check-Logic-App%2Fmain%2Fazuredeploy.json)


After deploying it can be called with the following options. Note that explain and scan data can be set depending on the level of detail required.

curl -X POST -H "Content-Type: application/json" -d '{
  "domain": "<DOMAIN>",
  "explain": "1",
  "scan_data": "0"
}' "<WORKFLOW_URL>"
