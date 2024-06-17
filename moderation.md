# Moderation

### Moderation

In our interactions with AI applications, we often have stringent requirements in terms of content security, user experience, and legal regulations. At this point, we need the "Sensitive Word Review" feature to create a better interactive environment for end-users. On the prompt orchestration page, click "Add Function" and locate the "Content Review" toolbox at the bottom:

### Call the OpenAI Moderation API <a href="#call-the-openai-moderation-api" id="call-the-openai-moderation-api"></a>

OpenAI, along with most companies providing LLMs, includes content moderation features in their models to ensure that outputs do not contain controversial content, such as violence, sexual content, and illegal activities. Additionally, OpenAI has made this content moderation capability available, which you can refer to at [https://platform.openai.com/docs/guides/moderation/overview](https://platform.openai.com/docs/guides/moderation/overview).

Now you can also directly call the OpenAI Moderation API on Dify; you can review either input or output content simply by entering the corresponding "preset reply."

### Keywords <a href="#keywords" id="keywords"></a>

Developers can customize the sensitive words they need to review, such as using "kill" as a keyword to perform an audit action when users input. The preset reply content should be "The content is violating usage policies." It can be anticipated that when a user inputs a text snippet containing "kill" at the terminal, it will trigger the sensitive word review tool and return the preset reply content.

### Moderation Extension <a href="#moderation-extension" id="moderation-extension"></a>

Different enterprises often have their own mechanisms for sensitive word moderation. When developing their own AI applications, such as an internal knowledge base ChatBot, enterprises need to moderate the query content input by employees for sensitive words. For this purpose, developers can write an API extension based on their enterprise's internal sensitive word moderation mechanisms, specifically referring to [Moderation Extension](<.gitbook/assets/moderation extension>), which can then be called on Dify to achieve a high degree of customization and privacy protection for sensitive word review.

[PreviousCode-based Extension](<.gitbook/assets/code based extension>)[NextDiscovery](broken-reference)

Last updated 3 months ago
