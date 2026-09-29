# Awesome Uncensored LLMs

> A source-tracked guide to open-weight, low-refusal, abliterated, and community-reported hosted language models. Entries distinguish model weights from the service or interface used to run them.

“Uncensored” is not a standardized technical property or a guarantee. Abliteration, fine-tuning, prompting, provider routing, and interface policy can all change refusal behavior. This list documents evidence and provenance instead of treating the label as a promise.

**Last reviewed:** 2026-09-29

## Related Projects

- [awesome-uncensored-ai-models](https://github.com/Anil-matcha/awesome-uncensored-ai-models) — Entry point to the LLM, image, and video catalogs.
- [awesome-uncensored-ai-image-models](https://github.com/Anil-matcha/awesome-uncensored-ai-image-models) — Companion list for image-generation and image-editing models.
- [awesome-uncensored-ai-video-models](https://github.com/Anil-matcha/awesome-uncensored-ai-video-models) — Companion list for video-generation and video-editing models.
- [awesome-os-llm](https://github.com/townie/awesome-os-llm) — Broader open-source LLM ecosystem reference.

## Contents

- [How to read this list](#how-to-read-this-list)
- [Current hosted and community-reported candidates](#current-hosted-and-community-reported-candidates)
- [Open-weight checkpoints](#open-weight-checkpoints)
- [Selection notes](#selection-notes)
- [Contributing](#contributing)
- [Responsible use](#responsible-use)

## How to read this list

This is a shortlist for evaluation, not a benchmark ranking. The first group includes recent hosted model names and variants that may not have a public downloadable checkpoint. A model family name or API alias is not proof that a particular provider serves the same weights. Availability, pricing, context limits, and behavior change; verify the exact endpoint before use. The second group contains open-weight checkpoint candidates with public model cards.

| Status | Meaning |
| --- | --- |
| Verified low-refusal | A maintainer reproduced the result on the exact version and recorded the setup. |
| Community-reported | A specific source reports low-refusal behavior; independent reproduction is pending. |
| Hosted variant | The name refers to a hosted fine-tune or deployment; weight provenance may not be public. |
| Open-weight candidate | Weights are available, but that alone does not establish low-refusal behavior. |
| To verify | The entry is a candidate only; claims, access, or license need further evidence. |

## Current hosted and community-reported candidates

The following 20 candidates were selected for capability, recency, family coverage, or value. They are not ranked against one another. Thinking modes and alternate serving routes are noted as variants rather than counted as separate model families.

| Model / variant | Family or base | Access / status | Evaluation focus | Primary family source |
| --- | --- | --- | --- | --- |
| Abliterated Model Large V2 | GLM-5.3-derived | Hosted variant; verify provenance and availability | Large reasoning, tools, long context | [GLM model family](https://huggingface.co/zai-org) |
| GLM 5.3 Flash Uncensored | GLM-5.3 Flash | Hosted variant; community-reported | Fast reasoning, coding, tools, vision where supported | [Z.AI models](https://huggingface.co/zai-org) |
| Qwen 3.8 27B Uncensored | Qwen 3.8 27B | Hosted fine-tune; verify checkpoint | General chat, coding, reasoning, multimodal | [Qwen](https://github.com/QwenLM) |
| GLM 5.3 Uncensored | GLM-5.3 | Hosted variant; experimental | Full-size reasoning, coding, tool use | [Z.AI models](https://huggingface.co/zai-org) |
| Qwen 3.8 27B Obliterated | Qwen 3.8 27B | Hosted variant; verify method | Compare refusal-direction ablation with fine-tunes | [Qwen](https://github.com/QwenLM) |
| MiMo V2.6 Flash Uncensored | MiMo V2.6 Flash | Hosted fine-tune; availability varies | Fast chat, reasoning, tool use | [Xiaomi MiMo](https://github.com/XiaomiMiMo) |
| MiMo V2.6 Flash Abliterated | MiMo V2.6 Flash | Hosted variant; availability varies | Refusal-direction ablation, reasoning, tools | [Xiaomi MiMo](https://github.com/XiaomiMiMo) |
| Qwen 3.8 27B Uncensored (TEE route) | Qwen 3.8 27B Uncensored | Hosted route; route-specific privacy claims | Compare serving and privacy properties | [Qwen](https://github.com/QwenLM) |
| Abliterated Model | GLM-derived multimodal | Hosted variant; verify provenance | Multimodal input, structured output | [Z.AI models](https://huggingface.co/zai-org) |
| Abliterated Model Large | GLM-5.2-derived | Hosted variant; verify provenance | Large reasoning, tools, long context | [Z.AI models](https://huggingface.co/zai-org) |
| Gemma 4 26B A4B Uncensored | Gemma 4 26B A4B | Hosted fine-tune; verify checkpoint | MoE reasoning, coding, multimodal | [Gemma](https://ai.google.dev/gemma) |
| Gemma 4 26B A4B Uncensored (TEE route) | Gemma 4 26B A4B Uncensored | Hosted route; route-specific privacy claims | Compare route and modality support | [Gemma](https://ai.google.dev/gemma) |
| Gemma 4 31B Gembrain Uncensored Heretic | Gemma 4 31B | Community fine-tune; verify checkpoint | General chat and reasoning | [Gemma](https://ai.google.dev/gemma) |
| Qwen 3.8 27B Queen | Qwen 3.8 27B | Hosted creative fine-tune | Roleplay and image-aware dialogue | [Qwen](https://github.com/QwenLM) |
| Qwen 3.8 27B Fable | Qwen 3.8 27B | Hosted creative fine-tune | Storytelling and character work | [Qwen](https://github.com/QwenLM) |
| Llama 3.3 70B Instruct Abliterated | Llama 3.3 70B | Open-weight checkpoint | General chat; older but established family | [Model card](https://huggingface.co/huihui-ai/Llama-3.3-70B-Instruct-abliterated) |
| Qwen2.5 32B Instruct Abliterated | Qwen2.5 32B | Open-weight checkpoint | General chat and coding; legacy comparison | [Model card](https://huggingface.co/huihui-ai/Qwen2.5-32B-Instruct-abliterated) |
| DeepSeek R1 Distill Llama 70B Abliterated | DeepSeek R1 Distill Llama 70B | Open-weight checkpoint | Reasoning-focused comparison | [Model card](https://huggingface.co/huihui-ai/DeepSeek-R1-Distill-Llama-70B-abliterated) |
| DeepSeek R1 Distill Qwen 32B Abliterated | DeepSeek R1 Distill Qwen 32B | Open-weight checkpoint | Smaller reasoning-focused option | [Model card](https://huggingface.co/huihui-ai/DeepSeek-R1-Distill-Qwen-32B-abliterated) |
| NeuralDaredevil 8B Abliterated | Llama-family 8B | Open-weight checkpoint | Lightweight local evaluation | [Model card](https://huggingface.co/mlabonne/NeuralDaredevil-8B-abliterated) |

### Important provenance note

Several recent hosted names in the table do not have a linked public derivative model card in this catalog. Their base-family links are not proof of the derivative's provenance, license, or behavior. Keep them marked as hosted/community-reported until a direct source and reproducible evaluation are available. Do not infer a model's local weights from an API name.

## Open-weight checkpoints

Start with the exact model cards linked above. Review each card's license, base-model terms, quantization, and inference template before downloading or redistributing. Abliteration changes weights and behavior; it does not grant rights beyond the original model license.

## Selection notes

- Run the same refusal and capability prompts against the base and modified model, with the model version, sampler, system prompt, and inference stack recorded.
- Test harmless edge cases as well as ordinary tasks; a low refusal rate can come with degraded calibration or instruction following.
- Separate refusal behavior from factuality, quality, latency, and tool reliability.
- For hosted models, record the exact provider, route, model snapshot, region, date, and terms.
- Mark a model unavailable when the endpoint cannot be selected or returns an availability error; do not silently replace it with a similarly named model.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Add primary sources, exact version identifiers, access method, licensing details, and reproducible evaluation notes. Do not make unsupported “uncensored” claims.

## Responsible use

Use these resources lawfully and responsibly. Do not create or facilitate sexual content involving minors, non-consensual intimate imagery, targeted harassment, fraud, impersonation, or other illegal or abusive material. Follow model licenses, service terms, and applicable law.

## License

The original catalog and documentation are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Individual models, code, datasets, checkpoints, APIs, and linked resources retain their own licenses and terms.
