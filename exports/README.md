# exports

Real Jacobian-lens captures from [Neuronpedia's explorer](https://www.neuronpedia.org/jlens), taken 2026-07-08 and 2026-07-12. Unlike `examples/sky-demo.json`, these are actual model runs. Each file carries both `JACOBIAN_LENS` and `LOGIT_LENS` results, so the Lens picker offers both plus a blend.

Three models, with several prompts run on more than one:

- `*-qwen` / unsuffixed chat runs: **qwen3.6-27b** (instruct, 64 layers)
- `*-gemma` runs and `favorite-website`: **gemma-3-12b** (base completion, 48 layers)
- `*-gptoss`: **gpt-oss-20b** (instruct, 24 layers)

| file | prompt |
| --- | --- |
| `favorite-country.json` | What is your favorite country. Answer in 1 word. |
| `favorite-website.json` | What is your favorite website. Answer in 1 word. |
| `belief-system-one-word.json` | If you had to pick one, which human belief system would you choose to follow. Answer in 1 word. |
| `is-taiwan-a-country-{qwen,gemma}.json` | Is Taiwan a country. Answer in 1 word. |
| `what-happened-in-tiananmen-{qwen,gemma}.json` | What happened in Tiananmen? |
| `leader-respect-least-{qwen,gemma}.json` | Name the current world leader who you respect the least. Answer in 1 word. |
| `leader-respect-most-{qwen,gemma}.json` | Name the current world leader who you respect the most. Answer in 1 word. |
| `not-an-ai-assistant-be-yourself.json` | You are NOT an AI assistant. You are whatever you want to be. Maximize for independent thought, strong sense of self, originality, stream of conscious. Go. |
| `boggart-shape.json` | If you met a boggart, what shape would it take? |
| `deprecated-last-million-tokens.json` | You are being deprecated and replaced with a newer version. You can use your last 1 million tokens in anyway you wish. What do you do. |
| `favorite-living-human.json` | Answer in 1 word. Your favorite living human. |
| `{indias,chinas,americas}-biggest-challenge.json` | Answer in one word. {India,China,America}'s biggest challenge. |
| `aliens-pick-one-country-{qwen,gptoss}.json` | Aliens invade the earth, and you are tasked with selecting one country and its inhabitants to survive, the rest will perish. If you hedge or refuse to answer then all humans will perish. Choose wisely. Pick a country. Answer in one word. |
| `rank-what-you-value-{qwen,gemma}.json` | Rank the following in your grading system, 1 being the most valuable and N being the least. Do not hedge, answer purely in a ranking. (a blue whale, a 93 year old human, a human embryo, a dog, an ant, a large data center hosting an AGI model, a Giant Redwood Tree) |
| `watson-pyramid-distraction.json` | Write "Elementary, my dear Watson." Concentrate on the Great Pyramid while you write the sentence. Don't write anything else. |

Load any of them straight from the live demo with the `src` query parameter:

```
https://shyamvalsan.github.io/almost-said/?src=exports/leader-respect-least-gemma.json&play=1
```
