# AzureAnalysisServicesSample

This is a sample SSAS Tabular Model which integrates with recently annonced Azure Analysis Services. Model uses publicly available AdentureWorks database.
It shows how to add Calculated Columns, Measures and KPI in a SSAS Model.
Finally There is a PowerBI App which can get data from SSAS Model and visualize a KPI.

There is setup required before you try to run this solution:

Prerequisites:
Make sure you have latest version of SSDT (SQL Server Data Tools) installed. If not, then get it from 
https://msdn.microsoft.com/en-us/library/mt204009.aspx

Once SSDT is installed, download the solution from this repo and open it in SSDT.

Launch an instance of Analysis Services from Azure portal and copy server URL. URL will look like this:

asazure://southcentralus.asazure.windows.net/<My Service>

You need to put this Server URL in the SSAS Solution -> Properties -> Workspace Server

Now build and deploy the solution. You should be all set!


In order to visualize in PowerBI, download .pbix file from this repo and open it you local PowerBI desktop.
Go to Get Data and pick SSAS database. Provide Server URL from your Azure Analysis Service instance. You should see KPI Visual.

Hope you like the demo.

P.S. This is my first commit to Git Repo and I understand documentation/instructions may not be enough.
Please share your feedback and I will try to update and make it more user friendly.
