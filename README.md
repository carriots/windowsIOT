# windowsIOT
A dll to work with visual studio and deploy over RaspberryPi
------------------------------------------------------------

RaspberryPi_example WindowsIoT

Version - 1.00

Install the Library
Navigate to the Release page.
Download the latest release.
Extract the zip file.
Go to "Reference" >> "Add reference" in Visual Studio 2015



Library Reference
- Carriots
This library defines a type named Carriots which can be used to represent a communication interface with the Carriots API.
An example:
Carriots carriots = new Carriots();

- API_key
This object defines a property named API_Key which can be used to define a apikey at Carriots.
An example:
carriots.API_Key = "1234....ABCD";

- Device
This object defines a property named Device which can be used to define a device to send streams to Carriots.
An example:
carriots.Device = "defaultDevice@user.user";

- Add(String, String)
This object defines a method named Add which can be used for insert data in a stream. 
   - The method parameters accept two value of type string.
     An example:
	 carriots.Add("key","value");
	 
   - The method parameters accept one value of type string and one value of type int.
     An example:
	 carriots.Add("key",1234);

- Send_Stream()
This object defines a method named Send_Stream which can be used to send stream to Carriots.
An example:
carriots.Send_Stream();
