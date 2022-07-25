Power BI Content for Dynamics 365 Sales, Marketing, Field Service, and Project Operations

# A Note About Templates
When it comes to BI, don't expect to install a template from *anyone* and have it "just work" for your company. This is a reality of BI and reporting, not of the capabilities of the template designer.

These templates are designed to be a good starting point to build from.

# Installation Parameters for Data Model
When opening a Data Model .pbit file, you will see the following parameters:

| Parameter | Instructions |
| --- | ----------- |
| Dynamics 365 URL | yourdynamics.crm.dynamics.com • The URL of your Dynamics 365 CRM environment. Don't include https:// |
| Company Time Zone Offset - From UTC In Hours | e.g. "-4" for US Eastern. • This is a simplified approach for converting Date/Time fields to Date Only. This may not be right for global organizations or when the precise time offset is important. |
| SQL Server (Optional) | OPTIONAL • The name of the Dataverse or Data Lake SQL endpoint. Populating this field will force the data model to use the SQL connector instead of the Dataverse connector. |
| SQL Database (Optional) | OPTIONAL • The name of the Dataverse or Data Lake database. |
| SQL Schema (Optional) | OPTIONAL • e.g. "dbo" • The name of the SQL schema. |

# Publishing
The .pbix file created from the .pbit file should be published to a PowerBI.com Workspace. From there reports can be pointed at the data model.
