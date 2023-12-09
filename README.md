# Deconstructing Hugging Chat

I started this repo as a place to kickstart a #30Days exploration of the Hugging Face Open-Source Chat application that is currently deployed at [https://huggingface.co/chat/](https://huggingface.co/chat/). As described in their [About](https://huggingface.co/chat/privacy) page, _"The goal of this app is to showcase that it is now possible to build an open source alternative to ChatGPT. 💪"_. 

## Hugging Face Chat Features

At a high level, it provides the UI and related interaction flows to support text inference and conversational experiences for generative AI applications. Looking closer, it has a number of interesting features that we can use or extend.
 - Easy deployment to a [Hugging Face Space](https://huggingface.co/docs/hub/spaces-overview)
 - Docker-based [chat-ui template](https://huggingface.co/new-space?template=huggingchat/chat-ui-template)
 - Work with open-source models (supported Llama 2 70B, CodeLlama 35B, Falcon 180B, Mistral 7B in Oct 2023)
 - UI built with Svelte Kit with code available in [open-source repo](https://github.com/huggingface/chat-ui)
 - Inference backend uses optimized [text-generation-inference](https://github.com/huggingface/text-generation-inference) on HuggingFace Inference API infra.
 - Can also be setup for local development - requires MongoDB database, Hugging Face token.
 - Can be used with any API server with OpenAI API compatability [using a custom endpoint](https://github.com/huggingface/chat-ui#running-your-own-models-using-a-custom-endpoint)
 - You can also build the app for production and [deploy to any server with a Svelte adapter](https://github.com/huggingface/chat-ui#building)

## Learning Objectives

For this #30Days Project, my learning objectives are:

1. Understand the Hugging Face platform and ecosystem
2. Understand the Hugging Face Chat experience - and compare to ChatGPT
3. Understand Hugging Face Chat SPACES deployment - requires payment
4. Understand Hugging Face Chat LOCAL deployment - requires MongoDB, HF key
5. Instrument the repo for GitHub Codespaces - establish consistent dev environment
6. Instrument the repo with GitHub Codepilot - explore and understand structure and codebase
7. Build and validate the Hugging Face Chat app locally - get experience working with an OSS LLM.
8. Deconstruct codebase to understand how app is constructed - get familiar with SvelteKit
9. Experiment with modifications or extensions to default experience and process
     - Use Azure CosmosDB for local MongoDB-compliant database
     - Deploy Chat-UI to Azure Static Web Apps using Svelte-Kit adapter
     - Get Chat-UI working with an Azure OpenAI endpoint usong custom endpoint capability.

## Dec 2023

Join me at the [Dec 2023 Global AI Conference](https://globalai.community/conference/) where I will talk briefly about this project and share some early insights and progress,

**Title**: 
Deconstructing Hugging Chat: Explore an open-source Chat UI for Generative AI Apps

**Abstract:**
Want to build a ChatGPT-like experience for your Generative AI use case but don't know where to start? What if you had an open-source project that was exploring the same goals, so you can learn from it and contribute back or transfer knowledge to your own development journey? How do you get started exploring it, especially if you are unfamiliar with the relevant programming framework or technology community? In this talk we'll look the "Hugging Chat" application from the HuggingFace community and deconstruct the open-source "Chat UI" project that powers it. We'll learn how the app is built and deployed, and how it can be customized to work with available LLMs, potentially in a local development environment. And we'll explore the value of tools like GitHub Codespaces and GitHub Copilot to help us navigate unfamiliar codebases with confidence, and even try to extend capabilities to suit our needs.

**Working Repo**
[Personal Fork of Chat-UI](https://github.com/nitya/huggingface-chat-ui-explore)

