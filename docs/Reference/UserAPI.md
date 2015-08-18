<table>
	<thead>
		<tr>
			<th>Method</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>saUserApi.authentication.getUserId()</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th>Response</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				A promise that will:
				<ul>
					<li>be resolved with the id of the current user</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th>Method</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>saUserApi.authentication.getUser()</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th>Response</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				A promise that will:
				<ul>
					<li>
						be resolved with the current user. Example: {id: 42, username: ‘MyUsername’}
					</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="4">Method</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">saUserApi.events.hasTriggeredEvent(parameters)</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th colspan="4">Parameters</th>
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
			<td>eventId</td>
			<td>integer</td>
			<td></td>
			<td>the id of the event</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th colspan="4">Response</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">
				A promise that will:
				<ul>
					<li>be resolved with true if the user has triggered the event, false otherwise</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="4">Method</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">saUserApi.events.hasTriggeredEvents(parameters)</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th colspan="4">Parameters</th>
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
			<td>eventIds</td>
			<td>array of integers</td>
			<td>[ ]</td>
			<td>the ids of the events</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th colspan="4">Response</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">
				A promise that will:
				<ul>
					<li>be resolved with an object mapping the event ids to booleans indicating if the events have been triggered. {101: true, 102: false, 103: true, ...}</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>

<table>
	<thead>
		<tr>
			<th colspan="4">Method</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">saUserApi.events.triggerEventWithToken(parameters)</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th colspan="4">Parameters</th>
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
			<td>token</td>
			<td>string</td>
			<td></td>
			<td>a unique token that identifies the event</td>
		</tr>
		<tr>
			<td>points</td>
			<td>points</td>
			<td>the number of points defined on the event</td>
			<td>
				the number of points to give to the user
				<ul>
					<li>min: 0</li>
					<li>max: the number of points defined on the event</li>
				</ul>
			</td>
		</tr>
	</tbody>
	<thead>
		<tr>
			<th colspan="4">Response</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">
				A promise that will:
				<ul>
					<li>be resolved if the points were awarded successfully</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>

