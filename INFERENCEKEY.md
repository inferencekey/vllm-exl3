# inferencekey build of vllm-exl3

This branch (`inferencekey-thor`) is the exact source of the vllm-exl3 plugin that the inferencekey worker installs
for its `vllm-exl3` backend (DeepSeek-V4.1-Flash on two 96 GB GPUs with host-memory expert offload).

It is upstream [vcruz305/vllm-exl3](https://github.com/vcruz305/vllm-exl3) at `d3cfd394920360d69f820d2dc96f8292a9e10283`
plus one commit that applies Diffbot's `patches/vllm-exl3/exl3-thor.patch` from the Hugging Face repo
[diffbot/DeepSeek-V4.1-Flash-EXL3-3bpw-2x-RTX-PRO-6000](https://huggingface.co/diffbot/DeepSeek-V4.1-Flash-EXL3-3bpw-2x-RTX-PRO-6000)
at revision `a1cf1bd227a754aa7e2ca5c21652bfaf256ee8a5`. The patch is unchanged; `PATCHES-exl3-thor.patch` is a
verbatim copy for reference.

License: AGPL-3.0-only (`LICENSE`), as upstream and as Diffbot's patch. This repository is published to offer the
Corresponding Source of the modified version we serve over a network (AGPL-3.0 section 13). Measurement study and
build recipe: https://github.com/inferencekey/vllm-exl3-moe-hostoffload
