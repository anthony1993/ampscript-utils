#H1 Ampscript Logger

In order to use the logging capabilities in the AMPScript file ampscript-logger.amp, you will need to create a DataExtension in the Business Unit this code will run. The DataExtension should be setup as follows:

| Table Name | Column Name | Column Data Type|
| -----------|:------------| ---------------:|
| Logging | logId | Text(50) |
| Logging | logTime | Date (set as system current date)|
| Logging | logText | Text(50) | 
 
