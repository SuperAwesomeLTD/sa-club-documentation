<table>
	<thead>
		<tr>
			<td colspan="4">Method</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">saAppApi.notifications.notify(parameters)</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<td colspan="4">Parameters</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>name</td>
			<td>type</td>
			<td>default</td>
			<td>comment</td>
		</tr>
		<tr>
			<td>targetUserIds</td>
			<td>array of integers</td>
			<td>[ ]</td>
			<td>cthe ids of the users of your application that should receive the notification</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<td colspan="4">Response</td>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">
				A promise that will:
				<ul>
					<li>be resolved without data if the notification was sent successfully</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>
