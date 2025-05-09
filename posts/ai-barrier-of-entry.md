We are witnessing the next major wave of technological innovation.

To be fair the term itself, **AI (Artifital Intelligence)**, has had it's meaning stretched pretty thin in the last few years. It's been used to describe everything from a simple chatbot to a self driving car. However I think it's important to understand that such use of the term is extremely broad. Using it this way doesn't truly describe the space that we think of as "AI".

The term AI has become a misnomer. Currently it's not about intelligence, it's about automation. The AI that people are afraid of is not the AI we are building today. That is often considered **AGI (Artificial General Intelligence)**. AGI is the ability for a machine to learn and adapt to new situations. This displays some level of consciousness and is something that we are still a ways from achieving.

The AI models that are most prevalent today are **LLMs (Large Language Models)** and **Stable Diffusion**. I won't go into too much detail here about them but the gist of it is LLMs recieve a text prompt and output new text. On the other hand with Stable Diffusion you input a text prompt and it generates an image. These models both consist of a system of weights that, based on the input, guesses what the desired output is. It quite literally is attempting to determine what next "token" is most statistically likely to be "correct". The correctness being determined by what the model is trained on and how it is trained.

The key here is that the AI doesn't actually understand what it is producing; it is just really good at approximating an answer. In this way the AI we have today is more like a supercharged search engine. It has lots of indexed information and it is really good at compiling that information into something cohesive. But what is really game changing is how **easy** these tools are to use.

When **OpenAI** introduced **Chat-GPT** they gave anyone who could read and write the ability to leverage these models. That meant that no matter your profession, education, (and at the moment) income level you could ask a question and get an extremely human-like, and often correct, response. Even as a web developer I've felt this ease of access enter the industry.

The motivator for this post was actually my first experience using AI in a project. At **[Edlink](https://ed.link)** we wanted to enable people to transform datasets in any way they could think of. The first iteration of this was allowing people to write a custom function in **JavaScript**. You knew what the inputs were and what the output needed to be. Whatever happened in between was up to you. However upon revisiting this strategy we realized that this is exactly what these LLMs are good at. And so we set to work adding a no code option. First the user sends us a prompt describing what they want updated, added, or deleted. Then we make script with a boilerplate function, all the types from our data model, and a constructed prompt asking the model to modify the function to do what the user requested. This is simply an API request that returns a set of answers from which we pick the best and insert it as if the user wrote the function. 

> Here is an example of making a request for this to OpenAI

```javascript
axios.post('https://api.openai.com/v1/completions', {
    model: 'code-davinci-002',
    prompt: `function customFunction(data) {\n // ${prompt}\n`,
    suffix: '\nreturn data;\n}',
    temperature: 0.2,
    max_tokens: 512
});
```


And voila...you have a magic text box that you can give english instructions to do almost anything to your data.