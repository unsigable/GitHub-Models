# GitHub Models
Find and experiment with AI models for free.
    
    
#### [Prototyping with AI models](https://docs.github.com/en/github-models/prototyping-with-ai-models)   
Find and experiment with AI models for free.

***

#### [Responsible use of GitHub Models](https://docs.github.com/en/github-models/responsible-use-of-github-models)    
Learn how to use GitHub Models responsibly by understanding its purposes, capabilities, and limitations.

***


## Responsible use of GitHub Models
Learn how to use GitHub Models responsibly by understanding its purposes, capabilities, and limitations.

With GitHub Models, you build your understanding of AI model capabilities by experimenting with model settings and sending prompts through a chat interface. Additionally, you can directly interact with models through an SDK. Refer to a model's "Getting Started" tab for more information about how to use the SDK. Refer to a model’s "README" tab for more information on the model. Remember when interacting with a model you are experimenting with AI, so content mistakes are possible.

GitHub Models is designed to allow for learning, experimentation and proof-of-concept activities. The feature is subject to various limits (including requests per minute, requests per day, tokens per request, and concurrent requests) and is not designed for production use cases. GitHub Models employs a number of [content filters](https://azure.microsoft.com/en-us/products/ai-services/ai-content-safety). These filters cannot be turned off as part of the GitHub Models experience. If you decide to employ models through [Azure AI](https://ai.azure.com/github/model/docs) or a paid service, please configure your content filters to meet your requirements.

***


## Prototyping with AI models
*Find and experiment with AI models for free.*

If you want to develop a generative AI application, you can use GitHub Models to find and experiment with AI models for free. Once you are ready to bring your application to production, you can switch to a token from a paid Azure account. See the Azure AI documentation.

See also "Responsible use of GitHub Models."

### Finding AI models
To find AI models, go to GitHub Marketplace, then click  Models in the sidebar.

To view details about a model, click on the model's name.

### Experimenting with AI models in the playground
Note

The playground is in limited public beta and subject to change. To request access, join the waitlist.

GitHub Marketplace provides a free playground where you can adjust model parameters and submit prompts to see how the model responds.

To open the playground, go to GitHub Marketplace, then click  Models in the sidebar. Click on a model's name, then click  Playground.

To adjust parameters for the model, select the Parameters tab in the sidebar. To see code that corresponds to the parameters that you selected, switch from the Chat tab to the Code tab.

The playground is rate limited. See Rate limits below.

### Experimenting with AI models using the API
Note

The free API usage is in limited public beta and subject to change. To request access, join the waitlist.

GitHub provides free API usage so that you can experiment with AI models in your own application.

To learn how to use a model in your application, go to GitHub Marketplace, then click  Models in the sidebar. Click on a model's name, then click  Code.

The steps to use each model are similar. In general, you will need to:

Optionally, use the language dropdown to select the programming language.

Optionally, use the SDK dropdown to select which SDK to use.

All models can be used with the Azure AI Inference SDK, and some models support additional SDKs. If you want to easily switch between models, you should select "Azure AI Inference SDK". If you selected "REST" as the language, you won't use an SDK. Instead, you will use the API endpoint directly.

Either open a codespace, or set up your local environment:

To run in a codespace, click  Run codespace, then click Create new codespace.
To run locally:
Create a GitHub personal access token. The token should not have any scopes or permissions. See "Managing your personal access tokens."
Save your token as an environment variable.
Install the dependencies for the SDK, if required.
Use the example code to make a request to the model.

The free API usage is rate limited. See Rate limits below.

### Going to production
The rate limits for the playground and free API usage are intended to help you experiment with models and develop your AI application. Once you are ready to bring your application to production, you can use a token from a paid Azure account instead of your GitHub personal access token. You don't need to change anything else in your code. For more information, see the Azure AI documentation.

### Rate limits
The playground and free API usage are rate limited by requests per minute, requests per day, tokens per request, and concurrent requests. If you get rate limited, you will need to wait for the rate limit that you hit to reset before you can make more requests.

Low, high, and embedding models have different rate limits. To see which type of model you are using, refer to the model's information in GitHub Marketplace.

Rate limit tier	Rate limits	Free and Copilot Individual	Copilot Business	Copilot Enterprise
Low	Requests per minute	15	15	20
Requests per day	150	300	450
Tokens per request	8000 in, 4000 out	8000 in, 4000 out	8000 in, 8000 out
Concurrent requests	5	5	8
High	Requests per minute	10	10	15
Requests per day	50	100	150
Tokens per request	8000 in, 4000 out	8000 in, 4000 out	16000 in, 8000 out
Concurrent requests	2	2	4
Embedding	Requests per minute	15	15	20
Requests per day	150	300	450
Tokens per request	64000	64000	64000
Concurrent requests	5	5	8
These limits are subject to change without notice.

### Leaving feedback
To leave feedback about GitHub Models, start a new discussion or comment on an existing discussion in the [GitHub Community](https://github.com/orgs/community/discussions/categories/models).
