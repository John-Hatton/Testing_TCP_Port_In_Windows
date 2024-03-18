# Testing TCP Port in Windows

---


To test a TCP port on your local server using PowerShell by utilizing the Test-NetConnection cmdlet. Here's how you can do it:

	Test-NetConnection -ComputerName localhost -Port <port_number>

Replace <port_number> with the port you want to test. For example:

	Test-NetConnection -ComputerName localhost -Port 80

This command will test if your local server is listening on port 80. You'll get output indicating whether the connection was successful or not.

Alternatively, you can use the Test-NetConnection cmdlet without specifying the -ComputerName parameter. In this case, it will test the connection to the local computer:

	Test-NetConnection -Port <port_number>

For example:

	Test-NetConnection -Port 80
