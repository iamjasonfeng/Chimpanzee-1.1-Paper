# Chimpanzee-1.1-Paper

[PDF](https://iamjasonfeng.github.io/Chimpanzee-1.1-Paper/chimpanzee_1_1_an_rps_trained_model_for_arc_agi_3.pdf)


Abstract

This paper documents Chimpanzee-1.1, my custom-trained model for ARC-AGI-3. Chimpanzee-1.1 is
a Qwen3.6-27B LoRA model trained with multimodal Direct Preference Optimization (DPO)[2] and a
four-stage Regressive Plasticity Schedule (RPS). Its chosen training trajectories come from Kimi K3
solving ARC Witness and ARC Interactive games normally, without being given the correct actions.
Each preference pair represents one exact pre-action state, its native image, a compact reasoning
summary, and one replay-verified action. I describe the curriculum with a child-adult analogy: Level 1
examples form a high-plasticity child phase, while later-level examples form a low-plasticity adult
phase. Although Chimpanzee-1.1 shares a base model and parts of its training infrastructure with
Gorilla-1.1, it is meaningfully different in data-generation method, training unit, curriculum, preference
construction, and context handling.
