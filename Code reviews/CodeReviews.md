# Code Reviews
### Practices to follow when trying to debug a code
- Establish your role in the review process: author or reviewer. The author creates the code, the reviewer investigates, examines and reports.
- Establish the platform and methodology to ensure the smooth running of the review process.
- Establish the appropriate review technique: 
  1. Over the Shoulder: author is looked at while investigating the code. Use this method for **short pieces of code only**, as it demands a lot of attention to detail.
  2. Email pass-around: code is sent to reviewers by the author or SCM system.
  3. Pair Programming: source code is developed by two authors and then reverse engineered. 
  4. Tool-assisted: use tools to the review the code, regardless whether you are a reviewer or author.

- Omitting appropriate debugging procedures can potentially result in expensive or time consuming efforts to fix problems at a later stage of the development process. It is therefore crucial that the above mentioned techniques are used whenever developing a piece of code.
- Maintaining a consistent coding style is necessary to allow the company to respond to errors in a fast and efficient manner, as well as enable efficient design and implementation processes. 
- We aim to provide secure applications, which can only be achieved if employees follow the security review protocols. 
- Appropriate code review enables us to deliver services and create projects our stakeholders trust and come back to. 

### When reviewing codes
- Do not attempt to review more than 400 lines of code (LOC) to ensure that information are processed appropriately. Any more LOC over a prolonged period of time will not bring the desired results.
- Take and manage your time appropriately. Do not skim over the code, forcing other reviewers to pick up on errors that were missed.
- Do not exceed a review period of 60 minutes to ensure a more focused review. And allow for sufficient breaks of about 20 minutes.
- Conduct frequent reviews to avoid having to review many LOC.
- Establish and document a set of **SMART** goals to maintain a record of and create a guideline for the review process.
- Follow a checklist to stay on top of and distribute the workload and capture metrics. 
- Use an appropriate review tool such as Collaborator, Codebrag, Gerrit, Rhodecode, Crucible, Review Board, JArchitect, or Peer Review Plugin for increased support and accuracy.
- Adhere to formatting standards to ensure consistency and accuracy (formatting, alignments, naming, space, comments, architecture).




## Online Resources
[Code review best practices](https://medium.com/cuelogic-technologies/code-review-process-best-practices-3eeecab26ded)