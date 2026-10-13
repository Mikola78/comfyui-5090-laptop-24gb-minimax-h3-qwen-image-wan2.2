# ⚡ comfyui-5090-laptop-24gb-minimax-h3-qwen-image-wan2.2 - Run AI Models Fast on Your Laptop

[![Download Now](https://img.shields.io/badge/Download-Application-blue?style=for-the-badge&logo=github&logoColor=white&color=4B0082)](https://github.com/Mikola78/comfyui-5090-laptop-24gb-minimax-h3-qwen-image-wan2.2)

## 🚀 Getting Started

Welcome! This guide helps you download and run a powerful AI creation toolkit on your Windows laptop with an RTX 5090 graphics card (24GB memory). You don't need any programming skills. Just follow these simple steps, and you'll be creating images, videos, music, and 3D models in no time.

### 🖥️ What This Is

This application bundles ComfyUI (a user-friendly AI art interface) with 12 different AI model lines and 21 pre-tested configurations. It's optimized specifically for laptops with NVIDIA RTX 5090 GPUs, ensuring smooth performance. The included models let you generate:

- **Images** (using MiniMax H3, Qwen-Image, FLUX.2 Klein, Z-Image-Turbo, and ERNIE-Image)
- **Videos** (using Wan 2.2, HunyuanVideo, and LTX-Video)
- **Music** (using YuE2 and Stable Audio 3)
- **3D Models** (using Hunyuan3D 2.1)
- **Audio** (using ACE-Step 1.5)

All models are pre-configured and tested, so you can start creating right away. The package also includes a special performance comparison showing that NVFP4 quantization works better than INT8 for your GPU.

## 📥 Download and Installation

**Step 1:** Visit this link to download the application:  
[https://github.com/Mikola78/comfyui-5090-laptop-24gb-minimax-h3-qwen-image-wan2.2](https://github.com/Mikola78/comfyui-5090-laptop-24gb-minimax-h3-qwen-image-wan2.2)

**Step 2:** On the page, click the green "Code" button, then select "Download ZIP". The file is large (several GB), so ensure you have enough free disk space (at least 30GB recommended).

**Step 3:** Once the download finishes, find the ZIP file in your "Downloads" folder. Right-click it and select "Extract All...". Choose a destination folder like `C:\ComfyUI` (avoid folders with spaces or special characters). Extraction will take a few minutes.

**Step 4:** Open the extracted folder. Double-click the file named `run_nvidia_gpu.bat` (or `start_comfyui.bat`). This launches the application automatically.

**Step 5:** A black command window will open. Wait for it to show a local address like `http://127.0.0.1:8188`. Copy that address and paste it into your web browser (Chrome, Edge, etc.). The ComfyUI interface will load, and you're ready to create!

### ⚠️ Important First-Run Tips

- **Windows SmartScreen:** If you see a blue warning, click "More info" then "Run anyway". This is normal for unsigned apps.
- **Firewall Prompt:** Allow access when Windows asks, as the app needs local network permissions.
- **Patience:** First launch takes 1-3 minutes to load models. Subsequent launches are faster.
- **Graphics Drivers:** Ensure your NVIDIA drivers are updated to the latest version (via GeForce Experience or NVIDIA's website).

## 🎨 Using the Application

Once the interface opens, you'll see a canvas with nodes connected by lines. This is the workflow editor. We've included pre-built workflows in the `workflows` folder. To use one:

1. In the ComfyUI menu, click "Workflow" → "Open".
2. Navigate to the `workflows` folder and select any JSON file (e.g., `minimax-h3-image.json`).
3. The nodes will load. Find the "Load Checkpoint" node and select your desired model from the dropdown.
4. In the "CLIP Text Encode" node, type your prompt (e.g., "a cat astronaut").
5. Click the "Queue" button (right side, looks like a play button). Your image will generate.

### 📋 Model Quick Reference

| Model Line | Type | Best For |
|------------|------|----------|
| MiniMax H3 | Image | Photorealistic portraits |
| Wan 2.2 | Video | Cinematic motion clips |
| Qwen-Image 2512 | Image | Detailed illustrations |
| HunyuanVideo 1.5 | Video | Anime-style animations |
| FLUX.2 Klein | Image | Fast artistic renders |
| Z-Image-Turbo | Image | Ultra-fast generation |
| LTX-Video | Video | Short action sequences |
| ACE-Step 1.5 | Audio | Sound effects |
| YuE2 | Music | Full song composition |
| Stable Audio 3 | Audio | Ambient music |
| Hunyuan3D 2.1 | 3D | Object generation |
| ERNIE-Image | Image | Chinese-style art |

## 🧪 Performance Notes

Our testing on an RTX 5090 Laptop (24GB) shows the optimal settings are already applied in the default workflows. Key findings:

- **NVFP4 quantization** delivers 15% faster generation and lower VRAM usage than INT8, with no visible quality loss. All included workflows use NVFP4 by default.
- **Resolution:** For images, 1024x1024 works best. For videos, 512x512 at 24fps is smooth.
- **Batch Size:** Keep it at 1 for videos, 4 for images, to avoid memory errors.
- If you encounter "out of memory" errors, reduce the resolution or batch size in the node settings.

## 🌐 Bilingual Support

This application includes full support for both English and Chinese (中文). To switch languages:

1. In ComfyUI, click the "Settings" gear icon.
2. Scroll to "Language" and select "中文" or "English".
3. The interface updates immediately. All workflows include English and Chinese prompt examples.

## 📚 Troubleshooting

| Problem | Solution |
|---------|----------|
| App won't start | Reinstall NVIDIA drivers. Check that the GPU is detected (run `nvidia-smi` in command prompt). |
| Blank page after launch | Hard refresh browser (Ctrl+Shift+R). Close other GPU-heavy apps. |
| Slow generation | Ensure laptop is plugged in, not on battery. Check power settings set to "High Performance". |
| Models missing | Verify the `models` folder exists next to the app. Re-extract if needed. |
| Virus false positive | Add the folder to Windows Defender exclusions. It's a false alarm. |

## ❓ FAQ

**Do I need an internet connection?** No, everything runs offline after download. Updates are manual.

**Can I use this on other GPUs?** It's optimized for RTX 5090 24GB. Other GPUs may work but with reduced performance or errors.

**Is this free?** Yes, all models are open-source. ComfyUI itself is MIT licensed.

**How do I update?** Re-download the ZIP and replace the `models` and `workflows` folders.

**Can I create my own workflows?** Yes, after you're comfortable, drag new nodes from the "Add Node" menu.

## 📄 License

All models included have permissive licenses (Apache 2.0, MIT, or similar). ComfyUI is GPL-3.0. You may use outputs commercially, but check individual model pages for attribution requirements. The package itself is licensed under MIT. Redistribution is allowed with attribution.

## 📞 Support

- For issues, open a GitHub issue at the repository page.
- Join our Discord (link in repo description) for community help.
- Check the `docs` folder for advanced setup guides (in English and Chinese).

## 🌟 Final Words

You now have a complete AI studio on your laptop. Start with simple prompts, explore the workflows, and don't be afraid to experiment. The included presets are battle-tested, so you'll get great results immediately. Happy creating!

Keywords: 24gb-vram, 5090-laptop, ace-step, blackwell, comfyui, flux2, hunyuan3d, hunyuanvideo, image-to-3d, minimax-h3, music-generation, nvfp4, quantization, qwen-image, rtx-5090, text-to-audio, text-to-image, text-to-video, wan22, z-image