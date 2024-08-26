---
title: Stable Diffusion , Automatic1111 Guide
date updated: 2024-06-08 11:10 AM
---

Hello! This guide explains how to install Stable Diffusion with the Automatic1111 web interface. Stable Diffusion is an image generation model. Automatic1111 is an open-source project that allows us to use it easily with a web interface.

Things You Need to Know:
- Python and Git must be installed on your system.
- Nvidia is the recommended GPU. It can also run with AMD.
- Stable Diffusion does not work with AMD GPUs on Windows.
- To run Stable Diffusion with an AMD GPU, you must use Arch Linux or Arch Linux based distributions.

### Installation for Windows (Nvidia)
**Installation:**
1. Download the [`sd-webui.zip`](https://github.com/AUTOMATIC1111/stable-diffusion-webui/releases/tag/v1.0.0-pre) file from here.
2. Extract it to any location.
3. To update the web interface, double-click `update.bat`.
4. Then, to run the web interface, double-click `run.bat`. It will start downloading the necessary files. Once everything is downloaded, you will see the message `Running on local URL: http://127.0.0.1:7860`.

### Automatic Installation for Windows (Nvidia)
**Installation:**
1. Open your terminal in any folder and type `git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git` and press Enter.
2. Then double-click `webui-user.bat` to run it.

### Installation for Linux (AMD)
**Installation:**
1. Open your terminal and run the command: `git clone https://github.com/lshqqytiger/stable-diffusion-webui-directml && cd stable-diffusion-webui-directml && git submodule init && git submodule update`.
2. Then run `webui-user.bat`.
3. If you have 4-6GB VRAM, add `COMMANDLINE_ARGS=--opt-sub-quad-attention --lowvram --disable-nan-check` to `webui-user.bat`.

### Automatic Installation for Linux (Nvidia)
**Installation:**
**Step 1:**
First, install these according to your distribution:
- For Debian-based distributions: `sudo apt install wget git python3 python3-venv libgl1 libglib2.0-0`
- For Red-Hat-based distributions: `sudo dnf install wget git python3 gperftools-libs libglvnd-glx`
- For OpenSUSE-based distributions: `sudo zypper install wget git python3 libtcmalloc4 libglvnd`
- For Arch-based distributions: `sudo pacman -S wget git python3`

**Step 2:**
Open your terminal and run the command: `wget -q https://raw.githubusercontent.com/AUTOMATIC1111/stable-diffusion-webui/master/webui.sh`.
Then run `webui.sh`.

### Stable Diffusion Plugins to Check Out
- **OpenPose Editor**: Copies the position of a character/person in an image and generates it with your prompt, recommended to use with ControlNET.
- **QR Code Generator**: A QR Code generator for ControlNET.
- **Dreambooth**: An advanced model trainer.

There are many more plugins, but I recommend checking these out.

### Where to Find AI Models?
- [CivitAI](https://www.civitai.com/)
- [Hugging Face](https://huggingface.co/)

This guide was that much. I hope I was able to help. If I did, I'm glad :slight_smile:. If you encounter any issues during the download process, you can write under this post and check Automatic1111's [GitHub page](https://github.com/AUTOMATIC1111/stable-diffusion-webui).

### References
- [Automatic1111 GitHub](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
- My own experiences.