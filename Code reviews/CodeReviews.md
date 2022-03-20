# Code Reviews

<a href="https://jserd.springeropen.com/articles/10.1186/s40411-018-0058-0/figures/1">

<img alt="Overview of the Code Review Process" src="https://www.researchgate.net/publication/328541762/figure/fig1/AS:686040184528896@1540576134082/Overview-of-the-Code-Review-Process.png" width="470" height="230">
</a>

For effective code reviews it is necessary to establish the platform and methodology, ensuring the smooth running of the review process. Your role in the review process will be either the author or reviewer. The author creates the code, the reviewer investigates, examines and reports.
## Practices to follow when trying to debug a code

- Establish the appropriate review technique: 
  1. Over the Shoulder: author is looked at while investigating the code. Use this method for **short pieces of code only**, as it demands a lot of attention to detail.
  2. Email pass-around: code is sent to reviewers by the author or SCM system.
  3. Pair Programming: source code is developed by two authors and then reverse engineered. 
  4. Tool-assisted: use tools to the review the code, regardless whether you are a reviewer or author.
   
- Omitting appropriate debugging procedures can potentially result in expensive or time consuming efforts to fix problems at a later stage of the development process. It is therefore crucial that the above mentioned techniques are used whenever developing a piece of code.
- Maintaining a consistent coding style is necessary to allow the company to respond to errors in a fast and efficient manner, as well as enable efficient design and implementation processes. 
- We aim to provide secure applications, which can only be achieved if employees follow the security review protocols. 
- Appropriate code review enables us to deliver services and create projects our stakeholders trust and come back to. 
- Following appropriate review techniques will allow employees to constantly learn and improve and strengthen each other. (Teamwork)

## When reviewing codes
- We are implementing code review as a mean to ensure quality. 
    -	Establish the framework of the code development process such as **discussing annotation practices**.
    -	Allow for important information to be **peer reviewed** to ensure alignment within the review team. 
    -	Ensure that errors are found and fixed.
    -   Always leave comments
        - This is an essential part to take some time and explain significant pieces. This a language of communication between programmer and user. 
        - It's very useful when checking variables, functions, complex loops and conditional statements.
- **Do not attempt** to review more than 400 lines of code (**LOC**) to ensure that information are processed appropriately. Any more LOC over a prolonged period of time will not bring the desired results.
  
- **Take and manage your time appropriately**. Do not skim over the code, forcing other reviewers to pick up on errors that were missed.
  
- **Do not exceed** a review period of 60 minutes to ensure a more focused review. And allow for sufficient breaks of about 20 minutes.
  
- **Conduct frequent reviews** to avoid having to review many **LOC**.
  
- Establish and document a set of **SMART** goals to maintain a record of and create a guideline for the review process.
  
- **Follow a checklist** to stay on top of and distribute the workload and capture metrics.
  
- **Use an appropriate review tool** such as Collaborator, Codebrag, Gerrit, Rhodecode, Crucible, Review Board, JArchitect, or Peer Review Plugin for increased support and accuracy.
  
- **Adhere to formatting standards** to ensure consistency and accuracy (formatting, alignments, naming, space, comments, architecture).

## Microsoft’s code review process

Microsoft is a good example. They are backed by research and are based on large-scale experiences and studies involving thousands of engineers and millions of comments on the code review.

For starters, Microsoft has approximately **140,000 employees**. About **44%** of them are engineers, which means over **60,000** employees. Different products such as Office, Visual Studio, or Windows are developed by thousands of engineers simultaneously working on the same codebase. One of the essential facts about code reviews at Microsoft is that it is a highly adopted engineering practice. Most high-performance teams spend much time reviewing the code.

In this study, **36%** of developers said they perform code reviews multiple times a day. Another **39%** of developers said they perform code reviews at least once daily. **12%** perform code reviews various times a week, and only **13%** said they did not perform a code review in the past week.
This means that Microsoft developers spend a significant portion of their time on code reviews. So it's essential to make sure this time is well spent.

## Which benefits does code reviewing provide?

<img alt="Benefits of code reviews" src="https://i0.wp.com/www.michaelagreiler.com/wp-content/uploads/2019/03/Code-Review-at-Microsoft-Graphics.png?resize=793%2C421&ssl=1" width="450" height="250">
</a>

## Taking information from different studies and statistics

We can discuss the investigation of technical factors and surveys of non-technical factors based on code reviews.

- **Investigation of technical factors:** Several correlations involving technical elements has been investigated. ***Thongtanunam*** et al. The study from *(2015a)* provided evidence that reviewers are less rigorous and find fewer defects on files with a high incidence of defects in the past, focusing on superficial aspects, such as coding standards, than functional aspects. In a more recent study *(Thongtanunam et al. 2016a)*, the same authors identified that bug fixes typically receive first feedback faster than new feature implementations. Focusing on the duration of the code review (in working days), some influencing factors were investigated. ***Bosu*** et al. *(2015)* concluded that patch size affects the time in most of the cases analyzed, while the priority of activities in the release plan and the software components affected only occasionally influenced some of the projects analyzed by ***Baysal*** et al. *(2016)*.

- **Investigation of non-technical factors:** As stated by ***Czerwonka*** et al. *(2015)*, the social network that emerges within companies or projects should be considered, as well as the specific skills of the auditors and their willingness and willingness to review. A social network analysis of three open-source projects *(Yang 2014)* revealed that the most active reviewers have central roles in those projects' social networks and are often some of the most important contributors. ***Bosu*** et al. *(2015)* noted, in one particular organization, that 75% of the feedback on code review comes from members of the author's team, but they are slightly less helpful than those of other teams. ***Baysal*** et al. *(2016)*, in turn, pointed out that when multiple organizations contribute to the same project, the code review can take longer to complete and have higher rejection rates depending on the organization that is creating or reviewing a patch—based on the analysis of several case studies.

[**CLICK HERE for looking at: Influence factors and review outcomes investigated by previous studies**](https://jserd.springeropen.com/articles/10.1186/s40411-018-0058-0/tables/1)

## Online Resources
- [Code review best practices](https://medium.com/cuelogic-technologies/code-review-process-best-practices-3eeecab26ded)
- [Guide to code review process](https://smartbear.com/learn/code-review/guide-to-code-review-process/#:~:text=Code%20Review%20is%20an%20integral,most%20effective%20quality%20assurance%20strategy)
- [Why code reviews matter](https://www.atlassian.com/agile/software-development/code-reviews)
- [Microsoft’s code review process](https://www.michaelagreiler.com/code-review-blog-post-series/)
- [Investigating the effectiveness of peer code review in distributed software development based on objective and subjective data](https://jserd.springeropen.com/articles/10.1186/s40411-018-0058-0)
