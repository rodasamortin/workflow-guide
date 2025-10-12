2025-10-07, NZST

# Git workflow

## Background

I begin by coding the task in its simplest form. It serves as an initial guide for transforming the code into a more reusable and maintainable structure. Finally, I evaluate how my code impacts the overall project.

I strive for my *code* to possess three key features: *feasibility, customizability, and compatibility* with the codebase. My code undergoes the following versions to ensure these three qualities are achieved:

***Code versions***

- basic: the simplest, untidiest, and most dumbed down version.*(feasibility)*
- modular: separate concerns *(customizability)*
	_ETC: Easier To Change_
	_SRP: Single Responsibility Principle:_ 1 change : 1 module

- advanced: optional* make the code more concise *(customizability)*
- testing: unit test *(compatibility)*
- final: most polished version. ready to be submitted to be reviewed or merged to main.*(compatibility)*

:tea: This structured approach keeps me focused and intentional in my coding. It helps ground me in the purpose of the project, making it easier to resist the temptation of pursuing endless "what-ifs" and "just one more feature."

### __Git Branch__

<br/>
Next, I will create a new <code>git branch</code> -> <code>pull-request</code> -> review <code>pull-request</code> -> <code>merge</code> changes

<br/>
Submitting a <code>pull-request</code> to myself helps me to see my code in a critique's perspective. Also, a merged PR groups related changes in chunks. It's cleaner than reading a long list of commit changes made in a day.

### Git Branch format

<code>code_version/file-name</code>

### __Git Commit Message__

 I want to highlight the *area* where the code is, and its *purpose*. It's important to show these in the _first 3-5 words._

 > Miller's Law - a person can hold up to 7 items in their working memory :wink:
 <br/>

A standardized commit messages format is vital in tracking files changes and preserving the code's history.
Mainly, a commit message has these components — *code version, message type, purpose.* Providing a scope is also optional.
<br/>

**A. Code Version**

I call it the code's stages of refinement.
<br/>
		<code>
			git commit -m "<b>type</b> -> <b>(optional_scope)</b> : purpose"
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

It's the summary of what happened in the code. Use imperative voice to make it sound neutral. 

### Git message format

<prep>
	<code>
		file_name | code_version | message_type -> *(optional scope)* : descriptiom
	</code>
</prep>

This format helps me to track the progress of how each file is linked to main.
