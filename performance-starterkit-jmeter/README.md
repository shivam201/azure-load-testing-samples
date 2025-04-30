# Performance Starter Kit for JMeter and Azure Load Testing
The performance starter kit for JMeter is designed to streamline the performance testing process using Azure Load Testing. Using this kit, you can:

1. Ensure compatibility with ALT: The kit converts your JMeter test scripts to be compatible for use with Azure Load Testing.
2. Azure Load Test Setup and Execution: It creates the Azure Load Test setup and executes JMeter test scripts within Azure Load Testing.
3. Prerequisites Installation: The kit installs the latest versions of all necessary prerequisites for using JMeter.
4. JMeter Setup: It handles the setup of JMeter, ensuring that users are ready to use it immediately.
5. JMeter Plugins Installation: The kit installs essential JMeter plugins, which are crucial for creating real-world performance test scripts.
6. Standard JMeter Template Script: It generates a standard JMeter template script, helping performance testers create scripts faster.
7. Generic Report Generation: The kit includes a facility for generating generic JMeter reports from result JTL files.
8. Auto Suite Generation: It assists in the automatic generation of test suites (.jmx files).
9. JMeter Test Best Practices: The kit provides guidelines for best practices in JMeter testing.

# How to Use the Kit
1. Clone the repository to your local machine.
2. Install Azure CLI If you haven't already. You can find the installation instructions [here](https://docs.microsoft.com/en-us/cli/azure/install-azure-cli).
3. Update the `config.json` file with your Azure credentials(Tenant,subscription,Resource Group)and other necessary configurations(duration,secret,certificate,env variables if any) for running and ALT setup
4. Enable starterkit setup if you want to install the prerequisites and setup JMeter. You can do this by setting the `enable_starterkit_setup` variable to `true` in the `config.json` file.
5. To generate the suite from APIM or Swagger you need to suitegenerationfromswagger or suitegenerationfromapimconfig=true and provie the swagger or apim file complete path in the config.json file.
6. To enable html report generation set the reportgeneration variable to `true` in the `config.json` file and provide the path to the jtl file in the config.json file.

## Resources

- Learn more about [Azure Load Testing](https://aka.ms/malt)
- [Azure Load Testing documentation](https://aka.ms/malt-docs)