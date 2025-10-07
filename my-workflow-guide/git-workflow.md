2025-10-07, NZST

# Git workflow

## Background

I begin by coding the task in its simplest form. It serves as an initial guide for transforming the code into a more reusable and maintainable structure. Finally, I evaluate how my code impacts the overall project.

In summary, I strive for my *code* to possess three key features: *feasibility, customizability, and compatibility* with the codebase. My code undergoes the following versions to ensure these three qualities are achieved:

***Code versions***

- basic: the simplest, and possibly untidiest version.
- modular: convert the code in modules for reusability and maintainability
- advanced: optional* make the code more concise
- testing:
- final: most polished version. ready to be submitted to be reviewed or merged to main.

:tea: This structured approach keeps me focused and intentional in my coding. It helps ground me in the purpose of the project, making it easier to resist the temptation of pursuing endless "what-ifs" and "just one more feature."

### Git Branch

<br/>
Next, I will create a new <code>git branch</code> -> <code>pull-request</code> -> review <code>pull-request</code> -> <code>merge</code> changes

<br/>
Submitting a <code>pull-request</code> to myself helps me to see my code in a critique's perspective. Also, a merged PR groups related changes in chunks. It's cleaner than reading a long list of commit changes made in a day.

### Git Branch format

<code>code_version/file-name</code>

### Commit message

 It is the summary of every changes made. It's important that the first 3-5 words convey what the change is about. 
 <br/>

A standardized commit messages format is vital in tracking files changes and preserving the code's history
Mainly, a commit message has these components — *code version, message type, description.* Providing a scope is also optional.
<br/>

**A. Code Version**

I call it the code's stages of refinement.
<br/>
		<code>
			git commit -m "<b>type</b> -> <b>(optional_scope)</b> : description"
		</code>
<br/>

I categorize commit messages into several types. It's like a gist of what the commit message is

**B. Message types**
<br/>
1. new_file: initiate new file, plan, feature or challenge 
2. feat: new feature 
3. bug :initial bug spotted 
4. bug | attempt_fix:  debugging 
5. fix: debugging completed
6. refactor: rewrite code without altering the logic, API or UI behavior 
7. perf:  improve performance (ex. basic code -> modular, global var -> function())
8. doc: update documentation or READMe. 
9. style: adjust spacing, font-related matters
10.chore: general uncategorised tasks (ex. edit .gitignore, tidy comments)
<br/>

**C. Description**

It's the summary of what happened in the code. 

### Git message format

<prep>
	<code>
		file_name | code_version | message_type -> *(optional scope)* : descriptiom
	</code>
</prep>

This format helps me to track the progress of how each file is linked to main.
