

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
						be resolved with the current user. Example: 
<pre><code class="lang-json">{
	id: 42,
	username: ‘MyUsername’
}</code></pre>
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
					<li>be resolved with an object mapping the event ids to booleans indicating if the events have been triggered.
<pre><code class="lang-json">{
	101: true,
	102: false,
	103: true,
	...
}</code></pre>
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
			<td>integer</td>
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

<table>
	<thead>
		<tr>
			<th colspan="4">Method</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="4">saUserApi.games.getGame(parameters)</td>
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
			<td>gameId</td>
			<td>integer</td>
			<td></td>
			<td>the id of the game</td>
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
					<li>be resolved with a game object
<pre><code class="lang-json">{
    id: 42,
    name: ‘Game abc’,
    // Indicates if the best score is the maximum or the minimum
    bestScoreFunction: ‘min’ 
}</code></pre>
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
			<td colspan="4">saUserApi.games.getGameScore(parameters)</td>
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
			<td>gameId</td>
			<td>integer</td>
			<td></td>
			<td>the id of the game</td>
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
					<li>be resolved with the global score of the user in the game (across all the levels)
<pre><code class="lang-json">{
	score: 999,
	rank: 1234
}</code></pre>
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
			<td colspan="4">saUserApi.games.getGamesScores(parameters)</td>
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
			<td>gameIds</td>
			<td>array of integers</td>
			<td></td>
			<td>the ids of the games</td>
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
					<li>be resolved with an object mapping the game ids to the global score of the user in the games (across all the levels, respectively)
<pre><code class="lang-json">{
	1: {
        score: 999,
        rank: 1234
    },
    2: {
        score: 998,
        rank: 1237
    }
}</code></pre>
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
			<td colspan="4">saUserApi.games.getGameLeaderBoard(parameters)</td>
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
			<td>gameId</td>
			<td>integer</td>
			<td></td>
			<td>the id of the game</td>
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
					<li>be resolved with the leaderboard of the game
<pre><code class="lang-json">{
	// Number of scores
    count: 123,
    // Size of the current page (pagination not yet implemented)
    limit: 10,
    // Index of the first result of the page (pagination not yet implemented)
    offset: 0,
    results: [
        {
            score: 999
            rank: 1,
            user: {
                id: 125,
                username: ‘User 125’
            }
        },
        {
            score: 1005
            rank: 2,
            user: {
                id: 15,
                username: ‘User 15’
            }
        }
    ]
}</code></pre>
					</li>
					<div>or</div>
					<li>be rejected with an error</li>
				</ul>
			</td>
		</tr>
	</tbody>
</table>