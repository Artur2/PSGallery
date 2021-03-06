# Saritasa.General
## Get-CallerPreference
### Synopsis
Fetches "Preference" variable values from the caller's scope.
### Syntax
Get-CallerPreference -Cmdlet <Object> -SessionState <SessionState> \[<CommonParameters>\]

Get-CallerPreference -Cmdlet <Object> -SessionState <SessionState> \[-Name <String\[\]>\] \[<CommonParameters>\]
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
			<td><nobr>Cmdlet</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>The $PSCmdlet object from a script module Advanced Function.</td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>SessionState</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>The $ExecutionContext.SessionState object from a script module Advanced Function.  This is how the  
Get-CallerPreference function sets variables in its callers' scope, even if that caller is in a different  
script module.</td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Name</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td>Optional array of parameter names to retrieve from the caller's scope.  Default is to retrieve all  
Preference variables as defined in the about\_Preference\_Variables help file \(as of PowerShell 4.0\)  
This parameter may also specify names of variables that are not in the about\_Preference\_Variables  
help file, and the function will retrieve and set those as well.</td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">true \(ByValue\)</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
### Inputs
 - String

### Outputs
 - None.  This function does not produce pipeline output.

### Note
Import Preference variables from the caller of a Script Module function
https://gallery.technet.microsoft.com/scriptcenter/Inherit-Preference-82343b9d
MICROSOFT LIMITED PUBLIC LICENSE

### Examples
**EXAMPLE 1**

		Get-CallerPreference -Cmdlet $PSCmdlet -SessionState $ExecutionContext.SessionState
		
Imports the default PowerShell preference variables from the caller into the local scope.
**EXAMPLE 2**

		Get-CallerPreference -Cmdlet $PSCmdlet -SessionState $ExecutionContext.SessionState -Name 'ErrorActionPreference','SomeOtherVariable'
		
Imports only the ErrorActionPreference and SomeOtherVariable variables into the local scope.
**EXAMPLE 3**

		'ErrorActionPreference','SomeOtherVariable' | Get-CallerPreference -Cmdlet $PSCmdlet -SessionState $ExecutionContext.SessionState
		
Same as Example 2, but sends variable names to the Name parameter via pipeline input.
### Links

 - [System.Collections.Hashtable.name](System.Collections.Hashtable.link)
## Test-IsLocalhost
### Synopsis
Returns $true if hostname represents local PC.
### Syntax
Test-IsLocalhost \[\[-ComputerName\] <String>\] \[<CommonParameters>\]
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
			<td><nobr>ComputerName</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
