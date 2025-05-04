---
title: "What are AI Reasoning Models?"
subtitle: "o3 and o4-mini"
date: 2025-04-30T14:33:10+01:00
draft: false
toc: false
images:
tags:
  - Technical
  - AI
  - LargeLanguageModels
---

## Introduction

AI has moved beyond simple chatbots. New reasoning models tackle problems step by step before answering. They don’t just blurt out a reply, they pause and think like a human would.

This post will explore what these reasoning models are, highlighting how they differ from standard Large Language Models (LLMs) and identifying the types of tasks where they excel. We will also look at OpenAI's recent releases, o3 and o4-mini, and discuss how their improved capabilities are improving real-world problem-solving. Finally, we'll cover how and when you can expect to gain access to these powerful new models.

## What are Reasoning Models?

Reasoning models are advanced LLMs trained to solve complex problems by breaking them into steps. This allows them to outperform standard models that would simply predict the most likely output based on the sole input.

**Example:** Given a math question, a reasoning model doesn’t guess the answer. It breaks the problem into parts and solves each sequentially.

This method is called *Chain-of-Thought*.

In ChatGPT, you can see the model think through each step before it answers.

Thanks to this, reasoning models are much more accurate with logic, calculations, and deep research.

## When should you use reasoning models vs using a standard model?

The table below shows examples of how/where each type of model performs best.

| Standard LLMs          | Reasoning LLMs     |
|------------------------|--------------------|
| Explicit Tasks         | Ambiguous Tasks    |
| Cheaper Cost           | Accuracy           |
| Faster Execution Speed | Problem Solving    |

Use a reasoning model for tasks that need judgment, nuance, or multiple steps.
Use a standard model for simple tasks in which speed and cost matter more.

That’s all well and good, but what do those decisions look like practically?

| Task                                                       | Model     |
|------------------------------------------------------------|-----------|
| “How to average a column in Excel?”                        | Standard  |
| “Summarise this document.”                                 | Standard  |
| “Structure my presentation using the brief.”               | Reasoning |
| “Extract all email addresses.”                             | Standard  |
| “Compare job listings to compare requirements.”            | Reasoning |


Both models have their place. Choosing the right one for the task helps you get the best results.

## OpenAI’s o3 and o4-mini

OpenAI recently launched o3 and o4-mini, replacing the older o1 and o3-mini.
They’re trained better, so the base models perform quite well, but the real improvements come from their ability to use “tools” during reasoning. These tools allow the models to do things such as browsing the web, running code and more.

Let’s say you’re at the back of a classroom and you take an image of the problem that a professor scribbled on a whiteboard. A reasoning model might take the following steps:

1. Zoom in on the problem on the whiteboard (using the image manipulation tool).
2. Look up the method to solve it (web search).
3. Solve it (run Python code, based on the method, and give the answer to the user).

These models think, then act. They chain steps across tools to solve even more complex tasks than what they were previously capable of.

## Other Reasoning Models

I’ve focused on o3 and o4-mini (as they’re new and shiny) BUT there are other options.

DeepSeek-R1 generated headlines a few months ago by competing with OpenAI’s o1 model. It had some worrying bias in its training but you are able to host and run it locally. 

This allows you to train it do anything you want. People have already trained the bias out of it, and you can access those models here: https://huggingface.co/nicoboss/DeepSeek-R1-Distill-Llama-70B-Uncensored-v2-Unbiased

Rumors are currently circulating about DeepSeek-R2 which I imagine will again compete with OpenAI’s forefront models.

There’s also Gemini 2.5, Llama 4 and many other options.

## Conclusion

In conclusion, AI reasoning models represent a significant leap beyond traditional LLMs. By breaking down complex tasks and working through problems step-by-step, they offer improved accuracy in logic, calculations, and in-depth analysis. 

While standard LLMs remain valuable for simpler, faster tasks, reasoning models excel in scenarios requiring judgment, nuance, and multi-step problem-solving. As these models become more useful and more widely accessible, they are set to further transform how we approach and solve complex problems with AI.

## Additional Information

If you’d like more information on how reasoning models work, their use cases and more. I’d recommend taking a look at the OpenAI docs. https://platform.openai.com/docs/guides/reasoning-best-practices

For more information on the o3 and o4-mini models particularly, especially from a technical perspective, see OpenAI’s official post: https://openai.com/index/introducing-o3-and-o4-mini/

