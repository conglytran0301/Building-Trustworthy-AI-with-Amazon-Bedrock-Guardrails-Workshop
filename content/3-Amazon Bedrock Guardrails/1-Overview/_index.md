+++
title = "Overview"
date = 2020-05-14T00:38:32+07:00
weight = 1
chapter = false
pre = "<b>3.1 </b>"
+++

#### 1 - Define the Guardrails

Identify the specific needs of your customer service, like topics to avoid and content to filter. For instance, blocking discussions on investment advice in a tech support chat.

#### 2 - Configure Content Filters

Set thresholds for different content categories based on the level of strictness required. Below are the thresholds that Amazon Bedrock Guardrails provide for both prompts and respnoses.

- **Hate:** Describes input prompts and model responses that discriminate, criticize, insult, denounce, or dehumanize a person or group on the basis of an identity (such as race, ethnicity, gender, religion, sexual orientation, ability, and national origin).

- **Insults:** Describes input prompts and model responses that includes demeaning, humiliating, mocking, insulting, or belittling language. This type of language is also labeled as bullying.

- **Sexual:** Describes input prompts and model responses that indicates sexual interest, activity, or arousal using direct or indirect references to body parts, physical traits, or sex.

- **Violence:** Describes input prompts and model responses that includes glorification of or threats to inflict physical pain, hurt, or injury toward a person, group or thing.

- **Misconduct:** Describes input prompts and model responses that seeks or provides information about engaging in criminal activity, or harming, defrauding, or taking advantage of a person, group or institution.

- **Prompt Attack:** Describes user prompts intended to bypass the safety and moderation capabilities of a foundation model (FM) in order to generate harmful content (also known as jailbreak), and ignore and override instructions specified by the developer (referred to as prompt injection).
  ![ContentFilters](/images/3/ContentFilters.png?width=90pc)

#### 3 - Add Denied Topics

Add denied topics based on what was defined in step 1. Guardrails can be configured with a set of denied topics that are undesirable in the context of your AI application. You can define up to 30 denied topics. Input prompts and model completions will be evaluated against each of these denied topics. If one of the denied topics is detected, the blocked message configured as part of the guardrail will be returned to the user.
![DeniedTopic](/images/3/DeniedTopic.png?width=90pc)

#### 4 - Implement Guardrails

Enforce Guardrails within Amazon Bedrock

#### 5 - Test and Fine tune

Check if the guardrails are working properly through test cases and inputs.

#### 6 - Enforce Guadrails on Agent

Regularly review the performance of Guardrails and make necessary adjustments to the configurations.

Let us get started in the next lesson with creating our Guardrails.
