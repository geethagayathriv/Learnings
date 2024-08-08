---
title : "How ChatGPT works technically"
date: 2024-08-08
categories: 
---

## Let's understand the working of ChatGPT

Released on November 30 2022,ChatGPT is one of the fastest growing app. Heart of ChatGPT is a Large Language model. The default model for ChatGPT is GPT-3.5 and it is capable of using GPT-4.

### What is a Large Language Model?

A LLM is a neural network based model that is trained on large volumes of text to make it capable enough to generate human text. An LLM is characterised by its size and the no.of parameters. GPT-3.5 has 175 billion parameters spread across 96 layers. GPT-3.5 is trained on large internet data of size 500 billion tokens and is capable of generating gramatically correct and semantically human-like outputs but, without proper training it is prone to generating harmful data.

## How do we make the model safe?

To make the model safer, we need the concept of prompt engineering. We can also make use of fine-tuning. Fine-tuning is the process of tuning a model that doesn't quite aline with the human values into a model that can be used by ChatGPT. This process is called Reinforcement Training from Human Feedback (RLHF).

## RLHF and chatGPT

From the top-view, Fine-tuned ChatGPT is trained on a reward model and based on the reward obtained, the policy is optimized using reinforcement learning's Proximal Policy Optimization(PPO).
It can be understood in these basic steps:
* A new prompt is sampled from the dataset.
* The policy generates an output.
* The reward model calculates a reward for the output.
* The reward is used to update the policy using Proximal Policy Optimization(PPO) algorithm.

## Give the input, get the output

The process of giving a prompt and getting an answer may seem easy but in reality, it's a bit more complicated.

### Conversational Prompt Injection

The ChatGPT model maintains the context of the conversation and the context is fed to the model every time a new prompt is entered. This enables the model to be context aware.

### Primary Prompt Engineering

These are pieces of instructions that guide the model's coversational tone.These are invisible to the user.

### Moderation API

This moderation API checks the content and blocks any unethical and harmful content if any. 