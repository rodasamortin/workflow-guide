
**Git workflow**

	<p> Ideally, create a new <code>git branch</code> -> <code>pull-request</code> -> review <code>pull-request</code> -> <code>merge</code> changes </p>

	<p> Submitting a <code>pull-request</code> to myself helps me to see my code in a critique's perspective. Also, a merged PR groups related changes in chunks. It's cleaner than reading a long list of commit changes made in a day </p>

***Commit message***

	<p> It is the summary of every changes made. It's important that the first 3-5 words convey what the change is about. 
	<p> A standardized commit messages format is vital in tracking files changes and preserving the code's history </p>
	<p> Mainly, a commit message has these components — <em> code status, message type, description. </em> Providing a scope is also optional.</p>
	<br/>

**A. Code Status***
	<p> I call it the code's stages of refinement. 

	<prep>
		<code>
			git commit -m "<b>type</b> -> <b>(optional_scope)</b> : description"
		</code>
	</prep>

		<p> I categorize commit messages into several types. It's like a gist of what the commit message is </p>

		<ul><b>Message types</b>
			<br/>
			<li><u> new_file :</u> initiate new file, plan, feature or challenge </li>
			<li><u> feat:</u> new feature </li>
			<li><u> bug :</u> initial bug spotted </li>
			<li><u> bug | attempt_fix:</u> debugging </li>
			<li><u> fix:</u> debugging completed</li>
			<li><u> refactor:</u> rewrite code without altering the logic, API or UI behavior </li>
			<li><u> perf: </u> improve performance (ex. basic code -> modular, global var -> function())</li>
			<li><u> doc: </u> update documentation or READMe. </li>
			<li><u> style: </u> adjust spacing, font-related matters </li>
			<li><u> chore: </u> general uncategorised tasks (ex. edit .gitignore, tidy comments)</li>
		</ul>

	<p> I always start in the <em>simplest code</em> to fulfill a task. Then, I organize them to <em>blocks</em> to be modular. It makes the code reusable and limit usage of global variables. Additionally, I would </p>


	<prep>
		<code>
			basic_code| message_type -> (scope) <i>optional</i> : commit_message
		</code>
	</prep>

