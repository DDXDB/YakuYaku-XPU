# 此变体：
添加支持XPU（Intel-GPU）

代码确认没有问题可以运行

目前无法确定部署Torch+XPU方法

建议参考[torch-test-xpu](https://github.com/Stanley5249/torch-test-xpu)部署

## Models
[台版轻小说翻译模型v1.2（日本語 → 繁體中文）](https://drive.google.com/file/d/1eUh7J6WOEujLrQSBO1gV6tpbLMvzIkRF/view?usp=sharing)

[A better practice](https://huggingface.co/sakuraumi/Sakura-13B-Galgame) on the same dataset produced by [@SakuraUmi](https://github.com/pipixia244)

[台版轻小说翻译模型v1.0（繁體中文 → 日本語）](https://drive.google.com/file/d/1PJRP5ucEeicvc-p7cXwaTWOU3mU4ozXt/view?usp=sharing)

[轻小说翻译模型（测试版）（日本語 → 한국어）](https://drive.google.com/file/d/1-wvmBLPzqbUM9iECAoWkBUJtVIp27GFm/view?usp=sharing)

## Sakura-13B-LNovel
Run `server.py` in [SakuraLLM/Sakura-13B-Galgame](https://github.com/SakuraLLM/Sakura-13B-Galgame/tree/dev_server)
```sh
python server.py \
    --listen "127.0.0.1:5000" \
    --model_name_or_path "SakuraLLM/Sakura-13B-LNovel-v0.8" \
    --trust_remote_code \
    --model_version 0.8 \
    --use_gptq_model \
    --no-auth
```
