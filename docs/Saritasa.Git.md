# Saritasa.Git
## Get-GitFlowStatus
### Syntax
Get-GitFlowStatus -BranchType <BranchType> \[-Path <string>\] \[-OlderThanDays <int>\] \[<CommonParameters>\]
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
			<td><nobr>BranchType</nobr></td>
			<td class="visible-lg visible-md">b</td>
			<td>Specify branch type</td>
			<td class="visible-lg visible-md">true</td>
			<td class="visible-lg">true \(ByValue, ByPropertyName\)</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>OlderThanDays</nobr></td>
			<td class="visible-lg visible-md">None</td>
			<td>Show branches with last commit made later than N days</td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">true \(ByPropertyName\)</td>
			<td class="visible-lg"></td>
		</tr>
		<tr>
			<td><nobr>Path</nobr></td>
			<td class="visible-lg visible-md">p</td>
			<td>Path to git repository</td>
			<td class="visible-lg visible-md">false</td>
			<td class="visible-lg">true \(ByPropertyName\)</td>
			<td class="visible-lg"></td>
		</tr>
	</tbody>
</table>			
