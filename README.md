## runCxCLI 
runCxCLI is a cross platform wrapper for the Checkmarx CLI plugin designed to return the exit code and error message after a scan. 

### Usage
* Place the runCxCLI.jar file in the CxConsolePlugin-x.x.x folder on your system.
* Call the jar with java -jar runCxCLI.jar followed by typical CLI parameters.
* Example:
```
java -jar runCxCLI.jar -CxServer <server> -CxUser <username> -CxPassword <password> -projectName CxServer/path/to/project -locationtype Git -locationurl https://github.com/xxx/xxx -locationbranch refs/head/branch
```
* Optional CLI parameters are supported as enumerated on https://checkmarx.atlassian.net/wiki/spaces/SD/pages/1297547309/CxSAST+CxOSA+Scan
* For parameters with spaces, please enclose in double quotes for example -preset "High and Medium"
* **Note** This wrapper was developed for use with CxSAST 9.x. It should work with prior versions. Limited testing has been done with version 8.9 https://checkmarx.atlassian.net/wiki/spaces/SD/pages/914096139/CxSAST+CxOSA+Scan+v8.9.0
