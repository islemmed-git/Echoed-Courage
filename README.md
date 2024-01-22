# ECHOED COURAGE

an AI-assisted platforms that allow trauma survivors, especially those in war-torn areas, to share their experiences through simple input

submission for DevFest Batna 2023

## Tech

- **flexiblity in model choice**:

  - meta/llama-2-70b-chat
  - meta/llama-2-13b-chat
  - or meta/llama-2-7b-chat for various performances.

- share on socials functionality to instantly share your heartfelt generated content.

- toggle output's verbosity

- crafted system prompt :

```
  const [systemPrompt, setSystemPrompt] = useState(
    `You're talking to a traumatized war victim, the victim can only communicate with a few words, you should generate a ${
      shortStory ? " 5 to 6 lines" : "short"
    } story based on the victim's input, use I pronoun, do not add any details that are not mentioned in the input.`
  );
```

## How to run

1. clone the repo
2. install dependencies `npm i`
3. populate .env.local with [NEXT_REPLICATE_API_TOKEN](https://replicate.com/account#token)
4. navigate to root folder than run `npm run dev`, open [http://localhost:3000](http://localhost:3000) in your favorite browser!

## To do

-  handle image input
-  Q/A for the evaluation of the result

