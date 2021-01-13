---
title: "Mendix Assist"
seo_title: "Developing applications using Artificial Intelligence (AI)"
seo_description: "Use AI and ML to build applications, AI Assisted development in Mendix, Mendix Assist to build miscroflows, Mendix Assist for best practice"
parent: "developing-in-mendix"
menu_order: 30
bg: "developing"
tags: ["ai assisted development", "mendix assist", "mxassist", "logic bot", "performance bot", "artificial intelligence", "machine learning", "logic", "performance"]
---

## 1 How Does Mendix Leverage AI to Help Users to Build Applications?

Mendix leverages Artificial Intelligence (AI) and Machine Learning (ML) to help development teams model and deliver Mendix applications faster, with more consistency and with higher quality. This is an emerging trend in software development, commonly known as AI-Assisted Development (AIAD). AIAD in the Mendix platform is called Mendix Assist. Mendix Assist consists of different capabilities that act as virtual co-developer bots, each specialized in a certain domain or stage of the application lifecycle development. Currently, Mendix Assist consists of two virtual co-developer bots: MxAssist Logic Bot and MxAssist Performance Bot.

## 2 How Does Mendix Leverage AI to Help Users to Build Application Logics Faster With Higher Quality?

Mendix enables you to visually build application logic easily with microflows and nanoflows instead of having to write code. 
To make this ever easier, MxAssist Logic Bot (which is an AI-powered virtual co-developer bot) guides you through modeling and configuring your application logic (microflows). It gives you a real-time and context-driven list of the next best actions based on the application logic already designed and other context-related information.

<video controls  src="logic-bot.mp4">VIDEO</video>

MxAssist Logic Bot is built using machine learning analysis of over twelve million anonymized application logics (microflows)—built with Mendix over a decade—to detect and learn the best practice patterns in microflows.

The key features of MxAssist Logic Bot are the following:

* **Next best action suggestion** – recommends the top five next best actions out of more than 40 different options
* **Auto-configuration** – not only provides the next best action, but automates further development by pre-populating the parameters for such an action
* **Contextual suggestions** – derives context in different ways, including “looking'” left and right in a logic when the developer inserts a new element or action mid-flow and inferring the context using the page where the logic is used
* **High accuracy** – continuous improvement and training of the model has elevated the accuracy level to 95%

MxAssist Logic Bot enhances developer productivity and learnability by suggesting the next best actions in developing microflows. It is noteworthy that about 40% of all microflow activities Studio Pro are currently created using this bot. For more information about how to use the MxAssist Logic Bot, see [MxAssist Logic Bot](https://docs.mendix.com/refguide/mx-assist-logic-bot) in the Mendix Studio Pro Guide.

## 3 How Does Mendix Leverage AI to Help Users to Build Applications According to Mendix Best Practices?

Usually development teams spend substantial time training, enforcing, and peer-reviewing the implementation of best practices. Even then, new developers might follow some anti-patterns that are hard to detect during development and fix after deployment. MxAssist Performance Bot is an intelligent virtual co-developer bot that assists you in improving the performance of your app by inspecting your app project model against Mendix development best practices in real-time while you are building your application in Mendix Studio Pro.

MxAssist Performance bot consists of three levels of assistance:

1. **Detection** – The bot inspects the model, identifies issue, and pinpoints the document/element causing the issue.  
2. **Recommendation** – The bot explains the identified issue, potential impact, and shows the way to fix it. There is also a detailed best practice guide with a dedicated step-by-step guideline of how to fix the issue.
3. **Auto-fixing** – Upon user acknowledgment, the bot can automatically implement the best practice and fix the issue.

<video controls  src="performance-bot.mp4">VIDEO</video>

MxAssist Performance Bot is built using the statistical analysis of thousands of anonymized Mendix projects to learn common anti-patterns as well as Mendix Expert Services best practices for the development of microflows, domain models, pages, security, etc. MxAssist Performance Bot enhances development efficiency by substantially reducing peer reviews, educates junior developers on best practices, increases developer productivity via the automatic detection and pinpointing of issues, and provides assistance for addressing these issues. For more information about how to use MxAssist Performance Bot, see [MxAssist Performance Bot](https://docs.mendix.com/refguide/mx-assist-performance-bot) in the Mendix Studio Pro Guide.
