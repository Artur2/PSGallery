# Saritasa.LocalManagement
## Set-PasswordNeverExpires
### Synopsis
Sets 'password never expires' flag for local user.
### Syntax
Set-PasswordNeverExpires \[-Username\] <String> \[<CommonParameters>\]
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
			<td><nobr>Username</nobr></td>
			<td class="visible-lg visible-md"></td>
			<td></td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">false</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
### Note
Requires administrator permissions.

## Test-UserIsAdministrator
### Synopsis
Returns $true if user has Administrator role.
### Syntax
Test-UserIsAdministrator \[<CommonParameters>\]
