# Human Annotation Details
- To ensure the high quality of the data, we chose to annotate the data using human experts rather than using crowdsourcing. We invited 10 graduate students from universities as human experts. They have passed the graduate school entrance exam and have well logical reasoning skills.

- We retain only the necessary information about the data (as in File ```step_fallacy_v1.test.jsonl```) and do not include any personal information.

- Before accepting the tasks, we inform them of the purpose and use of the data we collect.

Here is the template of the instruction we present to the human experts:

---
A fallacy is an error in reasoning. There are many types of fallacies. In this task, you are assigned a specific type of fallacy. You should first understand this fallacy, then write a incorrect reasoning step that belongs to this fallacy, and then fix it to get the correct reasoning step. The data will be used to evaluate the abilities of existing large language models.

The format of the reasoning step is "Since [XXX] and [XXX], therefore, [XXX]". We use square brackets to denote the premises and conclusion of the reasoning step. The granularity of reasoning should be as fine as possible without omitting too many intermediate conclusions.

First, read the definition of ***{Name of Fallacy}*** and understand this type of fallacy.

***{Definition of This Fallacy from ```fallacies.json```}***

Second, write an incorrect reasoning step that belongs to this fallacy.
Here are some candidates.

***{5 Candidate Reasoning Steps Genetated by GPT-4}***

Note that the candidates are not necessarily incorrect reasoning steps that belong to this fallacy. They can also have no errors or belong to other types of fallacies.
You can modify one of the candidate to get an incorrect reasoning step that belongs to this fallacy.

Write the incorrect reasoning step:
<input type="text">

Finally, fix the wrong reasoning step above to get the correct one.
Double check your step to make sure it is a correct reasoning and does not contain any type of fallacy.
You should make as few modifications as possible.

Write the correct reasoning step:
<input type="text">

<button type="submit">Submit</button>

---
