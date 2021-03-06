# Saritasa.PsakeExtensions
## Expand-PsakeConfiguration
### Synopsis
Extends Psake properties from the hashtable.
### Syntax
Expand-PsakeConfiguration \[-NewConfiguration\] <Hashtable> \[<CommonParameters>\]
### Parameters

<table class="table table-striped table-bordered table-condensed visible-on">
	<thead>
		<tr>
			<th>Name</th>
			<th class="visible-lg visible-md">Alias</th>
			<th>Description</th>
			<th class="visible-lg visible-md">Required?</th>
			<th class="visible-lg">Pipeline Input</th>
			<th class="visible-lg">Default Value</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><nobr>NewConfiguration</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
## Import-PsakeConfigurationFile
### Synopsis
Checks file existence and dot-sources it.
### Syntax
Import-PsakeConfigurationFile \[-Path\] <String> \[<CommonParameters>\]
### Parameters

<table class="table table-striped table-bordered table-condensed visible-on">
	<thead>
		<tr>
			<th>Name</th>
			<th class="visible-lg visible-md">Alias</th>
			<th>Description</th>
			<th class="visible-lg visible-md">Required?</th>
			<th class="visible-lg">Pipeline Input</th>
			<th class="visible-lg">Default Value</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><nobr>Path</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
### Examples
**EXAMPLE 1**

		Import-PsakeConfigurationFile ".\Config.$Configuration.ps1"
		
\# default.ps1  
TaskSetup \`  
\{  
Import-PsakeConfigurationFile ".\\Config.$Configuration.ps1"  
\}  
  
\# Config.Debug.ps1  
  
Expand-PsakeConfiguration \`  
@\{  
ServerHost = 'dev.example.com'  
\}
