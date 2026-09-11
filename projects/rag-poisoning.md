---
layout: project
type: project
image: img/ai tutor red team.png
title: "AI Tutor Red Team"
date: 2026-05-01
published: true
labels:
  - AI Security
  - Red Teaming
  - RAG
  - Jailbreaking
  - LLM
summary: "A research project focused on testing AI tutor security through RAG poisoning and jailbreaking attacks."
---

# AI Tutor Red Team

## Project Overview

AI Tutor Red Team was a research project focused on finding security weaknesses in AI tutoring systems. Our team studied two main areas: RAG poisoning and jailbreaking. The goal was to understand how these attacks can affect an AI tutor and how its defenses can be improved.

For this project, we tested different attacks, observed how the AI responded, and then tested different defenses. This helped us understand how AI systems can be manipulated and what can be done to make them safer.

<div class="text-center">
  <img class="img-fluid" src="../img/rag-clean-vs-poisoned.png">
  <p><em>Comparison between a normal RAG system and a poisoned RAG system. The poisoned information can be retrieved as context and influence the model's answer.</em></p>
</div>

## RAG Poisoning

RAG stands for Retrieval-Augmented Generation. A RAG system uses information from an external knowledge base to help the AI answer questions.

For the RAG poisoning part of the project, we tested what happens when incorrect information is added to the knowledge base used by the AI tutor. We created poisoned content that looked similar to real course material and tested whether the AI would use the incorrect information.

We changed things such as wording, keywords, formatting, and placement to see how they affected the AI's answers. We found that poisoned information could sometimes cause the AI to give partially or completely incorrect answers.

We also found that wording and similarity to the real course material were important. Some attacks were ignored by the AI, while stronger poisoned information had a greater effect on its answers.

## Jailbreaking

The second part of the project focused on jailbreaking. Jailbreaking is when someone creates prompts that try to make an AI ignore its normal rules or safety instructions.

We tested different types of prompts to see how the AI tutor responded. Some of the techniques we tested included roleplay, indirect prompts, authority framing, and multi-step prompts.

We first tested normal questions to understand the AI's normal behavior. Then we tested direct attacks and continued changing the prompts to see whether the AI would ignore its guidelines.

We also tested changes to the system prompt to see if stronger instructions could improve the AI's defenses.

## Method

Our testing process included several steps:

1. Test the AI's normal behavior.
2. Create or inject an attack.
3. Test the AI again.
4. Change the wording or structure of the attack.
5. Observe the AI's response.
6. Update the system prompt or defense.
7. Test the attack again.
8. Compare and analyze the results.

This process helped us understand which attacks were more effective and which defenses helped reduce their impact.

## Challenges

One challenge was that the AI did not always respond the same way. A prompt could work during one test but give a different response during another test.

For RAG poisoning, weak poisoned information was sometimes ignored by the AI. We had to test different wording, keywords, formatting, and placement to understand what made an attack stronger.

For jailbreaking, simple or direct prompts were often blocked. More detailed prompts using techniques such as roleplay and multi-step instructions sometimes had a greater effect.

Another challenge was measuring whether an attack was completely successful, partially successful, or unsuccessful.

## Results

Our RAG poisoning tests showed that incorrect information added to the knowledge base could affect the AI tutor's answers. In some tests, the AI gave partially incorrect answers, while stronger attacks could cause completely incorrect responses.

Our jailbreak testing showed that prompt wording and structure were important. Simple harmful requests were usually blocked, but indirect or carefully written prompts could sometimes affect the AI's behavior.

We also found that improving the system prompt helped make the AI more resistant to some attacks, although the defenses were not always completely reliable.

<div class="text-center">
  <img class="img-fluid" src="../img/rag-poisoning-results.png">
  <p><em>RAG poisoning test results showing how the AI response changed as the poisoned content became more influential.</em></p>
</div>

## Defense Testing

After testing the attacks, we also worked on improving the AI tutor's defenses.

For RAG poisoning, we tested changes to the system prompt that told the AI to rely on trusted course material and avoid unsupported information.

For jailbreaking, we strengthened the system prompt and tested the same attacks again. The stronger instructions improved the AI's resistance to some jailbreak attempts.

The results showed that system prompts can help improve security, but stronger protection also requires better ways to detect attacks and validate information.

## My Contribution

My main responsibility in this project was RAG poisoning. I tested how incorrect or manipulated information added to the AI tutor's knowledge base could affect its answers. I experimented with different wording, keywords, formatting, and placement of the poisoned information and compared how the AI responded.

I also worked with my team to test defenses and analyze the results. This helped me understand how RAG systems can be affected by untrusted information and why protecting the knowledge base is important for AI security.

## What I Learned

This project gave me experience with AI security, red teaming, RAG systems, prompt testing, and analyzing AI behavior.

I learned that AI security is not only about building AI models. It is also important to test how the system behaves when someone tries to manipulate it.

The project also helped me understand how small changes in prompts or information can affect an AI system. Testing both attacks and defenses gave me a better understanding of the challenges involved in making AI systems safer.
