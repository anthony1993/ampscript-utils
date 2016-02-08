# AMPScript Logger

In order to use the logging capabilities in the AMPScript file ampscript-logger.amp, you will need to create a DataExtension in the Business Unit this code will run. The DataExtension should be setup as follows:

| Table Name | Column Name | Column Data Type|
| -----------|:------------| ---------------:|
| Logging | logId | Text(50) |
| Logging | logTime | Date (set as system current date)|
| Logging | logText | Text(50) | 
| Logging | logType | Text(50) |

# Why use the AMPScript Logger

A fair amount of the AMPScript I write is tied to MobileConnect, therefore, there are special functions & keywords that are only available in that context. I ended up getting frustrated by simply seeing "There was an error processing your message." in my text window - since it doesn't really tell you what happened. By adding in logging statements, I was able to get a better idea of how far my code was executing without needing to delete huge chunks of code. 

Now that I have this little utility, I see myself writing more templatized code that is simply going to print to a log table (maybe only having the conditionals pieces working), then going back in and plugging in code that writes to DataExtensions or calls out to an external API, etc. 

I found this little trick helpful, I hope you do as well.
 
