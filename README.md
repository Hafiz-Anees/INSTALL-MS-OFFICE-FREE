# Office Installation Guide using Office Deployment Tool

## Step 1: Download Office Deployment Tool

1. **Visit the Official Website**:
   Go to the [Microsoft Office Deployment Tool download page](https://www.microsoft.com/en-us/download/details.aspx?id=49117).

2. **Download the Tool**:
   Click the **Download** button and save the `officedeploymenttool.exe` file to your computer.

3. **Extract the Tool**:
   Run the `officedeploymenttool.exe` file and choose a location to extract the contents.

## Step 2: Create the Configuration File

1. **Navigate to the Extraction Folder**:
   Open the folder where you extracted the Office Deployment Tool.

2. **Create a New Configuration File**:
   Use a text editor (like Notepad) to create a new XML file. Name it `configuration.xml`.

3. **Add Configuration Settings**:
   Copy and paste the following sample configuration into your `configuration.xml` file, and modify it as needed:

   ```xml
   <Configuration>
     <Add OfficeClientEdition="64" Channel="Monthly">
       <Product ID="O365ProPlusRetail">
         <Language ID="en-us" />
       </Product>
     </Add>
     <Display Level="None" AcceptEULA="TRUE" />
     <Property Name="AUTOACTIVATE" Value="1" />
   </Configuration>


## Step 3: Download Office Installation Files

```
pen Command Prompt:
Press Win + R, type cmd, and press Enter.

for example
cd path\to\extracted\folder
````
## install office
run this command

```
setup.exe /configure configuration.xml
```

