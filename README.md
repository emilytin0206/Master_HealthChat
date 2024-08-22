# HealthChat
Our project aims to develop a locally-operated multilingual conversational AI that integrates several advanced technologies to
enhance mental health support. These include speech-to-text (STT), Chinese large language models (LLM), and text-to-speech
(TTS). Additionally, we have incorporated Differentiable Digital Signal Processing - Singing Voice Conversion (DDSP-SVC)
technology, enabling the AI to transform voice characteristics and respond in a comforting, familiar voice. Our model, finetuned on chinese psychotherapy datasets, can provide personalized counseling services

1. Speech Recording or Text Input: Users can record their speech via the web interface or input text through the message box.
2. Speech-to-Text: Whisper converts the recorded speech to text.
3. Generating System Response: The converted text is input into the Fine-tuned chinese LLM to generate a response.
4. Text-to-Speech: Bark converts the LLM-generated response into human-like speech.
5. Personalized Voice Training and Cloning: Users can train their desired voice using the DDSP-SVC through the interface, and replace the system's voice with it.

<img width="482" alt="image" src="https://github.com/user-attachments/assets/96c1c9e6-b4c4-4247-bdbf-40d6d5bb5d1e">

## Setup
The recommended version of python is 3.8 to avoid gradio error messages.

### Finetuned Taiwan-LLM-13B
We use our own mental dataset to finetune model , can download this model in here: https://huggingface.co/huangyt/module_v7

```
cd taiwan_llama/module
git Ifs install
git clone https://huggingface.co/huangyt/module_v7
```

### Run
```
python launch.py
```


### Demo
![image](https://github.com/user-attachments/assets/7f722bae-847b-458c-8097-08fbb1ae9b35)
