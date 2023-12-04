# GPT

ChatGPT is a natural language processing tool driven by AI technology that allows you to have human-like conversations and much more with the chatbot.
The language model can answer questions and assist you with tasks, such as composing emails, essays, and code


### step 1

### Add OpenAI NuGet

To integrate ChatGPT, the initial step involves installing the OpenAI C# SDK. 
This can be accomplished by executing the following command Ctr Shift P ,, then search Open Nuget ,
and the install  OpenAI.


### Step #2

### Get API key

In order to be able to call and authenticate to the OpenAI API, it is necessary to generate a unique API key.

To do this:

  

• Visit: https://platform.openai.com/account/api-keys

• Log in

• Create your API Key by clicking on "Create new secret key" button.


### Step #3

### Instantiate OpenAI

After successfully installing the OpenAI C# SDK, the next step is to initialize it by providing your OpenAI API key. To accomplish this, create an instance of the OpenAI class and pass your API key as a parameter.

### Step #4

### Call the API

In order to call the API and get a response to the prompt we set, it is necessary to call the **CreateCompletionAsync()** method, which accepts the following parameters:

  

**1. prompt**  
A **required string parameter** that specifies the text prompt for which the API will generate a completion.

  

**2. model**  
A **required string parameter** that specifies the name of the OpenAI model to use for generating the completion. In this case, it is used the **text-davinci-003 model**.

  

**3. max\_tokens**  
An **optional integer parameter** that controls the maximum number of tokens (words or symbols) in the generated completion. If set to a low number, the completion will be shorter and more concise. If set to a higher number, the completion will be longer and more detailed.

  

**4. temperature**  
An **optional floating point parameter** - that controls the "creativity" or randomness of the generated completion.
A higher temperature value will result in more diverse and unpredictable output, whereas a lower temperature value will result in more conservative and predictable output.
In general, a temperature value between 0.5 and 1.0 tends to produce the most interesting and varied results, while a temperature value closer to 0 tends to be more predictable and safe.
