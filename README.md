**<h2>Addressing the Challenges for AI-Based Generation of Visually Consistent Sets of Map
Icons With LoRAicon</h2>**

For our LoRAicon output model can be dowloaded from this drive https://drive.google.com/drive/folders/1OT7lGlRBe5yqtyGjvLPPbSiAiMhvLU07?usp=sharing


<img width="274" height="233" alt="Cartoicon3" src="https://github.com/user-attachments/assets/41b7539e-c802-4c70-b908-7c345203ff79" />

<img width="273" height="233" alt="Cartoicon1" src="https://github.com/user-attachments/assets/eb9ee3d7-987b-44fb-8760-a9d908209db7" />

<img width="273" height="233" alt="Cartoicon2" src="https://github.com/user-attachments/assets/bd02a828-0732-462a-ab93-c9180fcbe8b5" />




**<h3>Source</h3>**
* Stable Diffusion XL 1.0 Base model (https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/resolve/main/sd_xl_base_1.0.safetensors)

* Kohya-ss GUI Portable version for training LoRA and setting hyperparameters by downloading via [Portable Kohya_ss GUI (LoRA)](https://github.com/serpotapov/Kohya_ss-GUI-LoRA-Portable/archive/refs/heads/main.zip) from https://github.com/serpotapov/Kohya_ss-GUI-LoRA-Portable.git based on Kohya-ss [https://github.com/bmaltais/kohya_ss?tab=readme-ov-file](https://github.com/bmaltais/kohya_ss.git)

* Fooocus GUI https://github.com/lllyasviel/Fooocus.git

  **<h4>Training through configuration</h4>**
 1. Install Kohya-ss GUI then add config file _config_lora-lr4ep2nd256.toml_ under configuration
 2. Assign image folder to caption for BLIP captions under Utilities
 3. Select _stabilityai/stable-diffusion-xl-base-1.0.safesensors_ as a pretrained model path
 4. Add images input, output and log directory
 5. Start training LoRA
  **<h4>Generating icons</h4>**
 1. Open Fooocus directly through the attached .ipynb or command line cd < yourFooocusfolder > and _!python entry_with_update.py --share --always-high-vram_
 2. Add file _sdxl_base_1.0.safetensors_ as a base model input, and file _testlr4ep2.safetensors_ LoRA input. Make sure that under path _..Fooocus\models\loras_ contains the LoRA model
 3. Add prompt for creating your prefer map icons.

**<h3>Acknowledgement</h3>**
This research was funded in part by a grant from Artificial Intelligence Privatstiftung Austria.
