# Sample-MSTest.Sdk

- If you run `dotnet test` without the file Directory.Build.props, it works fine.

- If you run `dotnet test` with the file Directory.Build.props, you get error:

```
System.ComponentModel.Win32Exception (2): An error occurred trying to start process '<folder_redacted>\Sample-MSTest.SDK\bin\Test\net10.0\Test.exe' with working directory '<folder_redacted>\Sample-MSTest.SDK'. The system cannot find the file specified.
   at System.Diagnostics.Process.StartWithCreateProcess(ProcessStartInfo startInfo)
   at System.Diagnostics.Process.Start(ProcessStartInfo startInfo)
   at Microsoft.DotNet.Cli.Commands.Test.TestApplication.RunAsync()
   at Microsoft.DotNet.Cli.Commands.Test.TestApplication.RunAsync()
   at Microsoft.DotNet.Cli.Commands.Test.TestApplicationActionQueue.Read(BuildOptions buildOptions, TestOptions testOptions, TerminalTestReporter output, Action`1 onHelpRequested)
 ```