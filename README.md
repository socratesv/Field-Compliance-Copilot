# Project Title

Field-Compliance-Copilot

## Summary

Field Compliance Copilot is an AI-assisted system that helps Field Officers retrieve regulatory guidance, assess evidence and prepare inspection reports while keeping compliance decisions under human control. This is a Building AI course project.

## Background

Field officers working in regulatory, environmental and infrastructure environments often need to make sense of information from many different sources while conducting inspections. These sources may include legislation, regulations, licence conditions, policies, operating procedures, previous inspection reports, equipment readings, photographs and other observations.

Typical environments that use Field Offices are many, from government to the private sector. Field Officers may work for the environment (EPA), Water Agencies, forestry, air-quality and meteorology, energy sector, warehousing, and many more...

Finding and interpreting the relevant information can be time-consuming, particularly when an officer is working in the field. The information available may also be incomplete or contradictory.

The main problems this project aims to address are:
  * Important regulatory information may be spread across multiple documents and systems;
  * Field officers may have limited time to search for relevant information during an inspection;
  * Observations, measurements and historical information may conflict with each other;
  * Considerable effort may be required after an inspection to convert field notes into structured reports; and
  * Conventional AI systems may provide confident answers even when there is insufficient evidence, therefore misleading outcomes.

My motivation for this project comes from my professional experience in enterprise architecture, data platforms, for utilities and government regulatory environments, combined with my interest in artificial intelligence.

I am particularly interested in how AI can assist people performing complex work without replacing their professional judgement, whilst improving the desired outcomes in quality, accuracy and timeliness. Components of the project, such as the Regulatory AI Navigator may also be used separately and made available publicly so that users may test their compliance by navigating the very complex regulatory frameworks in an easy to follow and understand way.

The central question for the project is:

Can AI help a Field Officer find relevant regulatory information, interpret available evidence and prepare a defensible report while ensuring that the final decision remains with a human? (In many cases, the evidence gather may be used for fine or to prosecute, so accuracy is very important)

In the case of Regulatory AI Navigator subsystem, can a Licensee self-assess their compliance to ensure that they are not breaching license conditions or regulatory obligations? 

## How is it used?

The Field Compliance Copilot would be a software application that could be used on a normal laptop, tablet or other mobile computing device.

A Field Officer could begin by receiving a job order or initiate an inspection by selecting a site, asset or activity. The system could then identify relevant inspection requirements and retrieve appropriate regulatory or procedural information and format them both in terms of a stepped workflow that the Field Office will need to enact and a report(s) for action.

During an inspection, the officer could enter observations such as:
  * measurements and meter readings;
  * notes and comments;
  * photographs;
  * observed equipment condition; and
  * other relevant evidence.

A Regulatory AI Navigator within the application would allow the officer to ask natural-language questions about the applicable regulations, procedures or license conditions. The system would retrieve relevant source material and provide an answer together with references to the original documents.

The AI could also identify inconsistencies in the available evidence.

For example, suppose a Water extraction license permits a maximum of 100 ML of water, while:
  * a meter suggests that 112 ML has been extracted;
  * telemetry data indicates 96 ML; and
  * a previous inspection identified a possible meter calibration problem.

The system should not simply conclude that a licence breach has occurred.

Instead, it should identify the inconsistency, explain why the evidence is inconclusive and recommend further investigation.

At the end of an inspection, the system could prepare a draft report containing observations, evidence, relevant regulatory references, issues requiring investigation and suggested follow-up actions.

The field officer would review, amend and approve the report.

The intended users would initially be regulatory or compliance Field Officers and their supervisors. People and organisations being inspected would also be affected, so transparency, accuracy and appropriate human oversight would be essential.

The Regulatory AI Navigator could also be made available for Licensees, so that they can check their compliance and ensure they are not breaching conditions or obligations and avoid fines or legal procecution.

## Data sources and AI methods

Depending on which component is used and who is deploying the Copilot, the Copilot would be loaded with organizational data, parameters, job data, etc. and also use publicly available regulatory information and synthetic inspection data. 

In the case of a publicly available system e.g. the Regulatory AI Navigator, no confidential or personal operational information is required so the sources will be primarily public data with the option to provide personal License data to assess compliance.

Possible data sources include:
  * legislation and regulations;
  * publicly available regulatory guidance;
  * policies and inspection procedures;
  * sample or synthetic licence conditions;
  * synthetic historical inspection reports;
  * equipment or environmental readings; and
  * photographs and field observations.

One of the main AI techniques would be Retrieval-Augmented Generation (RAG).

Instead of relying only on information learned by a language model during training, the system would search an approved collection of regulatory documents and provide the most relevant information to the language model when answering a question.

Embeddings and semantic search could be used to find document sections that are relevant to a question even when the user does not use exactly the same wording as the source document.

Natural language processing could also be used to convert unstructured field notes into structured observations and draft report content.

A later version could investigate image analysis for photographs taken during inspections and/or populate organisational portals with the required data.

The basic reasoning process would be:

  * Evidence → Retrieval → Inspection → AI analysis → Recommendation → Human decision

A particularly important feature would be the ability of the AI to recognise when the available evidence is insufficient or contradictory.

## Challenges

The Field Compliance Copilot would be a decision-support system and would not replace a regulator, inspector or other authorised decision-maker.

Important limitations include:
  * language models can generate incorrect or unsupported information;
  * regulatory documents can change over time;
  * retrieved information may be incomplete or irrelevant;
  * poor-quality input data can lead to poor recommendations; (this is a typical problem space)
  * photographs and measurements may be incorrectly interpreted;
  * confidential, personal or sensitive information must be protected;
  * regulatory decisions may depend on circumstances that cannot be represented completely in data; and
  * people may place too much trust in recommendations made by an AI system.

For these reasons, AI-generated conclusions should be traceable to their supporting evidence wherever possible.

The system should distinguish between:
  * facts contained in source material,
  * observations supplied by the user, and
  * inferences made by the AI.

Where the evidence does not support a conclusion, the preferred response should be “insufficient information” rather than an unsupported answer.

Human review would remain mandatory for significant regulatory decisions.

## What next?

The first practical version of the project could be a small prototype using one regulatory domain, such as Water compliance.

A test dataset of perhaps 20–30 synthetic inspection scenarios could be developed. Some cases would deliberately contain missing or conflicting evidence.

The prototype could then be evaluated using measures such as:
  * accuracy of information retrieved from regulatory documents;
  * accuracy of source citations;
  * ability to identify contradictory evidence;
  * frequency of unsupported AI statements or hallucinations;
  * ability to recognise insufficient evidence;
  * completeness of generated inspection reports; and
  * time required for a user to complete an inspection report.

A later version could incorporate speech-to-text, photographs, geographic information, operational data and off-line or intermittently connected operation. The last capability is very useful for remote locations where connectivity may be poor or non-existent.

The same approach could eventually be extended beyond water regulation to environmental regulation, infrastructure maintenance, utilities, safety inspections and other field-based activities.

The Regulatory AI Navigator could also potentially become a separate public-facing service that helps Licensees/citizens understand regulatory requirements using plain language and references to authoritative sources.

## Acknowledgments

This project concept was developed as part of the Building AI course by the University of Helsinki and Reaktor Innovations.

The project is also inspired by my professional experience with enterprise architecture, data platforms and processes for utilities and regulatory environments.

Any future prototype will use original, synthetic, publicly available or appropriately licensed data, code and other materials. 
Where open-source software, datasets, documents or Creative Commons material are used, the original authors and applicable licences will be acknowledged.
