# quickkeys-tools

這個專案在 GitHub 的雲端 Mac / Windows 編譯機上，自動編譯一份**完全獨立**的 `whisper-cli`（語音辨識程式），並放在 Releases 供下載。它不需要 Homebrew，也不依賴其他函式庫。

QuickKeys（Premiere 插件）第一次使用「自動字幕」時，會自動下載：

| 檔案 | 來源 |
|---|---|
| `whisper-cli-darwin-arm64.gz` / `-darwin-x64.gz` / `-win32-x64.gz` | 本專案的 Releases |
| `ffmpeg` | [eugeneware/ffmpeg-static](https://github.com/eugeneware/ffmpeg-static) |
| 語音模型 | [ggerganov/whisper.cpp（Hugging Face）](https://huggingface.co/ggerganov/whisper.cpp) |

## 重新編譯
打開 **Actions → Build whisper-cli for QuickKeys → Run workflow**。大約 10–15 分鐘後，Releases 會出現新版。

whisper.cpp 使用 MIT 授權。
