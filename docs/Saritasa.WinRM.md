# Saritasa.WinRM
## Get-RemoteTempPath
### Synopsis
Creates a new directory in remote server's %TEMP% and returns it.
### Syntax
Get-RemoteTempPath \[-Session\] <PSSession> \[<CommonParameters>\]
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
			<td><nobr>Session</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
## Initialize-RemoteManagement
### Syntax
Initialize-RemoteManagement \[\[-Credential\] <pscredential>\] \[\[-Port\] <int>\] \[\[-Authentication\] <AuthenticationMechanism>\] \[<CommonParameters>\]
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
			<td><nobr>Authentication</nobr></td>
			<td class="visible-lg visible-md">None</td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Credential</nobr></td>
			<td class="visible-lg visible-md">None</td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Port</nobr></td>
			<td class="visible-lg visible-md">None</td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
## Install-WinrmHttps
### Synopsis
Configures server to accept WinRM connections over HTTPS.
### Syntax
Install-WinrmHttps \[\[-CertificateThumbprint\] <String>\] \[-Force\] \[\[-AlternativeDnsNames\] <String\[\]>\] \[<CommonParameters>\]
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
			<td><nobr>CertificateThumbprint</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Force</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg">False</td>
		</tr>
		<tr>
			<td><nobr>AlternativeDnsNames</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
## Invoke-RemoteScript
### Synopsis
Executes a script on a remote server.
### Syntax
Invoke-RemoteScript \[-Path <String>\] \[-Parameters <Hashtable>\] -ServerHost <String> \[<CommonParameters>\]

Invoke-RemoteScript \[-Path <String>\] \[-Parameters <Hashtable>\] -Session <PSSession> \[<CommonParameters>\]
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
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Parameters</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>ServerHost</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Session</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
### Note
Based on code by mjolinor.
http://stackoverflow.com/a/27799658/991267

## Start-RemoteSession
### Syntax
Start-RemoteSession \[-ServerHost\] <string> \[<CommonParameters>\]
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
			<td><nobr>ServerHost</nobr></td>
			<td class="visible-lg visible-md">None</td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
