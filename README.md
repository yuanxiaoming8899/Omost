<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">奥莫斯特</font></font></h1><a id="user-content-omost" class="anchor" aria-label="固定链接：Omost" href="#omost"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Omost 是一个将 LLM 的编码能力转化为图像生成（或者更准确地说，图像合成）能力的项目。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这个名字</font></font><code>Omost</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（发音：几乎）有两层含义：1）每次使用 Omost 后，您的图像几乎就完成了；2）</font></font><code>O</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">意思是“omni”（多模式），</font></font><code>most</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">意味着我们想最大限度地利用它。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Omost 提供 LLM 模型，该模型将编写代码以使用 Omost 的虚拟</font></font><code>Canvas</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代理来组合图像视觉内容。这</font></font><code>Canvas</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可以通过图像生成器的特定实现来渲染以实际生成图像。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">目前，我们基于 Llama3 和 Phi3 的变体提供 3 种预训练的 LLM 模型（另请参阅本页末尾的模型说明）。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有模型都使用以下混合数据进行训练：(1) 包括 Open-Images 在内的多个数据集的真实注释，(2) 通过自动注释图像提取的数据，(3) 来自 DPO（直接偏好优化，“代码是否可以由 python 3.10 编译”作为直接偏好）的强化，以及 (4) 来自 OpenAI GPT4o 多模态功能的少量调整数据。</font></font></p>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">立即开始</font></font></h1><a id="user-content-get-started" class="anchor" aria-label="永久链接：开始" href="#get-started"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以直接使用</font></font><a href="https://huggingface.co/spaces/lllyasviel/Omost" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">官方的HuggingFace空间</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或者，您可以使用以下部署（需要 8GB Nvidia VRAM）：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>git clone https://github.com/lllyasviel/Omost.git
cd Omost
conda create -n omost python=3.10
conda activate omost
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu121
pip install -r requirements.txt
python gradio_app.py
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="git clone https://github.com/lllyasviel/Omost.git
cd Omost
conda create -n omost python=3.10
conda activate omost
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu121
pip install -r requirements.txt
python gradio_app.py" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（请注意，量化 LLM 要求</font></font><code>bitsandbytes</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">- 某些 9XX 或 10XX 或 20XX GPU 可能无法正常运行。如果发生这种情况，请使用我们的官方 huggingface 空间。）</font></font></p>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">截图</font></font></h1><a id="user-content-screenshots" class="anchor" aria-label="永久链接：截图" href="#screenshots"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（全部采用随机种子 12345）</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">十九世纪一位衣衫褴褛、穿着破烂夹克的男子：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335529329-6acc5eac-87e4-428b-a209-1d4b947c590c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MjkzMjktNmFjYzVlYWMtODdlNC00MjhiLWEyMDktMWQ0Yjk0N2M1OTBjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWZmODZiNGE1YjIwYTI2MGUyM2UzZDdhYjAwNTY0NWQ1ZDdiYTAxMmY1MzZiNDBlMDEyN2NhNDNkODU4OTJjYTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.A0E72_ZoIHQsx2o3gV0-UAO3H3vJf4LAiJ2GKCcuaco"><img src="https://private-user-images.githubusercontent.com/19834515/335529329-6acc5eac-87e4-428b-a209-1d4b947c590c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MjkzMjktNmFjYzVlYWMtODdlNC00MjhiLWEyMDktMWQ0Yjk0N2M1OTBjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWZmODZiNGE1YjIwYTI2MGUyM2UzZDdhYjAwNTY0NWQ1ZDdiYTAxMmY1MzZiNDBlMDEyN2NhNDNkODU4OTJjYTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.A0E72_ZoIHQsx2o3gV0-UAO3H3vJf4LAiJ2GKCcuaco" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335529442-c60dadfc-6e82-4582-9561-8389260714c0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1Mjk0NDItYzYwZGFkZmMtNmU4Mi00NTgyLTk1NjEtODM4OTI2MDcxNGMwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWI0MjkyMmE5YjQzOWIzNzYzNDM0MjNjNDUxMTEyZDJhM2M5Y2M3ZTY0NDc0N2EzMWZlZjczMjhjMDUwMWZlYmYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0._FL0I2GcQvB3HdcpxiDbcH2ck3JnNV2Z6IrrBCHU0PU"><img src="https://private-user-images.githubusercontent.com/19834515/335529442-c60dadfc-6e82-4582-9561-8389260714c0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1Mjk0NDItYzYwZGFkZmMtNmU4Mi00NTgyLTk1NjEtODM4OTI2MDcxNGMwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWI0MjkyMmE5YjQzOWIzNzYzNDM0MjNjNDUxMTEyZDJhM2M5Y2M3ZTY0NDc0N2EzMWZlZjczMjhjMDUwMWZlYmYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0._FL0I2GcQvB3HdcpxiDbcH2ck3JnNV2Z6IrrBCHU0PU" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">末世后最伟大的逃亡，全人类的希望：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335531259-997d41ab-ea52-4036-898b-47c8b863acf4.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzEyNTktOTk3ZDQxYWItZWE1Mi00MDM2LTg5OGItNDdjOGI4NjNhY2Y0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ0NTNjOGQ0NjQ1NDYyZWY4ODQ0NGVjMDE2MWMyMjMxYWFmMTYyNjZlYTNmNTczMmJjM2ExOWNiYjNkZTU4YzAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Wxpg7x6xRUc1hmltCBltQ8GSXCYK5c-4tehv0RHjH1k"><img src="https://private-user-images.githubusercontent.com/19834515/335531259-997d41ab-ea52-4036-898b-47c8b863acf4.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzEyNTktOTk3ZDQxYWItZWE1Mi00MDM2LTg5OGItNDdjOGI4NjNhY2Y0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ0NTNjOGQ0NjQ1NDYyZWY4ODQ0NGVjMDE2MWMyMjMxYWFmMTYyNjZlYTNmNTczMmJjM2ExOWNiYjNkZTU4YzAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Wxpg7x6xRUc1hmltCBltQ8GSXCYK5c-4tehv0RHjH1k" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335531329-c6653558-bfd8-40d9-95fb-c5ec1b68c289.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzEzMjktYzY2NTM1NTgtYmZkOC00MGQ5LTk1ZmItYzVlYzFiNjhjMjg5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ1YjUwYjg2MGJhMmFjZTRmMGRhMzc1MDMwZDRhMDkzNDIzZDIzODIyOGJlZTM5MTg1NDc3NTBhNjlkMTBlZGUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.6qHuemq22lRgVNE5YaehuuVWhKFhm8bXcIu1peZyfVE"><img src="https://private-user-images.githubusercontent.com/19834515/335531329-c6653558-bfd8-40d9-95fb-c5ec1b68c289.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzEzMjktYzY2NTM1NTgtYmZkOC00MGQ5LTk1ZmItYzVlYzFiNjhjMjg5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ1YjUwYjg2MGJhMmFjZTRmMGRhMzc1MDMwZDRhMDkzNDIzZDIzODIyOGJlZTM5MTg1NDc3NTBhNjlkMTBlZGUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.6qHuemq22lRgVNE5YaehuuVWhKFhm8bXcIu1peZyfVE" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">侏罗纪恐龙大战：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335531999-7efe0b56-9da2-4967-bbb0-ed3cf4eddd23.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzE5OTktN2VmZTBiNTYtOWRhMi00OTY3LWJiYjAtZWQzY2Y0ZWRkZDIzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWY2YzE3OWI4Yjg0YTUxZmRmNjA5OGZkYjliZGYwYzBhMzRiZjZmN2U2MWI3ZjhhNWY0Mzk2YTQ5M2E2ZDhlYjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.JKNZuEmisuAsA-zXTcdiH4gCWh6iYyFBQBRUjc2VRl0"><img src="https://private-user-images.githubusercontent.com/19834515/335531999-7efe0b56-9da2-4967-bbb0-ed3cf4eddd23.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzE5OTktN2VmZTBiNTYtOWRhMi00OTY3LWJiYjAtZWQzY2Y0ZWRkZDIzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWY2YzE3OWI4Yjg0YTUxZmRmNjA5OGZkYjliZGYwYzBhMzRiZjZmN2U2MWI3ZjhhNWY0Mzk2YTQ5M2E2ZDhlYjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.JKNZuEmisuAsA-zXTcdiH4gCWh6iYyFBQBRUjc2VRl0" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335532058-f4b39798-488d-429c-bf96-27a7da6f91f7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzIwNTgtZjRiMzk3OTgtNDg4ZC00MjljLWJmOTYtMjdhN2RhNmY5MWY3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWM3ZmIzMDNhYWRjMGViYTQ0ZjE3YmYzODg4NmRkMDAzZDM3MTQ1OGRjMmU2YTI3ZDUxMzYxNDJjZWUwOWFjOTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.lj1sPWrbx4WVAzQ3rTGepsdZuiAn1HNb2HmP-eWB5Cw"><img src="https://private-user-images.githubusercontent.com/19834515/335532058-f4b39798-488d-429c-bf96-27a7da6f91f7.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1MzIwNTgtZjRiMzk3OTgtNDg4ZC00MjljLWJmOTYtMjdhN2RhNmY5MWY3LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWM3ZmIzMDNhYWRjMGViYTQ0ZjE3YmYzODg4NmRkMDAzZDM3MTQ1OGRjMmU2YTI3ZDUxMzYxNDJjZWUwOWFjOTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.lj1sPWrbx4WVAzQ3rTGepsdZuiAn1HNb2HmP-eWB5Cw" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">拥有无尽魔法的最高统治者坐在哥特式王座上，不死大军跪下：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335538528-336b7f94-0f8e-425a-b541-6e8cd5642a2e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1Mzg1MjgtMzM2YjdmOTQtMGY4ZS00MjVhLWI1NDEtNmU4Y2Q1NjQyYTJlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTMyOWNjYzZiODhiYTE0ZDYwYzJjNzVlNTg5NmRkOTdjMDA2M2Q1NzI1N2ZmYTkxYzY2NTA0ZTYyMmRiMjc4NTYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.P0Ig2GzrJBXX8VjGQXhP88w84Yq-eF6BchWkISbD5mg"><img src="https://private-user-images.githubusercontent.com/19834515/335538528-336b7f94-0f8e-425a-b541-6e8cd5642a2e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1Mzg1MjgtMzM2YjdmOTQtMGY4ZS00MjVhLWI1NDEtNmU4Y2Q1NjQyYTJlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTMyOWNjYzZiODhiYTE0ZDYwYzJjNzVlNTg5NmRkOTdjMDA2M2Q1NzI1N2ZmYTkxYzY2NTA0ZTYyMmRiMjc4NTYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.P0Ig2GzrJBXX8VjGQXhP88w84Yq-eF6BchWkISbD5mg" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335538577-9de68d20-0c01-4cee-b656-04d59cbdc695.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1Mzg1NzctOWRlNjhkMjAtMGMwMS00Y2VlLWI2NTYtMDRkNTljYmRjNjk1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBlNWIzZmRhODdkNzJkNTk5YzJlZWI2M2JmYTNiMWQ3MWIyNDIxYzdlODk2ZDlmZGU0M2ViZGE5MzMxNTVjZjUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.9D6zl9jF7FV0A62M7Ku4D58NjAKszjTCXJ8B3FazrrY"><img src="https://private-user-images.githubusercontent.com/19834515/335538577-9de68d20-0c01-4cee-b656-04d59cbdc695.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1Mzg1NzctOWRlNjhkMjAtMGMwMS00Y2VlLWI2NTYtMDRkNTljYmRjNjk1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBlNWIzZmRhODdkNzJkNTk5YzJlZWI2M2JmYTNiMWQ3MWIyNDIxYzdlODk2ZDlmZGU0M2ViZGE5MzMxNTVjZjUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.9D6zl9jF7FV0A62M7Ku4D58NjAKszjTCXJ8B3FazrrY" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">一部有趣的动画片，蝙蝠侠与小丑战斗：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335550862-dc751ded-f0f7-4312-8cd2-2a3aced15a60.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NTA4NjItZGM3NTFkZWQtZjBmNy00MzEyLThjZDItMmEzYWNlZDE1YTYwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTlmYjMxYjZjMTNjYjk1MzNkOGE3ZjNhNzVkY2MxNzRkNDNmMGMwODIzYTU2MGJjMWRmODQ1N2Y1ZTQ5NWM5MWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Sxl_f_LFYUlcSJv7Swma_4qDJ7w_LnvdJ1BfCi6oO9Y"><img src="https://private-user-images.githubusercontent.com/19834515/335550862-dc751ded-f0f7-4312-8cd2-2a3aced15a60.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NTA4NjItZGM3NTFkZWQtZjBmNy00MzEyLThjZDItMmEzYWNlZDE1YTYwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTlmYjMxYjZjMTNjYjk1MzNkOGE3ZjNhNzVkY2MxNzRkNDNmMGMwODIzYTU2MGJjMWRmODQ1N2Y1ZTQ5NWM5MWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Sxl_f_LFYUlcSJv7Swma_4qDJ7w_LnvdJ1BfCi6oO9Y" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335550901-f3e6e8e8-2e08-4e5e-a109-a8054461e71f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NTA5MDEtZjNlNmU4ZTgtMmUwOC00ZTVlLWExMDktYTgwNTQ0NjFlNzFmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTc5Yjg3ZDQ5YWI2MjA1ZWUzNDYwNWNjYzhhMGMyMDBlN2Y1OTQwYWE3Njk2MmI3MWY0ZThhNmU2N2E3NzUyNDkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.QuZnc3bc8vIVXRb6MWvXxHYNPooGQav1Ty8-LUubDnM"><img src="https://private-user-images.githubusercontent.com/19834515/335550901-f3e6e8e8-2e08-4e5e-a109-a8054461e71f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NTA5MDEtZjNlNmU4ZTgtMmUwOC00ZTVlLWExMDktYTgwNTQ0NjFlNzFmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTc5Yjg3ZDQ5YWI2MjA1ZWUzNDYwNWNjYzhhMGMyMDBlN2Y1OTQwYWE3Njk2MmI3MWY0ZThhNmU2N2E3NzUyNDkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.QuZnc3bc8vIVXRb6MWvXxHYNPooGQav1Ty8-LUubDnM" alt="图像" style="max-width: 100%;"></a></p>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例成绩单（带对话编辑）</font></font></h1><a id="user-content-example-transcripts-with-conversational-editing" class="anchor" aria-label="永久链接：示例成绩单（带对话编辑）" href="#example-transcripts-with-conversational-editing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（以下是默认模型的原始记录，随机种子为 123456）</font></font></em></p>
<p dir="auto"><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（如果 GitHub 的代码块渲染对阅读长行内容造成不便，请点击</font></font><a href="https://raw.githubusercontent.com/lllyasviel/Omost/main/README.md" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此处</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阅读原文。）</font></font></em></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">用户</font></font></h3><a id="user-content-user" class="anchor" aria-label="永久链接：用户" href="#user"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">生成战士与龙激烈战斗的图像</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">助手</font></font></h3><a id="user-content-assistant" class="anchor" aria-label="永久链接：助理" href="#assistant"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"># Initialize the canvas</span>
<span class="pl-s1">canvas</span> <span class="pl-c1">=</span> <span class="pl-v">Canvas</span>()

<span class="pl-c"># Set a global description for the canvas</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">set_global_description</span>(
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A fierce battle between warriors and a dragon.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'In this intense scene, a group of fierce warriors is engaged in an epic battle with a mighty dragon.'</span>,
        <span class="pl-s">'The warriors, clad in armor and wielding swords and shields, are positioned on the left side of the image.'</span>,
        <span class="pl-s">'Their expressions are determined and focused, reflecting their resolve to defeat the dragon.'</span>,
        <span class="pl-s">'The dragon, with its massive wings spread wide and its fiery breath illuminating the scene, dominates the center of the image.'</span>,
        <span class="pl-s">'Its scales glisten with a metallic sheen, and its eyes burn with a fierce intensity.'</span>,
        <span class="pl-s">'The background is a dark, stormy sky with flashes of lightning, adding to the drama and tension of the battle.'</span>,
        <span class="pl-s">'The ground is littered with debris and the remnants of previous battles, enhancing the sense of a long and brutal conflict.'</span>,
        <span class="pl-s">'The overall atmosphere is one of chaos and intensity, with the warriors and the dragon locked in a fierce struggle for survival.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'battle, warriors, dragon, fierce, armor, swords, shields, determined, focused, epic, intense, metallic, glistening, fiery breath, stormy sky, lightning, debris, conflict, struggle, survival, chaos, tension, drama, wings, scales, eyes, burning, illuminated'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'darkslategray'</span>,
)

<span class="pl-c"># Add a group of fierce warriors.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'on the left'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large horizontal area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">5.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A group of fierce warriors.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The warriors, clad in gleaming armor, are positioned on the left side of the image.'</span>,
        <span class="pl-s">'They are armed with swords, shields, and spears, ready for battle.'</span>,
        <span class="pl-s">'Their faces are set with determination and focus, reflecting their resolve to defeat the dragon.'</span>,
        <span class="pl-s">'Some warriors are in mid-action, swinging their swords or shields, while others stand ready to strike.'</span>,
        <span class="pl-s">'The armor they wear is intricately designed, with symbols and patterns that signify their rank and bravery.'</span>,
        <span class="pl-s">'The ground beneath them is uneven and littered with debris, adding to the sense of a chaotic and intense battle.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'warriors, armor, swords, shields, spears, determined, focused, mid-action, intricate design, symbols, patterns, rank, bravery, uneven ground, debris, chaotic, intense, battle'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Determined and focused, ready for the fierce battle.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Highly detailed and dynamic, capturing the intensity of the warriors.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with intricate details and dynamic poses.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'darkgoldenrod'</span>,
)

<span class="pl-c"># Add a mighty dragon.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'in the center'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large square area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">7.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A mighty dragon.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The dragon is a massive creature, dominating the center of the image with its wide-spread wings and fiery breath.'</span>,
        <span class="pl-s">'Its scales glisten with a metallic sheen, reflecting the light from its fiery breath.'</span>,
        <span class="pl-s">"The dragon's eyes burn with a fierce intensity, and its teeth are sharp and menacing."</span>,
        <span class="pl-s">'The wings of the dragon are powerful and spread wide, casting shadows over the battlefield.'</span>,
        <span class="pl-s">'The dragon’s body is muscular and covered in protective scales, with a long, sinewy tail that adds to its formidable appearance.'</span>,
        <span class="pl-s">'The fiery breath of the dragon illuminates the scene, casting a reddish glow over the warriors and the battlefield.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'dragon, massive, wings, fiery breath, glistening scales, metallic sheen, fierce eyes, sharp teeth, powerful wings, shadows, battlefield, muscular body, protective scales, sinewy tail, formidable, reddish glow, illumination'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Intense and menacing, with a powerful presence.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Epic and dramatic, emphasizing the grandeur and danger of the dragon.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with dramatic lighting and detailed textures.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'firebrick'</span>,
)

<span class="pl-c"># Add a stormy sky with flashes of lightning.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'on the top'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large horizontal area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">10.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A stormy sky with flashes of lightning.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The background of the image is a dark, stormy sky filled with swirling clouds and flashes of lightning.'</span>,
        <span class="pl-s">'The sky is turbulent, with clouds dark and foreboding, adding to the dramatic tension of the battle.'</span>,
        <span class="pl-s">'The lightning flashes illuminate the scene, casting sharp, brief lights over the warriors and the dragon.'</span>,
        <span class="pl-s">'The stormy sky creates a sense of chaos and unpredictability, heightening the intensity of the battle below.'</span>,
        <span class="pl-s">'The overall atmosphere is one of impending doom and relentless conflict, with the storm mirroring the fierce struggle between the warriors and the dragon.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'stormy sky, dark clouds, lightning, turbulent, foreboding, dramatic tension, illumination, chaos, unpredictability, intensity, impending doom, relentless conflict, battle, warriors, dragon, swirling clouds, sharp lights, brief lights'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Chaotic and intense, mirroring the fierce battle below.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Dramatic and turbulent, emphasizing the conflict and tension.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with dynamic lighting and detailed cloud textures.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'midnightblue'</span>,
)

<span class="pl-c"># Add a debris-covered battlefield.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'on the bottom'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large horizontal area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">5.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A debris-covered battlefield.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The ground of the battlefield is littered with debris, remnants of previous battles.'</span>,
        <span class="pl-s">'Broken weapons, shattered shields, and scattered armor pieces are strewn across the battlefield.'</span>,
        <span class="pl-s">'The terrain is uneven, with patches of mud and dirt, adding to the sense of a long and brutal conflict.'</span>,
        <span class="pl-s">'The debris-covered battlefield enhances the chaotic and intense atmosphere of the scene, reflecting the ferocity and duration of the battle.'</span>,
        <span class="pl-s">'The overall appearance is one of destruction and turmoil, with the remnants of previous battles serving as a grim reminder of the ongoing struggle.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'battlefield, debris, broken weapons, shattered shields, scattered armor, uneven terrain, mud, dirt, brutal conflict, chaos, intensity, destruction, turmoil, previous battles, ongoing struggle, remnants, ferocity, duration'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Chaotic and intense, reflecting the ferocity of the battle.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Detailed and realistic, emphasizing the destruction and chaos.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with detailed textures and realistic debris.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'darkolivegreen'</span>,
)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# Initialize the canvas
canvas = Canvas()

# Set a global description for the canvas
canvas.set_global_description(
    description='A fierce battle between warriors and a dragon.',
    detailed_descriptions=[
        'In this intense scene, a group of fierce warriors is engaged in an epic battle with a mighty dragon.',
        'The warriors, clad in armor and wielding swords and shields, are positioned on the left side of the image.',
        'Their expressions are determined and focused, reflecting their resolve to defeat the dragon.',
        'The dragon, with its massive wings spread wide and its fiery breath illuminating the scene, dominates the center of the image.',
        'Its scales glisten with a metallic sheen, and its eyes burn with a fierce intensity.',
        'The background is a dark, stormy sky with flashes of lightning, adding to the drama and tension of the battle.',
        'The ground is littered with debris and the remnants of previous battles, enhancing the sense of a long and brutal conflict.',
        'The overall atmosphere is one of chaos and intensity, with the warriors and the dragon locked in a fierce struggle for survival.',
    ],
    tags='battle, warriors, dragon, fierce, armor, swords, shields, determined, focused, epic, intense, metallic, glistening, fiery breath, stormy sky, lightning, debris, conflict, struggle, survival, chaos, tension, drama, wings, scales, eyes, burning, illuminated',
    HTML_web_color_name='darkslategray',
)

# Add a group of fierce warriors.
canvas.add_local_description(
    location='on the left',
    offset='no offset',
    area='a large horizontal area',
    distance_to_viewer=5.0,
    description='A group of fierce warriors.',
    detailed_descriptions=[
        'The warriors, clad in gleaming armor, are positioned on the left side of the image.',
        'They are armed with swords, shields, and spears, ready for battle.',
        'Their faces are set with determination and focus, reflecting their resolve to defeat the dragon.',
        'Some warriors are in mid-action, swinging their swords or shields, while others stand ready to strike.',
        'The armor they wear is intricately designed, with symbols and patterns that signify their rank and bravery.',
        'The ground beneath them is uneven and littered with debris, adding to the sense of a chaotic and intense battle.',
    ],
    tags='warriors, armor, swords, shields, spears, determined, focused, mid-action, intricate design, symbols, patterns, rank, bravery, uneven ground, debris, chaotic, intense, battle',
    atmosphere='Determined and focused, ready for the fierce battle.',
    style='Highly detailed and dynamic, capturing the intensity of the warriors.',
    quality_meta='High resolution with intricate details and dynamic poses.',
    HTML_web_color_name='darkgoldenrod',
)

# Add a mighty dragon.
canvas.add_local_description(
    location='in the center',
    offset='no offset',
    area='a large square area',
    distance_to_viewer=7.0,
    description='A mighty dragon.',
    detailed_descriptions=[
        'The dragon is a massive creature, dominating the center of the image with its wide-spread wings and fiery breath.',
        'Its scales glisten with a metallic sheen, reflecting the light from its fiery breath.',
        &quot;The dragon's eyes burn with a fierce intensity, and its teeth are sharp and menacing.&quot;,
        'The wings of the dragon are powerful and spread wide, casting shadows over the battlefield.',
        'The dragon’s body is muscular and covered in protective scales, with a long, sinewy tail that adds to its formidable appearance.',
        'The fiery breath of the dragon illuminates the scene, casting a reddish glow over the warriors and the battlefield.',
    ],
    tags='dragon, massive, wings, fiery breath, glistening scales, metallic sheen, fierce eyes, sharp teeth, powerful wings, shadows, battlefield, muscular body, protective scales, sinewy tail, formidable, reddish glow, illumination',
    atmosphere='Intense and menacing, with a powerful presence.',
    style='Epic and dramatic, emphasizing the grandeur and danger of the dragon.',
    quality_meta='High resolution with dramatic lighting and detailed textures.',
    HTML_web_color_name='firebrick',
)

# Add a stormy sky with flashes of lightning.
canvas.add_local_description(
    location='on the top',
    offset='no offset',
    area='a large horizontal area',
    distance_to_viewer=10.0,
    description='A stormy sky with flashes of lightning.',
    detailed_descriptions=[
        'The background of the image is a dark, stormy sky filled with swirling clouds and flashes of lightning.',
        'The sky is turbulent, with clouds dark and foreboding, adding to the dramatic tension of the battle.',
        'The lightning flashes illuminate the scene, casting sharp, brief lights over the warriors and the dragon.',
        'The stormy sky creates a sense of chaos and unpredictability, heightening the intensity of the battle below.',
        'The overall atmosphere is one of impending doom and relentless conflict, with the storm mirroring the fierce struggle between the warriors and the dragon.',
    ],
    tags='stormy sky, dark clouds, lightning, turbulent, foreboding, dramatic tension, illumination, chaos, unpredictability, intensity, impending doom, relentless conflict, battle, warriors, dragon, swirling clouds, sharp lights, brief lights',
    atmosphere='Chaotic and intense, mirroring the fierce battle below.',
    style='Dramatic and turbulent, emphasizing the conflict and tension.',
    quality_meta='High resolution with dynamic lighting and detailed cloud textures.',
    HTML_web_color_name='midnightblue',
)

# Add a debris-covered battlefield.
canvas.add_local_description(
    location='on the bottom',
    offset='no offset',
    area='a large horizontal area',
    distance_to_viewer=5.0,
    description='A debris-covered battlefield.',
    detailed_descriptions=[
        'The ground of the battlefield is littered with debris, remnants of previous battles.',
        'Broken weapons, shattered shields, and scattered armor pieces are strewn across the battlefield.',
        'The terrain is uneven, with patches of mud and dirt, adding to the sense of a long and brutal conflict.',
        'The debris-covered battlefield enhances the chaotic and intense atmosphere of the scene, reflecting the ferocity and duration of the battle.',
        'The overall appearance is one of destruction and turmoil, with the remnants of previous battles serving as a grim reminder of the ongoing struggle.',
    ],
    tags='battlefield, debris, broken weapons, shattered shields, scattered armor, uneven terrain, mud, dirt, brutal conflict, chaos, intensity, destruction, turmoil, previous battles, ongoing struggle, remnants, ferocity, duration',
    atmosphere='Chaotic and intense, reflecting the ferocity of the battle.',
    style='Detailed and realistic, emphasizing the destruction and chaos.',
    quality_meta='High resolution with detailed textures and realistic debris.',
    HTML_web_color_name='darkolivegreen',
)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">用户</font></font></h3><a id="user-content-user-1" class="anchor" aria-label="永久链接：用户" href="#user-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">把龙变成恐龙</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">助手</font></font></h3><a id="user-content-assistant-1" class="anchor" aria-label="永久链接：助理" href="#assistant-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"># Initialize the canvas</span>
<span class="pl-s1">canvas</span> <span class="pl-c1">=</span> <span class="pl-v">Canvas</span>()

<span class="pl-c"># Set a global description for the canvas</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">set_global_description</span>(
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A fierce battle between warriors and a dinosaur.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'In this intense scene, a group of fierce warriors is engaged in an epic battle with a mighty dinosaur.'</span>,
        <span class="pl-s">'The warriors, clad in armor and wielding swords and shields, are positioned on the left side of the image.'</span>,
        <span class="pl-s">'Their expressions are determined and focused, reflecting their resolve to defeat the dinosaur.'</span>,
        <span class="pl-s">'The dinosaur, with its massive body and powerful legs, dominates the center of the image.'</span>,
        <span class="pl-s">'Its scales glisten with a metallic sheen, and its eyes burn with a fierce intensity.'</span>,
        <span class="pl-s">'The background is a dark, stormy sky with flashes of lightning, adding to the drama and tension of the battle.'</span>,
        <span class="pl-s">'The ground is littered with debris and the remnants of previous battles, enhancing the sense of a long and brutal conflict.'</span>,
        <span class="pl-s">'The overall atmosphere is one of chaos and intensity, with the warriors and the dinosaur locked in a fierce struggle for survival.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'battle, warriors, dinosaur, fierce, armor, swords, shields, determined, focused, epic, intense, metallic, glistening, stormy sky, lightning, debris, conflict, struggle, survival, chaos, tension, drama, powerful legs, scales, eyes, burning, illuminated'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'darkslategray'</span>,
)

<span class="pl-c"># Add a group of fierce warriors.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'on the left'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large horizontal area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">5.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A group of fierce warriors.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The warriors, clad in gleaming armor, are positioned on the left side of the image.'</span>,
        <span class="pl-s">'They are armed with swords, shields, and spears, ready for battle.'</span>,
        <span class="pl-s">'Their faces are set with determination and focus, reflecting their resolve to defeat the dinosaur.'</span>,
        <span class="pl-s">'Some warriors are in mid-action, swinging their swords or shields, while others stand ready to strike.'</span>,
        <span class="pl-s">'The armor they wear is intricately designed, with symbols and patterns that signify their rank and bravery.'</span>,
        <span class="pl-s">'The ground beneath them is uneven and littered with debris, adding to the sense of a chaotic and intense battle.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'warriors, armor, swords, shields, spears, determined, focused, mid-action, intricate design, symbols, patterns, rank, bravery, uneven ground, debris, chaotic, intense, battle'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Determined and focused, ready for the fierce battle.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Highly detailed and dynamic, capturing the intensity of the warriors.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with intricate details and dynamic poses.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'darkgoldenrod'</span>,
)

<span class="pl-c"># Add a mighty dinosaur.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'in the center'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large square area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">7.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A mighty dinosaur.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The dinosaur is a massive creature, dominating the center of the image with its powerful legs and fierce roar.'</span>,
        <span class="pl-s">'Its scales glisten with a metallic sheen, reflecting the light from the stormy sky.'</span>,
        <span class="pl-s">"The dinosaur's eyes burn with a fierce intensity, and its teeth are sharp and menacing."</span>,
        <span class="pl-s">'The powerful legs of the dinosaur are muscular and add to its formidable appearance.'</span>,
        <span class="pl-s">'The ground shakes beneath its feet, enhancing the sense of a long and brutal conflict.'</span>,
        <span class="pl-s">'The overall appearance is one of destruction and turmoil, with the dinosaur adding to the chaotic atmosphere.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'dinosaur, massive, powerful legs, fierce roar, glistening scales, metallic sheen, fierce eyes, sharp teeth, muscular legs, formidable, ground shaking, destruction, turmoil, chaos, battle'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Intense and menacing, with a powerful presence.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Epic and dramatic, emphasizing the grandeur and danger of the dinosaur.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with dramatic lighting and detailed textures.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'firebrick'</span>,
)

<span class="pl-c"># Add a stormy sky with flashes of lightning.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'on the top'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large horizontal area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">10.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A stormy sky with flashes of lightning.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The background of the image is a dark, stormy sky filled with swirling clouds and flashes of lightning.'</span>,
        <span class="pl-s">'The sky is turbulent, with clouds dark and foreboding, adding to the dramatic tension of the battle.'</span>,
        <span class="pl-s">'The lightning flashes illuminate the scene, casting sharp, brief lights over the warriors and the dinosaur.'</span>,
        <span class="pl-s">'The stormy sky creates a sense of chaos and unpredictability, heightening the intensity of the battle below.'</span>,
        <span class="pl-s">'The overall atmosphere is one of impending doom and relentless conflict, with the storm mirroring the fierce struggle between the warriors and the dinosaur.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'stormy sky, dark clouds, lightning, turbulent, foreboding, dramatic tension, illumination, chaos, unpredictability, intensity, impending doom, relentless conflict, battle, warriors, dinosaur, swirling clouds, sharp lights, brief lights'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Chaotic and intense, mirroring the fierce battle below.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Dramatic and turbulent, emphasizing the conflict and tension.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with dynamic lighting and detailed cloud textures.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'midnightblue'</span>,
)

<span class="pl-c"># Add a debris-covered battlefield.</span>
<span class="pl-s1">canvas</span>.<span class="pl-en">add_local_description</span>(
    <span class="pl-s1">location</span><span class="pl-c1">=</span><span class="pl-s">'on the bottom'</span>,
    <span class="pl-s1">offset</span><span class="pl-c1">=</span><span class="pl-s">'no offset'</span>,
    <span class="pl-s1">area</span><span class="pl-c1">=</span><span class="pl-s">'a large horizontal area'</span>,
    <span class="pl-s1">distance_to_viewer</span><span class="pl-c1">=</span><span class="pl-c1">5.0</span>,
    <span class="pl-s1">description</span><span class="pl-c1">=</span><span class="pl-s">'A debris-covered battlefield.'</span>,
    <span class="pl-s1">detailed_descriptions</span><span class="pl-c1">=</span>[
        <span class="pl-s">'The ground of the battlefield is littered with debris, remnants of previous battles.'</span>,
        <span class="pl-s">'Broken weapons, shattered shields, and scattered armor pieces are strewn across the battlefield.'</span>,
        <span class="pl-s">'The terrain is uneven, with patches of mud and dirt, adding to the sense of a long and brutal conflict.'</span>,
        <span class="pl-s">'The debris-covered battlefield enhances the chaotic and intense atmosphere of the scene, reflecting the ferocity and duration of the battle.'</span>,
        <span class="pl-s">'The overall appearance is one of destruction and turmoil, with the remnants of previous battles serving as a grim reminder of the ongoing struggle.'</span>,
    ],
    <span class="pl-s1">tags</span><span class="pl-c1">=</span><span class="pl-s">'battlefield, debris, broken weapons, shattered shields, scattered armor, uneven terrain, mud, dirt, brutal conflict, chaos, intensity, destruction, turmoil, previous battles, ongoing struggle, remnants, ferocity, duration'</span>,
    <span class="pl-s1">atmosphere</span><span class="pl-c1">=</span><span class="pl-s">'Chaotic and intense, reflecting the ferocity of the battle.'</span>,
    <span class="pl-s1">style</span><span class="pl-c1">=</span><span class="pl-s">'Detailed and realistic, emphasizing the destruction and chaos.'</span>,
    <span class="pl-s1">quality_meta</span><span class="pl-c1">=</span><span class="pl-s">'High resolution with detailed textures and realistic debris.'</span>,
    <span class="pl-v">HTML_web_color_name</span><span class="pl-c1">=</span><span class="pl-s">'darkolivegreen'</span>,
)</pre><div class="zeroclipboard-container">
  
18.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有奥莫斯特法学硕士均接受过以下符号的培训</font></font></p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">class</span> <span class="pl-v">Canvas</span>:
    <span class="pl-k">def</span> <span class="pl-en">set_global_description</span>(
            <span class="pl-s1">self</span>, 
            <span class="pl-s1">description</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">detailed_descriptions</span>: <span class="pl-s1">list</span>[<span class="pl-s1">str</span>], 
            <span class="pl-s1">tags</span>: <span class="pl-s1">str</span>, 
            <span class="pl-v">HTML_web_color_name</span>: <span class="pl-s1">str</span>
    ):
        <span class="pl-k">pass</span>

    <span class="pl-k">def</span> <span class="pl-en">add_local_description</span>(
            <span class="pl-s1">self</span>, 
            <span class="pl-s1">location</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">offset</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">area</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">distance_to_viewer</span>: <span class="pl-s1">float</span>, 
            <span class="pl-s1">description</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">detailed_descriptions</span>: <span class="pl-s1">list</span>[<span class="pl-s1">str</span>], 
            <span class="pl-s1">tags</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">atmosphere</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">style</span>: <span class="pl-s1">str</span>, 
            <span class="pl-s1">quality_meta</span>: <span class="pl-s1">str</span>, 
            <span class="pl-v">HTML_web_color_name</span>: <span class="pl-s1">str</span>
    ):
        <span class="pl-k">assert</span> <span class="pl-s1">location</span> <span class="pl-c1">in</span> [
            <span class="pl-s">"in the center"</span>, 
            <span class="pl-s">"on the left"</span>, 
            <span class="pl-s">"on the right"</span>, 
            <span class="pl-s">"on the top"</span>, 
            <span class="pl-s">"on the bottom"</span>, 
            <span class="pl-s">"on the top-left"</span>, 
            <span class="pl-s">"on the top-right"</span>, 
            <span class="pl-s">"on the bottom-left"</span>, 
            <span class="pl-s">"on the bottom-right"</span>
        ]
        <span class="pl-k">assert</span> <span class="pl-s1">offset</span> <span class="pl-c1">in</span> [
            <span class="pl-s">"no offset"</span>, 
            <span class="pl-s">"slightly to the left"</span>, 
            <span class="pl-s">"slightly to the right"</span>, 
            <span class="pl-s">"slightly to the upper"</span>, 
            <span class="pl-s">"slightly to the lower"</span>, 
            <span class="pl-s">"slightly to the upper-left"</span>, 
            <span class="pl-s">"slightly to the upper-right"</span>, 
            <span class="pl-s">"slightly to the lower-left"</span>, 
            <span class="pl-s">"slightly to the lower-right"</span>
        ]
        <span class="pl-k">assert</span> <span class="pl-s1">area</span> <span class="pl-c1">in</span> [
            <span class="pl-s">"a small square area"</span>, 
            <span class="pl-s">"a small vertical area"</span>, 
            <span class="pl-s">"a small horizontal area"</span>, 
            <span class="pl-s">"a medium-sized square area"</span>, 
            <span class="pl-s">"a medium-sized vertical area"</span>, 
            <span class="pl-s">"a medium-sized horizontal area"</span>, 
            <span class="pl-s">"a large square area"</span>, 
            <span class="pl-s">"a large vertical area"</span>, 
            <span class="pl-s">"a large horizontal area"</span>
        ]
        <span class="pl-k">assert</span> <span class="pl-s1">distance_to_viewer</span> <span class="pl-c1">&gt;</span> <span class="pl-c1">0</span>
        <span class="pl-k">pass</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="class Canvas:
    def set_global_description(
            self, 
            description: str, 
            detailed_descriptions: list[str], 
            tags: str, 
            HTML_web_color_name: str
    ):
        pass

    def add_local_description(
            self, 
            location: str, 
            offset: str, 
            area: str, 
            distance_to_viewer: float, 
            description: str, 
            detailed_descriptions: list[str], 
            tags: str, 
            atmosphere: str, 
            style: str, 
            quality_meta: str, 
            HTML_web_color_name: str
    ):
        assert location in [
            &quot;in the center&quot;, 
            &quot;on the left&quot;, 
            &quot;on the right&quot;, 
            &quot;on the top&quot;, 
            &quot;on the bottom&quot;, 
            &quot;on the top-left&quot;, 
            &quot;on the top-right&quot;, 
            &quot;on the bottom-left&quot;, 
            &quot;on the bottom-right&quot;
        ]
        assert offset in [
            &quot;no offset&quot;, 
            &quot;slightly to the left&quot;, 
            &quot;slightly to the right&quot;, 
            &quot;slightly to the upper&quot;, 
            &quot;slightly to the lower&quot;, 
            &quot;slightly to the upper-left&quot;, 
            &quot;slightly to the upper-right&quot;, 
            &quot;slightly to the lower-left&quot;, 
            &quot;slightly to the lower-right&quot;
        ]
        assert area in [
            &quot;a small square area&quot;, 
            &quot;a small vertical area&quot;, 
            &quot;a small horizontal area&quot;, 
            &quot;a medium-sized square area&quot;, 
            &quot;a medium-sized vertical area&quot;, 
            &quot;a medium-sized horizontal area&quot;, 
            &quot;a large square area&quot;, 
            &quot;a large vertical area&quot;, 
            &quot;a large horizontal area&quot;
        ]
        assert distance_to_viewer > 0
        pass" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在训练过程中，上述符号与图像生成相关的特定概念和用例相关联。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该设计是为了使这些代码易于 LLM 学习，同时也易于扩散模型处理。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">让我们分解一下每个部分：</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">函数：Canvas.set_global_description 和 Canvas.add_local_description</font></font></h2><a id="user-content-function-canvasset_global_description-and-canvasadd_local_description" class="anchor" aria-label="永久链接：功能：Canvas.set_global_description 和 Canvas.add_local_description" href="#function-canvasset_global_description-and-canvasadd_local_description"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">它们为图片设置描述。 它们的参数含义相同， 比</font></font><code>add_local_description</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">具有更多的字段</font></font><code>set_global_description</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注释</font></font><code>set_global_description</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">整个图像， 而</font></font><code>add_local_description</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注释图像的一部分。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">参数：description 和 Detailed_descriptions</font></font></h2><a id="user-content-parameter-description-and-detailed_descriptions" class="anchor" aria-label="永久链接：参数：description 和 Detailed_descriptions" href="#parameter-description-and-detailed_descriptions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们引入一个概念，叫“子提示”。如果一个提示少于 75 个 token，并且能够自给自足地描述某件事，不依赖于其他提示，我们就称其为“子提示”。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是</font></font><code>description</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">一个子提示，</font></font><code>detailed_descriptions</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是子提示的列表。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，每个子提示严格少于 75 个标记（通常少于 40 个标记），您可以安全地使用任何剪辑对它们进行编码，而不必担心截断位置会影响语义。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">子提示符的设计还允许基于贪婪合并的更令人满意的文本编码。例如，如果你有</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>sub-prompt A: 25 tokens
sub-prompt B: 35 tokens
sub-prompt C: 5 tokens
sub-prompt D: 60 tokens
sub-prompt E: 15 tokens
sub-prompt F: 25 tokens
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="sub-prompt A: 25 tokens
sub-prompt B: 35 tokens
sub-prompt C: 5 tokens
sub-prompt D: 60 tokens
sub-prompt E: 15 tokens
sub-prompt F: 25 tokens" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">由于每个子提示都保证能够独立描述某件事，我们可以使用贪婪方法将它们合并到类似</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>bag 1 {A, B, C} : 65 tokens
bag 2 {D} : 60 tokens
bag 1 {E, F} : 40 tokens
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="bag 1 {A, B, C} : 65 tokens
bag 2 {D} : 60 tokens
bag 1 {E, F} : 40 tokens" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">每个袋子少于 75 个标记，并且可以一次性通过任何剪辑进行编码（然后将它们连接起来）。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以这种方式对文本进行编码将确保文本编码器永远不会犯语义截断错误。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有人可能会问 - 如果所有子提示都少于 75 个具有独立语义的标记，为什么不直接对它们进行编码而不进行合并然后再连接呢？这主要是因为我们希望文本嵌入更加连贯。例如，假设子提示 A 是“一个男人”，而子提示 B 是“英俊，专业”，那么在编码之前合并它们将为您提供一个更加混合的文本嵌入概念，其中包含英俊专业男人的连贯特征。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有 Omost LLM 都经过训练，可以提供严格定义的子提示。您可以利用这些定义来设计无损文本编码方法。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">参数：位置、偏移、面积</font></font></h3><a id="user-content-parameter-location-offset-area" class="anchor" aria-label="永久链接：参数：位置、偏移、区域" href="#parameter-location-offset-area"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这三个参数定义了一个边界框。注意它们必须遵循</font></font></p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">assert</span> <span class="pl-s1">location</span> <span class="pl-c1">in</span> [
    <span class="pl-s">"in the center"</span>, 
    <span class="pl-s">"on the left"</span>, 
    <span class="pl-s">"on the right"</span>, 
    <span class="pl-s">"on the top"</span>, 
    <span class="pl-s">"on the bottom"</span>, 
    <span class="pl-s">"on the top-left"</span>, 
    <span class="pl-s">"on the top-right"</span>, 
    <span class="pl-s">"on the bottom-left"</span>, 
    <span class="pl-s">"on the bottom-right"</span>
]
<span class="pl-k">assert</span> <span class="pl-s1">offset</span> <span class="pl-c1">in</span> [
    <span class="pl-s">"no offset"</span>, 
    <span class="pl-s">"slightly to the left"</span>, 
    <span class="pl-s">"slightly to the right"</span>, 
    <span class="pl-s">"slightly to the upper"</span>, 
    <span class="pl-s">"slightly to the lower"</span>, 
    <span class="pl-s">"slightly to the upper-left"</span>, 
    <span class="pl-s">"slightly to the upper-right"</span>, 
    <span class="pl-s">"slightly to the lower-left"</span>, 
    <span class="pl-s">"slightly to the lower-right"</span>
]
<span class="pl-k">assert</span> <span class="pl-s1">area</span> <span class="pl-c1">in</span> [
    <span class="pl-s">"a small square area"</span>, 
    <span class="pl-s">"a small vertical area"</span>, 
    <span class="pl-s">"a small horizontal area"</span>, 
    <span class="pl-s">"a medium-sized square area"</span>, 
    <span class="pl-s">"a medium-sized vertical area"</span>, 
    <span class="pl-s">"a medium-sized horizontal area"</span>, 
    <span class="pl-s">"a large square area"</span>, 
    <span class="pl-s">"a large vertical area"</span>, 
    <span class="pl-s">"a large horizontal area"</span>
]</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="assert location in [
    &quot;in the center&quot;, 
    &quot;on the left&quot;, 
    &quot;on the right&quot;, 
    &quot;on the top&quot;, 
    &quot;on the bottom&quot;, 
    &quot;on the top-left&quot;, 
    &quot;on the top-right&quot;, 
    &quot;on the bottom-left&quot;, 
    &quot;on the bottom-right&quot;
]
assert offset in [
    &quot;no offset&quot;, 
    &quot;slightly to the left&quot;, 
    &quot;slightly to the right&quot;, 
    &quot;slightly to the upper&quot;, 
    &quot;slightly to the lower&quot;, 
    &quot;slightly to the upper-left&quot;, 
    &quot;slightly to the upper-right&quot;, 
    &quot;slightly to the lower-left&quot;, 
    &quot;slightly to the lower-right&quot;
]
assert area in [
    &quot;a small square area&quot;, 
    &quot;a small vertical area&quot;, 
    &quot;a small horizontal area&quot;, 
    &quot;a medium-sized square area&quot;, 
    &quot;a medium-sized vertical area&quot;, 
    &quot;a medium-sized horizontal area&quot;, 
    &quot;a large square area&quot;, 
    &quot;a large vertical area&quot;, 
    &quot;a large horizontal area&quot;
]" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">首先我们将画布分成3*3=9个位置：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335338392-5d39cf93-c229-4c83-ae82-3eeeae2fabea.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzMzgzOTItNWQzOWNmOTMtYzIyOS00YzgzLWFlODItM2VlZWFlMmZhYmVhLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWM4ZDgxZDYyNjA1MWEwNTkyNzk3Yzg2MjZjMjhjYTQyZWRlYmVhMTQ2MjBlYmFmMjgxNDQyZDZjZjhhOTk0MTQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.sO_we85IeL3ZBUwC1zdawoSmqvgEnQXv2p1HSRZwJ5Q"><img src="https://private-user-images.githubusercontent.com/19834515/335338392-5d39cf93-c229-4c83-ae82-3eeeae2fabea.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzMzgzOTItNWQzOWNmOTMtYzIyOS00YzgzLWFlODItM2VlZWFlMmZhYmVhLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWM4ZDgxZDYyNjA1MWEwNTkyNzk3Yzg2MjZjMjhjYTQyZWRlYmVhMTQ2MjBlYmFmMjgxNDQyZDZjZjhhOTk0MTQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.sO_we85IeL3ZBUwC1zdawoSmqvgEnQXv2p1HSRZwJ5Q" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后我们进一步将每个位置划分为 3*3 偏移量，从而得到 9*9=81 个位置：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335341893-b744d787-11f3-4aeb-9d3a-aeba7a41b433.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzNDE4OTMtYjc0NGQ3ODctMTFmMy00YWViLTlkM2EtYWViYTdhNDFiNDMzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWYwY2Q5YjNmMDg2M2E5OTZmNTlkNzQ0ZTFlNmRhMzlhM2U1MGM3NDkzZjZhN2NjNzdkY2Y0NTljMmI2MTgwNWEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.QZRl0jzF7NpQu1yanJcETwUSHzRo7NulUETukBqTkJ4"><img src="https://private-user-images.githubusercontent.com/19834515/335341893-b744d787-11f3-4aeb-9d3a-aeba7a41b433.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzNDE4OTMtYjc0NGQ3ODctMTFmMy00YWViLTlkM2EtYWViYTdhNDFiNDMzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWYwY2Q5YjNmMDg2M2E5OTZmNTlkNzQ0ZTFlNmRhMzlhM2U1MGM3NDkzZjZhN2NjNzdkY2Y0NTljMmI2MTgwNWEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.QZRl0jzF7NpQu1yanJcETwUSHzRo7NulUETukBqTkJ4" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以这些位置为中心，我们进一步定义 9 种类型的边界框：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335343565-0e484b73-680f-486b-8b61-4373c9eec9a0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzNDM1NjUtMGU0ODRiNzMtNjgwZi00ODZiLThiNjEtNDM3M2M5ZWVjOWEwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWE0ODQxMWQ5OWQ3OGIxYmU0OWViM2I1N2ZkMjVhN2Q0M2JmM2IyYzVjMmYzYWU5MTk2Y2Y5MWI5MTZhMjIzZTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.5fwM6nDNP_oJS0U76W4J8gsogSpED8cpF2YOHHyfaTo"><img src="https://private-user-images.githubusercontent.com/19834515/335343565-0e484b73-680f-486b-8b61-4373c9eec9a0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzNDM1NjUtMGU0ODRiNzMtNjgwZi00ODZiLThiNjEtNDM3M2M5ZWVjOWEwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWE0ODQxMWQ5OWQ3OGIxYmU0OWViM2I1N2ZkMjVhN2Q0M2JmM2IyYzVjMmYzYWU5MTk2Y2Y5MWI5MTZhMjIzZTkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.5fwM6nDNP_oJS0U76W4J8gsogSpED8cpF2YOHHyfaTo" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们可以看到，该方法允许9*9*9=729个不同的边界框，几乎覆盖了图像中物体的所有常见可能位置。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">有人可能会争论为什么这是必要的——为什么不让法学硕士学习像素索引或 x、y 坐标——这样应该更准确吗？以下是我的几点笔记：</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我尝试了几种表示形式，包括像素索引（如 {x=32, y=16, w=58, h=99}），或边距像素（如 {left=32, right=15, top=27, bottom=33}），或百分比像素索引（如 {x=0.124, y=0.65, w=0.335, h=0.251}），或百分比边距（如 {left=0.251, right=0.154, top=0.254, bottom=0.441}）。结果是，开源 LLM 真的不太擅长学习这些表示形式，即使对于 Llama3（也许 GPT4o 可以学习它）。有时它会起作用，有时它会给出完全随机的数字。请注意，我们的问题与 MLLM 非常不同。视觉 LLM 通常将图像嵌入作为输入，在这种情况下估计数字位置就像查找表问题，并且可以在某种程度上进行学习，但我们的情况是 LLM 需要从头开始生成每个构图，而不需要任何图像嵌入来查找。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">但是自然语言，如“在右边”、“稍微靠右上方”、“一小块垂直区域”等，效果很好。模型收敛速度非常快，学习也很稳定。它与 LLM 的预训练知识非常吻合。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我也尝试过添加一些特殊的 token 来表示空间位置，并训练嵌入层。但该模型很难训练和调试。此外，每次我们更改 LLM 时，基于 token 嵌入的方法都需要进行许多超参数调整 - 例如，当从 Llama3 更改为 Phi 时，如果我们使用 token 嵌入方法，我们需要再次设计训练参数。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从边界框提议的角度来看，9*9*9=729 这个数字并不是一个小数目。这也可以称为 ROI（感兴趣区域），一些旧的语义分割技术使用 (RPN) 区域提议网络来生成类似数量（&lt;1000）的区域。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">大多数区域引导扩散方法都是粗级方法（如多重扩散和注意耦合和忽略），它们不需要像素完美的区域。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这些都是我个人的结果 - 如果您正在进行一些类似的多模态 LLM 研究，使用像素索引是完全可以的，值得尝试，并且其他训练方法可能也可以实现强大的系统。</font></font></li>
</ol>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">参数：distance_to_viewer 和 HTML_web_color_name</font></font></h3><a id="user-content-parameter-distance_to_viewer-and-html_web_color_name" class="anchor" aria-label="永久链接：参数：distance_to_viewer 和 HTML_web_color_name" href="#parameter-distance_to_viewer-and-html_web_color_name"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可以将其</font></font><code>distance_to_viewer</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视为相对深度。请注意，该值的绝对数字根本不可靠（因为开源 LLM 并不擅长生成图像空间数字），并且它只应用于将元素排序为背景到前景层。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在使用扩散模型渲染所有局部元素之前，您可以始终</font></font><code>distance_to_viewer</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对其进行排序。全局描述始终可以被视为最远的背景层。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其中之一就是</font></font><code>HTML_web_color_name</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：</font></font></p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-s1">possible_HTML_web_color_names</span> <span class="pl-c1">=</span> {  <span class="pl-c"># r, g, b</span>
    <span class="pl-s">'aliceblue'</span>: (<span class="pl-c1">240</span>, <span class="pl-c1">248</span>, <span class="pl-c1">255</span>), <span class="pl-s">'antiquewhite'</span>: (<span class="pl-c1">250</span>, <span class="pl-c1">235</span>, <span class="pl-c1">215</span>), <span class="pl-s">'aqua'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">255</span>, <span class="pl-c1">255</span>),
    <span class="pl-s">'aquamarine'</span>: (<span class="pl-c1">127</span>, <span class="pl-c1">255</span>, <span class="pl-c1">212</span>), <span class="pl-s">'azure'</span>: (<span class="pl-c1">240</span>, <span class="pl-c1">255</span>, <span class="pl-c1">255</span>), <span class="pl-s">'beige'</span>: (<span class="pl-c1">245</span>, <span class="pl-c1">245</span>, <span class="pl-c1">220</span>),
    <span class="pl-s">'bisque'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">228</span>, <span class="pl-c1">196</span>), <span class="pl-s">'black'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">0</span>, <span class="pl-c1">0</span>), <span class="pl-s">'blanchedalmond'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">235</span>, <span class="pl-c1">205</span>), <span class="pl-s">'blue'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">0</span>, <span class="pl-c1">255</span>),
    <span class="pl-s">'blueviolet'</span>: (<span class="pl-c1">138</span>, <span class="pl-c1">43</span>, <span class="pl-c1">226</span>), <span class="pl-s">'brown'</span>: (<span class="pl-c1">165</span>, <span class="pl-c1">42</span>, <span class="pl-c1">42</span>), <span class="pl-s">'burlywood'</span>: (<span class="pl-c1">222</span>, <span class="pl-c1">184</span>, <span class="pl-c1">135</span>),
    <span class="pl-s">'cadetblue'</span>: (<span class="pl-c1">95</span>, <span class="pl-c1">158</span>, <span class="pl-c1">160</span>), <span class="pl-s">'chartreuse'</span>: (<span class="pl-c1">127</span>, <span class="pl-c1">255</span>, <span class="pl-c1">0</span>), <span class="pl-s">'chocolate'</span>: (<span class="pl-c1">210</span>, <span class="pl-c1">105</span>, <span class="pl-c1">30</span>),
    <span class="pl-s">'coral'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">127</span>, <span class="pl-c1">80</span>), <span class="pl-s">'cornflowerblue'</span>: (<span class="pl-c1">100</span>, <span class="pl-c1">149</span>, <span class="pl-c1">237</span>), <span class="pl-s">'cornsilk'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">248</span>, <span class="pl-c1">220</span>),
    <span class="pl-s">'crimson'</span>: (<span class="pl-c1">220</span>, <span class="pl-c1">20</span>, <span class="pl-c1">60</span>), <span class="pl-s">'cyan'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">255</span>, <span class="pl-c1">255</span>), <span class="pl-s">'darkblue'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">0</span>, <span class="pl-c1">139</span>), <span class="pl-s">'darkcyan'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">139</span>, <span class="pl-c1">139</span>),
    <span class="pl-s">'darkgoldenrod'</span>: (<span class="pl-c1">184</span>, <span class="pl-c1">134</span>, <span class="pl-c1">11</span>), <span class="pl-s">'darkgray'</span>: (<span class="pl-c1">169</span>, <span class="pl-c1">169</span>, <span class="pl-c1">169</span>), <span class="pl-s">'darkgrey'</span>: (<span class="pl-c1">169</span>, <span class="pl-c1">169</span>, <span class="pl-c1">169</span>),
    <span class="pl-s">'darkgreen'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">100</span>, <span class="pl-c1">0</span>), <span class="pl-s">'darkkhaki'</span>: (<span class="pl-c1">189</span>, <span class="pl-c1">183</span>, <span class="pl-c1">107</span>), <span class="pl-s">'darkmagenta'</span>: (<span class="pl-c1">139</span>, <span class="pl-c1">0</span>, <span class="pl-c1">139</span>),
    <span class="pl-s">'darkolivegreen'</span>: (<span class="pl-c1">85</span>, <span class="pl-c1">107</span>, <span class="pl-c1">47</span>), <span class="pl-s">'darkorange'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">140</span>, <span class="pl-c1">0</span>), <span class="pl-s">'darkorchid'</span>: (<span class="pl-c1">153</span>, <span class="pl-c1">50</span>, <span class="pl-c1">204</span>),
    <span class="pl-s">'darkred'</span>: (<span class="pl-c1">139</span>, <span class="pl-c1">0</span>, <span class="pl-c1">0</span>), <span class="pl-s">'darksalmon'</span>: (<span class="pl-c1">233</span>, <span class="pl-c1">150</span>, <span class="pl-c1">122</span>), <span class="pl-s">'darkseagreen'</span>: (<span class="pl-c1">143</span>, <span class="pl-c1">188</span>, <span class="pl-c1">143</span>),
    <span class="pl-s">'darkslateblue'</span>: (<span class="pl-c1">72</span>, <span class="pl-c1">61</span>, <span class="pl-c1">139</span>), <span class="pl-s">'darkslategray'</span>: (<span class="pl-c1">47</span>, <span class="pl-c1">79</span>, <span class="pl-c1">79</span>), <span class="pl-s">'darkslategrey'</span>: (<span class="pl-c1">47</span>, <span class="pl-c1">79</span>, <span class="pl-c1">79</span>),
    <span class="pl-s">'darkturquoise'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">206</span>, <span class="pl-c1">209</span>), <span class="pl-s">'darkviolet'</span>: (<span class="pl-c1">148</span>, <span class="pl-c1">0</span>, <span class="pl-c1">211</span>), <span class="pl-s">'deeppink'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">20</span>, <span class="pl-c1">147</span>),
    <span class="pl-s">'deepskyblue'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">191</span>, <span class="pl-c1">255</span>), <span class="pl-s">'dimgray'</span>: (<span class="pl-c1">105</span>, <span class="pl-c1">105</span>, <span class="pl-c1">105</span>), <span class="pl-s">'dimgrey'</span>: (<span class="pl-c1">105</span>, <span class="pl-c1">105</span>, <span class="pl-c1">105</span>),
    <span class="pl-s">'dodgerblue'</span>: (<span class="pl-c1">30</span>, <span class="pl-c1">144</span>, <span class="pl-c1">255</span>), <span class="pl-s">'firebrick'</span>: (<span class="pl-c1">178</span>, <span class="pl-c1">34</span>, <span class="pl-c1">34</span>), <span class="pl-s">'floralwhite'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">250</span>, <span class="pl-c1">240</span>),
    <span class="pl-s">'forestgreen'</span>: (<span class="pl-c1">34</span>, <span class="pl-c1">139</span>, <span class="pl-c1">34</span>), <span class="pl-s">'fuchsia'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">0</span>, <span class="pl-c1">255</span>), <span class="pl-s">'gainsboro'</span>: (<span class="pl-c1">220</span>, <span class="pl-c1">220</span>, <span class="pl-c1">220</span>),
    <span class="pl-s">'ghostwhite'</span>: (<span class="pl-c1">248</span>, <span class="pl-c1">248</span>, <span class="pl-c1">255</span>), <span class="pl-s">'gold'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">215</span>, <span class="pl-c1">0</span>), <span class="pl-s">'goldenrod'</span>: (<span class="pl-c1">218</span>, <span class="pl-c1">165</span>, <span class="pl-c1">32</span>),
    <span class="pl-s">'gray'</span>: (<span class="pl-c1">128</span>, <span class="pl-c1">128</span>, <span class="pl-c1">128</span>), <span class="pl-s">'grey'</span>: (<span class="pl-c1">128</span>, <span class="pl-c1">128</span>, <span class="pl-c1">128</span>), <span class="pl-s">'green'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">128</span>, <span class="pl-c1">0</span>), <span class="pl-s">'greenyellow'</span>: (<span class="pl-c1">173</span>, <span class="pl-c1">255</span>, <span class="pl-c1">47</span>),
    <span class="pl-s">'honeydew'</span>: (<span class="pl-c1">240</span>, <span class="pl-c1">255</span>, <span class="pl-c1">240</span>), <span class="pl-s">'hotpink'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">105</span>, <span class="pl-c1">180</span>), <span class="pl-s">'indianred'</span>: (<span class="pl-c1">205</span>, <span class="pl-c1">92</span>, <span class="pl-c1">92</span>),
    <span class="pl-s">'indigo'</span>: (<span class="pl-c1">75</span>, <span class="pl-c1">0</span>, <span class="pl-c1">130</span>), <span class="pl-s">'ivory'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">255</span>, <span class="pl-c1">240</span>), <span class="pl-s">'khaki'</span>: (<span class="pl-c1">240</span>, <span class="pl-c1">230</span>, <span class="pl-c1">140</span>), <span class="pl-s">'lavender'</span>: (<span class="pl-c1">230</span>, <span class="pl-c1">230</span>, <span class="pl-c1">250</span>),
    <span class="pl-s">'lavenderblush'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">240</span>, <span class="pl-c1">245</span>), <span class="pl-s">'lawngreen'</span>: (<span class="pl-c1">124</span>, <span class="pl-c1">252</span>, <span class="pl-c1">0</span>), <span class="pl-s">'lemonchiffon'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">250</span>, <span class="pl-c1">205</span>),
    <span class="pl-s">'lightblue'</span>: (<span class="pl-c1">173</span>, <span class="pl-c1">216</span>, <span class="pl-c1">230</span>), <span class="pl-s">'lightcoral'</span>: (<span class="pl-c1">240</span>, <span class="pl-c1">128</span>, <span class="pl-c1">128</span>), <span class="pl-s">'lightcyan'</span>: (<span class="pl-c1">224</span>, <span class="pl-c1">255</span>, <span class="pl-c1">255</span>),
    <span class="pl-s">'lightgoldenrodyellow'</span>: (<span class="pl-c1">250</span>, <span class="pl-c1">250</span>, <span class="pl-c1">210</span>), <span class="pl-s">'lightgray'</span>: (<span class="pl-c1">211</span>, <span class="pl-c1">211</span>, <span class="pl-c1">211</span>), <span class="pl-s">'lightgrey'</span>: (<span class="pl-c1">211</span>, <span class="pl-c1">211</span>, <span class="pl-c1">211</span>),
    <span class="pl-s">'lightgreen'</span>: (<span class="pl-c1">144</span>, <span class="pl-c1">238</span>, <span class="pl-c1">144</span>), <span class="pl-s">'lightpink'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">182</span>, <span class="pl-c1">193</span>), <span class="pl-s">'lightsalmon'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">160</span>, <span class="pl-c1">122</span>),
    <span class="pl-s">'lightseagreen'</span>: (<span class="pl-c1">32</span>, <span class="pl-c1">178</span>, <span class="pl-c1">170</span>), <span class="pl-s">'lightskyblue'</span>: (<span class="pl-c1">135</span>, <span class="pl-c1">206</span>, <span class="pl-c1">250</span>), <span class="pl-s">'lightslategray'</span>: (<span class="pl-c1">119</span>, <span class="pl-c1">136</span>, <span class="pl-c1">153</span>),
    <span class="pl-s">'lightslategrey'</span>: (<span class="pl-c1">119</span>, <span class="pl-c1">136</span>, <span class="pl-c1">153</span>), <span class="pl-s">'lightsteelblue'</span>: (<span class="pl-c1">176</span>, <span class="pl-c1">196</span>, <span class="pl-c1">222</span>), <span class="pl-s">'lightyellow'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">255</span>, <span class="pl-c1">224</span>),
    <span class="pl-s">'lime'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">255</span>, <span class="pl-c1">0</span>), <span class="pl-s">'limegreen'</span>: (<span class="pl-c1">50</span>, <span class="pl-c1">205</span>, <span class="pl-c1">50</span>), <span class="pl-s">'linen'</span>: (<span class="pl-c1">250</span>, <span class="pl-c1">240</span>, <span class="pl-c1">230</span>), <span class="pl-s">'magenta'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">0</span>, <span class="pl-c1">255</span>),
    <span class="pl-s">'maroon'</span>: (<span class="pl-c1">128</span>, <span class="pl-c1">0</span>, <span class="pl-c1">0</span>), <span class="pl-s">'mediumaquamarine'</span>: (<span class="pl-c1">102</span>, <span class="pl-c1">205</span>, <span class="pl-c1">170</span>), <span class="pl-s">'mediumblue'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">0</span>, <span class="pl-c1">205</span>),
    <span class="pl-s">'mediumorchid'</span>: (<span class="pl-c1">186</span>, <span class="pl-c1">85</span>, <span class="pl-c1">211</span>), <span class="pl-s">'mediumpurple'</span>: (<span class="pl-c1">147</span>, <span class="pl-c1">112</span>, <span class="pl-c1">219</span>), <span class="pl-s">'mediumseagreen'</span>: (<span class="pl-c1">60</span>, <span class="pl-c1">179</span>, <span class="pl-c1">113</span>),
    <span class="pl-s">'mediumslateblue'</span>: (<span class="pl-c1">123</span>, <span class="pl-c1">104</span>, <span class="pl-c1">238</span>), <span class="pl-s">'mediumspringgreen'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">250</span>, <span class="pl-c1">154</span>),
    <span class="pl-s">'mediumturquoise'</span>: (<span class="pl-c1">72</span>, <span class="pl-c1">209</span>, <span class="pl-c1">204</span>), <span class="pl-s">'mediumvioletred'</span>: (<span class="pl-c1">199</span>, <span class="pl-c1">21</span>, <span class="pl-c1">133</span>), <span class="pl-s">'midnightblue'</span>: (<span class="pl-c1">25</span>, <span class="pl-c1">25</span>, <span class="pl-c1">112</span>),
    <span class="pl-s">'mintcream'</span>: (<span class="pl-c1">245</span>, <span class="pl-c1">255</span>, <span class="pl-c1">250</span>), <span class="pl-s">'mistyrose'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">228</span>, <span class="pl-c1">225</span>), <span class="pl-s">'moccasin'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">228</span>, <span class="pl-c1">181</span>),
    <span class="pl-s">'navajowhite'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">222</span>, <span class="pl-c1">173</span>), <span class="pl-s">'navy'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">0</span>, <span class="pl-c1">128</span>), <span class="pl-s">'navyblue'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">0</span>, <span class="pl-c1">128</span>),
    <span class="pl-s">'oldlace'</span>: (<span class="pl-c1">253</span>, <span class="pl-c1">245</span>, <span class="pl-c1">230</span>), <span class="pl-s">'olive'</span>: (<span class="pl-c1">128</span>, <span class="pl-c1">128</span>, <span class="pl-c1">0</span>), <span class="pl-s">'olivedrab'</span>: (<span class="pl-c1">107</span>, <span class="pl-c1">142</span>, <span class="pl-c1">35</span>),
    <span class="pl-s">'orange'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">165</span>, <span class="pl-c1">0</span>), <span class="pl-s">'orangered'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">69</span>, <span class="pl-c1">0</span>), <span class="pl-s">'orchid'</span>: (<span class="pl-c1">218</span>, <span class="pl-c1">112</span>, <span class="pl-c1">214</span>),
    <span class="pl-s">'palegoldenrod'</span>: (<span class="pl-c1">238</span>, <span class="pl-c1">232</span>, <span class="pl-c1">170</span>), <span class="pl-s">'palegreen'</span>: (<span class="pl-c1">152</span>, <span class="pl-c1">251</span>, <span class="pl-c1">152</span>), <span class="pl-s">'paleturquoise'</span>: (<span class="pl-c1">175</span>, <span class="pl-c1">238</span>, <span class="pl-c1">238</span>),
    <span class="pl-s">'palevioletred'</span>: (<span class="pl-c1">219</span>, <span class="pl-c1">112</span>, <span class="pl-c1">147</span>), <span class="pl-s">'papayawhip'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">239</span>, <span class="pl-c1">213</span>), <span class="pl-s">'peachpuff'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">218</span>, <span class="pl-c1">185</span>),
    <span class="pl-s">'peru'</span>: (<span class="pl-c1">205</span>, <span class="pl-c1">133</span>, <span class="pl-c1">63</span>), <span class="pl-s">'pink'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">192</span>, <span class="pl-c1">203</span>), <span class="pl-s">'plum'</span>: (<span class="pl-c1">221</span>, <span class="pl-c1">160</span>, <span class="pl-c1">221</span>), <span class="pl-s">'powderblue'</span>: (<span class="pl-c1">176</span>, <span class="pl-c1">224</span>, <span class="pl-c1">230</span>),
    <span class="pl-s">'purple'</span>: (<span class="pl-c1">128</span>, <span class="pl-c1">0</span>, <span class="pl-c1">128</span>), <span class="pl-s">'rebeccapurple'</span>: (<span class="pl-c1">102</span>, <span class="pl-c1">51</span>, <span class="pl-c1">153</span>), <span class="pl-s">'red'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">0</span>, <span class="pl-c1">0</span>),
    <span class="pl-s">'rosybrown'</span>: (<span class="pl-c1">188</span>, <span class="pl-c1">143</span>, <span class="pl-c1">143</span>), <span class="pl-s">'royalblue'</span>: (<span class="pl-c1">65</span>, <span class="pl-c1">105</span>, <span class="pl-c1">225</span>), <span class="pl-s">'saddlebrown'</span>: (<span class="pl-c1">139</span>, <span class="pl-c1">69</span>, <span class="pl-c1">19</span>),
    <span class="pl-s">'salmon'</span>: (<span class="pl-c1">250</span>, <span class="pl-c1">128</span>, <span class="pl-c1">114</span>), <span class="pl-s">'sandybrown'</span>: (<span class="pl-c1">244</span>, <span class="pl-c1">164</span>, <span class="pl-c1">96</span>), <span class="pl-s">'seagreen'</span>: (<span class="pl-c1">46</span>, <span class="pl-c1">139</span>, <span class="pl-c1">87</span>),
    <span class="pl-s">'seashell'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">245</span>, <span class="pl-c1">238</span>), <span class="pl-s">'sienna'</span>: (<span class="pl-c1">160</span>, <span class="pl-c1">82</span>, <span class="pl-c1">45</span>), <span class="pl-s">'silver'</span>: (<span class="pl-c1">192</span>, <span class="pl-c1">192</span>, <span class="pl-c1">192</span>),
    <span class="pl-s">'skyblue'</span>: (<span class="pl-c1">135</span>, <span class="pl-c1">206</span>, <span class="pl-c1">235</span>), <span class="pl-s">'slateblue'</span>: (<span class="pl-c1">106</span>, <span class="pl-c1">90</span>, <span class="pl-c1">205</span>), <span class="pl-s">'slategray'</span>: (<span class="pl-c1">112</span>, <span class="pl-c1">128</span>, <span class="pl-c1">144</span>),
    <span class="pl-s">'slategrey'</span>: (<span class="pl-c1">112</span>, <span class="pl-c1">128</span>, <span class="pl-c1">144</span>), <span class="pl-s">'snow'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">250</span>, <span class="pl-c1">250</span>), <span class="pl-s">'springgreen'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">255</span>, <span class="pl-c1">127</span>),
    <span class="pl-s">'steelblue'</span>: (<span class="pl-c1">70</span>, <span class="pl-c1">130</span>, <span class="pl-c1">180</span>), <span class="pl-s">'tan'</span>: (<span class="pl-c1">210</span>, <span class="pl-c1">180</span>, <span class="pl-c1">140</span>), <span class="pl-s">'teal'</span>: (<span class="pl-c1">0</span>, <span class="pl-c1">128</span>, <span class="pl-c1">128</span>), <span class="pl-s">'thistle'</span>: (<span class="pl-c1">216</span>, <span class="pl-c1">191</span>, <span class="pl-c1">216</span>),
    <span class="pl-s">'tomato'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">99</span>, <span class="pl-c1">71</span>), <span class="pl-s">'turquoise'</span>: (<span class="pl-c1">64</span>, <span class="pl-c1">224</span>, <span class="pl-c1">208</span>), <span class="pl-s">'violet'</span>: (<span class="pl-c1">238</span>, <span class="pl-c1">130</span>, <span class="pl-c1">238</span>),
    <span class="pl-s">'wheat'</span>: (<span class="pl-c1">245</span>, <span class="pl-c1">222</span>, <span class="pl-c1">179</span>), <span class="pl-s">'white'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">255</span>, <span class="pl-c1">255</span>), <span class="pl-s">'whitesmoke'</span>: (<span class="pl-c1">245</span>, <span class="pl-c1">245</span>, <span class="pl-c1">245</span>),
    <span class="pl-s">'yellow'</span>: (<span class="pl-c1">255</span>, <span class="pl-c1">255</span>, <span class="pl-c1">0</span>), <span class="pl-s">'yellowgreen'</span>: (<span class="pl-c1">154</span>, <span class="pl-c1">205</span>, <span class="pl-c1">50</span>)
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="possible_HTML_web_color_names = {  # r, g, b
    'aliceblue': (240, 248, 255), 'antiquewhite': (250, 235, 215), 'aqua': (0, 255, 255),
    'aquamarine': (127, 255, 212), 'azure': (240, 255, 255), 'beige': (245, 245, 220),
    'bisque': (255, 228, 196), 'black': (0, 0, 0), 'blanchedalmond': (255, 235, 205), 'blue': (0, 0, 255),
    'blueviolet': (138, 43, 226), 'brown': (165, 42, 42), 'burlywood': (222, 184, 135),
    'cadetblue': (95, 158, 160), 'chartreuse': (127, 255, 0), 'chocolate': (210, 105, 30),
    'coral': (255, 127, 80), 'cornflowerblue': (100, 149, 237), 'cornsilk': (255, 248, 220),
    'crimson': (220, 20, 60), 'cyan': (0, 255, 255), 'darkblue': (0, 0, 139), 'darkcyan': (0, 139, 139),
    'darkgoldenrod': (184, 134, 11), 'darkgray': (169, 169, 169), 'darkgrey': (169, 169, 169),
    'darkgreen': (0, 100, 0), 'darkkhaki': (189, 183, 107), 'darkmagenta': (139, 0, 139),
    'darkolivegreen': (85, 107, 47), 'darkorange': (255, 140, 0), 'darkorchid': (153, 50, 204),
    'darkred': (139, 0, 0), 'darksalmon': (233, 150, 122), 'darkseagreen': (143, 188, 143),
    'darkslateblue': (72, 61, 139), 'darkslategray': (47, 79, 79), 'darkslategrey': (47, 79, 79),
    'darkturquoise': (0, 206, 209), 'darkviolet': (148, 0, 211), 'deeppink': (255, 20, 147),
    'deepskyblue': (0, 191, 255), 'dimgray': (105, 105, 105), 'dimgrey': (105, 105, 105),
    'dodgerblue': (30, 144, 255), 'firebrick': (178, 34, 34), 'floralwhite': (255, 250, 240),
    'forestgreen': (34, 139, 34), 'fuchsia': (255, 0, 255), 'gainsboro': (220, 220, 220),
    'ghostwhite': (248, 248, 255), 'gold': (255, 215, 0), 'goldenrod': (218, 165, 32),
    'gray': (128, 128, 128), 'grey': (128, 128, 128), 'green': (0, 128, 0), 'greenyellow': (173, 255, 47),
    'honeydew': (240, 255, 240), 'hotpink': (255, 105, 180), 'indianred': (205, 92, 92),
    'indigo': (75, 0, 130), 'ivory': (255, 255, 240), 'khaki': (240, 230, 140), 'lavender': (230, 230, 250),
    'lavenderblush': (255, 240, 245), 'lawngreen': (124, 252, 0), 'lemonchiffon': (255, 250, 205),
    'lightblue': (173, 216, 230), 'lightcoral': (240, 128, 128), 'lightcyan': (224, 255, 255),
    'lightgoldenrodyellow': (250, 250, 210), 'lightgray': (211, 211, 211), 'lightgrey': (211, 211, 211),
    'lightgreen': (144, 238, 144), 'lightpink': (255, 182, 193), 'lightsalmon': (255, 160, 122),
    'lightseagreen': (32, 178, 170), 'lightskyblue': (135, 206, 250), 'lightslategray': (119, 136, 153),
    'lightslategrey': (119, 136, 153), 'lightsteelblue': (176, 196, 222), 'lightyellow': (255, 255, 224),
    'lime': (0, 255, 0), 'limegreen': (50, 205, 50), 'linen': (250, 240, 230), 'magenta': (255, 0, 255),
    'maroon': (128, 0, 0), 'mediumaquamarine': (102, 205, 170), 'mediumblue': (0, 0, 205),
    'mediumorchid': (186, 85, 211), 'mediumpurple': (147, 112, 219), 'mediumseagreen': (60, 179, 113),
    'mediumslateblue': (123, 104, 238), 'mediumspringgreen': (0, 250, 154),
    'mediumturquoise': (72, 209, 204), 'mediumvioletred': (199, 21, 133), 'midnightblue': (25, 25, 112),
    'mintcream': (245, 255, 250), 'mistyrose': (255, 228, 225), 'moccasin': (255, 228, 181),
    'navajowhite': (255, 222, 173), 'navy': (0, 0, 128), 'navyblue': (0, 0, 128),
    'oldlace': (253, 245, 230), 'olive': (128, 128, 0), 'olivedrab': (107, 142, 35),
    'orange': (255, 165, 0), 'orangered': (255, 69, 0), 'orchid': (218, 112, 214),
    'palegoldenrod': (238, 232, 170), 'palegreen': (152, 251, 152), 'paleturquoise': (175, 238, 238),
    'palevioletred': (219, 112, 147), 'papayawhip': (255, 239, 213), 'peachpuff': (255, 218, 185),
    'peru': (205, 133, 63), 'pink': (255, 192, 203), 'plum': (221, 160, 221), 'powderblue': (176, 224, 230),
    'purple': (128, 0, 128), 'rebeccapurple': (102, 51, 153), 'red': (255, 0, 0),
    'rosybrown': (188, 143, 143), 'royalblue': (65, 105, 225), 'saddlebrown': (139, 69, 19),
    'salmon': (250, 128, 114), 'sandybrown': (244, 164, 96), 'seagreen': (46, 139, 87),
    'seashell': (255, 245, 238), 'sienna': (160, 82, 45), 'silver': (192, 192, 192),
    'skyblue': (135, 206, 235), 'slateblue': (106, 90, 205), 'slategray': (112, 128, 144),
    'slategrey': (112, 128, 144), 'snow': (255, 250, 250), 'springgreen': (0, 255, 127),
    'steelblue': (70, 130, 180), 'tan': (210, 180, 140), 'teal': (0, 128, 128), 'thistle': (216, 191, 216),
    'tomato': (255, 99, 71), 'turquoise': (64, 224, 208), 'violet': (238, 130, 238),
    'wheat': (245, 222, 179), 'white': (255, 255, 255), 'whitesmoke': (245, 245, 245),
    'yellow': (255, 255, 0), 'yellowgreen': (154, 205, 50)
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">通过组合</font></font><code>distance_to_viewer</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>HTML_web_color_name</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，您可以绘制非常粗略的合成图像。例如，如果 LLM 运行良好，“暗室中木桌上红色瓶子前面的绿色瓶子”应该可以让您计算出如下图像：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335352959-ab501872-bbcc-4fd4-8ab4-6fecd1a44d4d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzNTI5NTktYWI1MDE4NzItYmJjYy00ZmQ0LThhYjQtNmZlY2QxYTQ0ZDRkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTk0ZWI3YzZhZThiMzkzYTU1MDRkMTAwMjZjZTVjMzU3ZTQ0NWJkMDlkNWMyNDkyZDhkZTdjYzZjN2Y2NDk2MGYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.IQcK1EzzmU8XGmabsSiE_Er05ArtCRmoiAf6Cu5ghNY"><img src="https://private-user-images.githubusercontent.com/19834515/335352959-ab501872-bbcc-4fd4-8ab4-6fecd1a44d4d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzUzNTI5NTktYWI1MDE4NzItYmJjYy00ZmQ0LThhYjQtNmZlY2QxYTQ0ZDRkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTk0ZWI3YzZhZThiMzkzYTU1MDRkMTAwMjZjZTVjMzU3ZTQ0NWJkMDlkNWMyNDkyZDhkZTdjYzZjN2Y2NDk2MGYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.IQcK1EzzmU8XGmabsSiE_Er05ArtCRmoiAf6Cu5ghNY" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以使用此图像作为初始潜在图像，并使用 0.95 到 0.99 的去噪强度来生成图像。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或者如果您不喜欢这样并且仍然喜欢让扩散模型从零均值生成（即使您知道大多数扩散模型都有 tsnr 问题），您可以忽略此图像或仅使用此图像作为调试器。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此外，层排序在一些非常特殊的注意力公式中也很有用——我们稍后会讨论这个问题。</font></font></p>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">参数：标签和氛围和风格和质量元</font></font></h1><a id="user-content-parameter-tags-and-atmosphere-and-style-and-quality_meta" class="anchor" aria-label="永久链接：参数：标签和氛围和风格和质量元" href="#parameter-tags-and-atmosphere-and-style-and-quality_meta"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">由于许多传播模型更喜欢标签，因此设计</font></font><code>tags</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为可能的替代品</font></font><code>description</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。如果与动漫模型一起使用，可以硬编码一些逻辑将所有“girl”替换为“1girl”。如果与 Pony 一起使用，则可能总是硬编码添加“score_9, score_8 ...”到其中。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>atmosphere</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>style</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是</font></font><code>quality_meta</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">一些没有非常具体用例的实验参数。目前我们可以将它们视为子提示，并将它们纳入子提示包的贪婪合并中。在我的实验中，这会稍微改善氛围和质量。</font></font></p>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基础渲染器</font></font></h1><a id="user-content-a-baseline-renderer" class="anchor" aria-label="固定链接：基础渲染器" href="#a-baseline-renderer"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这个 repo 中，我们根据注意力操纵为 Omost LLM 提供了基线渲染。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">区域提词员</font></font></h3><a id="user-content-regional-prompter" class="anchor" aria-label="永久链接：区域提示器" href="#regional-prompter"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">截至 2024 年，如果我们想要实现区域引导的扩散系统，一些可能的选择是：</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">多重扩散/混合扩散器：这些方法在不同位置运行 UNet，然后使用不同区域的权重或掩码合并估计的 epsilon 或 x0。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意力分解：假设注意力是这样的</font></font><code>y=softmax(q@k)@v</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，那么就可以实现注意力分解，其中</font></font><code>y=mask_A * softmax(q@k_A)@v_A + mask_B * softmax(q@k_B)@v_B</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mask_A、k_A、v_A是区域A的掩码，k、v；mask_B、k_B、v_B是区域B的掩码，k、v。这种方法通常能产生比（1）更好的图像质量，有些人称之为注意力耦合或区域提示注意力模式。但是这种方法有一个考虑：掩码只使区域注意力在数值上成为可能，但它并不强迫UNet真正关注这些区域的激活。也就是说，注意力确实被掩盖了，但不能保证注意力softmax真的会在被掩盖的区域中被激活，也不能保证注意力softmax永远不会在被掩盖的区域之外被激活。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意力分数操纵：与 (2) 相比，这是一种更先进的方法。它直接操纵注意力分数，以确保鼓励每个掩码区域中的激活，并阻止掩码之外的激活。公式类似于 ，</font></font><code>y=softmax(modify(q@k))@v</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其中</font></font><code>modify()</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是一个复杂的非线性函数，具有许多规范化和技巧来改变分数的分布。这种方法超越了简单的掩码注意力，真正确保这些层得到想要的激活。一个典型的例子是</font></font><a href="https://github.com/naver-ai/DenseDiffusion"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">密集扩散</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">梯度优化：由于注意力机制可以告诉我们每个部分对应哪个提示，我们可以将提示分成几段，然后获取每个提示段的注意力激活。然后我们将这些激活与外部掩码进行比较以计算损失函数，并反向传播梯度。这些方法通常质量很高，但占用大量 VRAM 且速度很慢。典型的方法是</font></font><a href="https://github.com/showlab/BoxDiff"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BoxDiff</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://github.com/yuval-alaluf/Attend-and-Excite"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">A&ZeroWidthSpace;&ZeroWidthSpace;ttend-and-Excite</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用外部控制模型，如 gligen 和</font></font><a href="https://github.com/frank-xwang/InstanceDiffusion"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">InstanceDiffusion</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。这些方法在区域跟踪方面提供了最高的基准性能，但由于它们是经过训练的参数，因此也会给基础模型引入一些风格偏移。此外，这些方法需要将提示转换为向量，并且通常不支持任意长度的提示（但可以将它们与其他注意方法一起使用以实现任意长度）。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更多可能的图层选项，如 layerdiffuse 和</font></font><a href="https://mulan-dataset.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">mulan</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
</ol>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这个 repo 中，我基于 (3) 编写了一个基线公式。我认为这个无参数公式是一个非常标准的基线实现，几乎不会引入任何风格偏移或质量下降。未来我们可能会考虑为 Omost 训练一些参数化方法。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">让我们考虑一个只有 2*2=4 个像素的极其简化的图像：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335492158-00f97ad6-202b-4a39-9091-da6d76b0aacb.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU0OTIxNTgtMDBmOTdhZDYtMjAyYi00YTM5LTkwOTEtZGE2ZDc2YjBhYWNiLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU3MTRkOTUzZDc5ZmZmZmUxZGFmYjIwNGQyNWVjNDE1OTBmYjMwYmI5OTI1YmU5YmU4NGVjOGRiM2FlYWEwNjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.uennUy5GTNDHINdVUfnWW4kvG_6B72Or0TcRfsAxhTw"><img src="https://private-user-images.githubusercontent.com/19834515/335492158-00f97ad6-202b-4a39-9091-da6d76b0aacb.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU0OTIxNTgtMDBmOTdhZDYtMjAyYi00YTM5LTkwOTEtZGE2ZDc2YjBhYWNiLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU3MTRkOTUzZDc5ZmZmZmUxZGFmYjIwNGQyNWVjNDE1OTBmYjMwYmI5OTI1YmU5YmU4NGVjOGRiM2FlYWEwNjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.uennUy5GTNDHINdVUfnWW4kvG_6B72Or0TcRfsAxhTw" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后我们有三个提示“两只猫”、“一只黑猫”、“一只白猫”，我们有它们的面具：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335492734-f9f5e87c-5f82-41fe-8a49-580d3eb6f2be.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU0OTI3MzQtZjlmNWU4N2MtNWY4Mi00MWZlLThhNDktNTgwZDNlYjZmMmJlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTFmZDQzNzAxNjdhZTM0ZWE2ZjA3NzIzY2M0NDc4NTNkMGM3NWRlZWZkMGViM2JiOWM5ZDUxZDgxNGI3YTcyZTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.O1Y9uoFETRLJNMgZ1-4KkJDG9SGIEIbFFoVtARtSwZI"><img src="https://private-user-images.githubusercontent.com/19834515/335492734-f9f5e87c-5f82-41fe-8a49-580d3eb6f2be.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU0OTI3MzQtZjlmNWU4N2MtNWY4Mi00MWZlLThhNDktNTgwZDNlYjZmMmJlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTFmZDQzNzAxNjdhZTM0ZWE2ZjA3NzIzY2M0NDc4NTNkMGM3NWRlZWZkMGViM2JiOWM5ZDUxZDgxNGI3YTcyZTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.O1Y9uoFETRLJNMgZ1-4KkJDG9SGIEIbFFoVtARtSwZI" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后我们可以画出这个注意力分数表：</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335493693-a77936b3-050e-4894-9252-476713144f6c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU0OTM2OTMtYTc3OTM2YjMtMDUwZS00ODk0LTkyNTItNDc2NzEzMTQ0ZjZjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTJiZTJjNTU1NTIzMzE0ZDc1ZDVkZDA5ZTUyOTljOTY0NTg0NmZlNjUxYzczZThjMzI4NzZlYWI5YTVmYzY2OTEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.j2h-krSskPq9WwHFCgPcplq5SCiO8cHmfeF2gdKL0Lo"><img src="https://private-user-images.githubusercontent.com/19834515/335493693-a77936b3-050e-4894-9252-476713144f6c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU0OTM2OTMtYTc3OTM2YjMtMDUwZS00ODk0LTkyNTItNDc2NzEzMTQ0ZjZjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTJiZTJjNTU1NTIzMzE0ZDc1ZDVkZDA5ZTUyOTljOTY0NTg0NmZlNjUxYzczZThjMzI4NzZlYWI5YTVmYzY2OTEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.j2h-krSskPq9WwHFCgPcplq5SCiO8cHmfeF2gdKL0Lo" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其中上面的箭头表示我们想要鼓励激活，而下面的箭头表示我们想要摆脱这些激活。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这种操作直接修改注意力分数，并在一次 SDP 注意力传递中计算所有提示条件。（有关更多详细信息，另请参阅代码。）</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提示前缀树</font></font></h3><a id="user-content-prompt-prefix-tree" class="anchor" aria-label="永久链接：提示前缀树" href="#prompt-prefix-tree"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这个 repo 中，我还介绍了另一个我发现的可以大大提高提示理解力的技巧。我们称之为提示前缀树。动机是，既然现在我们所有的提示都是可以任意合并的子提示（回想一下，所有子提示都严格少于 75 个标记，通常少于 40 个标记，描述独立的概念，并且可以任意合并为 clip 编码的通用提示），找到一种更好的方法来合并这些子提示可能会改善结果和提示解释。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">例如下面是全局/局部总体/详细描述的树结构。</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335572678-2b3a895f-9bb5-4da8-9d5d-989bac9c1a7e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NzI2NzgtMmIzYTg5NWYtOWJiNS00ZGE4LTlkNWQtOTg5YmFjOWMxYTdlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBkNjVlZGMxM2YwZTNmZWJjNDcyMmI4ZmJiOGIwNjFkOTk2ZjcxNGYxNzI3MjA3MTVlY2JjM2Q0ZGM3NWYyNTMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.U7_RSTpEMcPc6ngDJmpD6_4sKiYZC1BdKEY89nznj2U"><img src="https://private-user-images.githubusercontent.com/19834515/335572678-2b3a895f-9bb5-4da8-9d5d-989bac9c1a7e.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NzI2NzgtMmIzYTg5NWYtOWJiNS00ZGE4LTlkNWQtOTg5YmFjOWMxYTdlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBkNjVlZGMxM2YwZTNmZWJjNDcyMmI4ZmJiOGIwNjFkOTk2ZjcxNGYxNzI3MjA3MTVlY2JjM2Q0ZGM3NWYyNTMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.U7_RSTpEMcPc6ngDJmpD6_4sKiYZC1BdKEY89nznj2U" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这个想法是，由于所有子提示都可以任意合并，我们可以使用此树图中的路径作为提示。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">例如下面的路径将给出提示“一只猫和一只狗。沙发上的猫。”</font></font></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://private-user-images.githubusercontent.com/19834515/335572621-902ec939-65be-4232-912b-d1bc6f5da44f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NzI2MjEtOTAyZWM5MzktNjViZS00MjMyLTkxMmItZDFiYzZmNWRhNDRmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU1NTllZTZjYmU0NjUyZDA3OWIyODhhNmZjNjkyYTg5MGM3NzcwMTVlMjFjNDRlZGQwODBiNjZhMDFmZmJjYzEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.aQ1yG0i12zOkqLBvETOg5eFEgikbucSyWBVLH9CgxB4"><img src="https://private-user-images.githubusercontent.com/19834515/335572621-902ec939-65be-4232-912b-d1bc6f5da44f.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTczOTAwNzAsIm5iZiI6MTcxNzM4OTc3MCwicGF0aCI6Ii8xOTgzNDUxNS8zMzU1NzI2MjEtOTAyZWM5MzktNjViZS00MjMyLTkxMmItZDFiYzZmNWRhNDRmLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA2MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNjAzVDA0NDI1MFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU1NTllZTZjYmU0NjUyZDA3OWIyODhhNmZjNjkyYTg5MGM3NzcwMTVlMjFjNDRlZGQwODBiNjZhMDFmZmJjYzEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.aQ1yG0i12zOkqLBvETOg5eFEgikbucSyWBVLH9CgxB4" alt="图像" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，当路径超过 75 个标记时，我们可以将其与贪婪子提示包合并一起使用。而且，如果路径有剩余空间来包含更多子提示，贪婪子提示包合并也会处理它。同样，由于所有子提示都描述独立的概念，贪婪子提示包合并永远不会犯语义截断错误。太令人满意了！</font></font></p>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型说明</font></font></h1><a id="user-content-model-notes" class="anchor" aria-label="固定链接：模型说明" href="#model-notes"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><code>https://huggingface.co/lllyasviel/</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">目前我们提供3种型号（您可以通过在以下名称中</font><font style="vertical-align: inherit;">添加前缀来获取它们）：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>omost-llama-3-8b
omost-dolphin-2.9-llama3-8b
omost-phi-3-mini-128k
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="omost-llama-3-8b
omost-dolphin-2.9-llama3-8b
omost-phi-3-mini-128k" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以及它们的量化版本：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>omost-llama-3-8b-4bits
omost-dolphin-2.9-llama3-8b-4bits
omost-phi-3-mini-128k-8bits
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="omost-llama-3-8b-4bits
omost-dolphin-2.9-llama3-8b-4bits
omost-phi-3-mini-128k-8bits" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">一些说明：</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">推荐的量化为</font></font><code>omost-llama-3-8b</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">4 位，而</font></font><code>omost-phi-3-mini-128k</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">(3.8B) 的量化为 8 位。它们都适合 8GB VRAM，无需卸载。量化造成的性能下降非常小，我个人从未观察到任何性能下降的迹象。但是，</font></font><code>omost-phi-3-mini-128k</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不建议将量化为 4 位，因为我注意到了一些明显的性能下降。当您确实没有更强大的 GPU 时，4 位推断</font></font><code>omost-phi-3-mini-128k</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">应该被视为极端情况下的最后方法。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我的用户研究表明</font></font><code>omost-llama-3-8b-4bits</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">&gt; </font></font><code>omost-dolphin-2.9-llama3-8b-4bits</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">&gt; </font></font><code>omost-phi-3-mini-128k-8bits</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。因此，在大多数情况下，只需使用</font></font><code>omost-llama-3-8b-4bits</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>omost-llama-3-8b</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用</font></font><code>omost-phi-3-mini-128k</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">经过筛选的安全数据进行训练，不含 NSFW 或不当内容。如果您需要其他选项，请参阅 (4)。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">训练时使用所有数据，不进行任何过滤。如果您向</font><font style="vertical-align: inherit;">公众</font></font><code>omost-dolphin-2.9-llama3-8b</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">公开任何服务，则必须应用自己的安全校准方法。</font></font><code>omost-dolphin-2.9-llama3-8b</code><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，(3) 中的过滤不是因为任何策略 - 原因是我注意到这些模型中的训练梯度略有不稳定性，因为它们是使用受安全对齐控制的指令跟踪进行预训练的，导致性能略有下降。但是的指令跟踪</font></font><code>omost-dolphin-2.9-llama3-8b</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是在社区努力下进行预训练的，没有这个问题。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">128k 的上下文长度</font></font><code>omost-phi-3-mini-128k</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不可信。当 token 达到约 8k 时，其性能会大幅下降。应该将其视为内容长度约为 8k 的模型。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">8k 上下文长度的模型可以进行大约 5 到 6 轮对话编辑。如果您即将用完 token 长度，请使用 UI 修改消息并再次回复（这可以无限次完成）。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有模型都使用我们的 H100 集群在精度 fp16 下进行全面训练，没有使用任何类似量化或 Q-LoRA 等技巧。优化器是 Adam，没有任何技巧。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您还必须遵守 Llama-3 和 Phi-3 的许可证。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果合理且必要，您可以请求我们进行其他法学硕士学位的培训。</font></font></li>
</ol>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引用</font></font></h1><a id="user-content-cite" class="anchor" aria-label="永久链接：引用" href="#cite"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>@Misc{omost,
  author = {Omost Team},
  title  = {Omost GitHub Page},
  year   = {2024},
}
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@Misc{omost,
  author = {Omost Team},
  title  = {Omost GitHub Page},
  year   = {2024},
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">相关工作</font></font></h1><a id="user-content-related-work" class="anchor" aria-label="固定链接：相关工作" href="#related-work"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">另请阅读...</font></font></p>
<p dir="auto"><a href="https://google.github.io/docci/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">DOCCI：连通和对比图像的描述</font></font></a></p>
<p dir="auto"><a href="https://github.com/YangLing0818/RPG-DiffusionMaster"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（RPG-DiffusionMaster）掌握文本到图像的传播：使用多模态 LLM 进行重新描述、规划和生成</font></font></a></p>
<p dir="auto"><a href="https://arxiv.org/abs/2305.13655" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于 LLM 的扩散：使用大型语言模型和</font><a href="https://arxiv.org/abs/2311.16090" rel="nofollow"><font style="vertical-align: inherit;">自校正 LLM 控制的扩散模型</font></a><a href="https://arxiv.org/abs/2305.13655" rel="nofollow"><font style="vertical-align: inherit;">增强对文本到图像扩散模型的快速理解</font></a></font><a href="https://arxiv.org/abs/2311.16090" rel="nofollow"><font style="vertical-align: inherit;"></font></a></p>
<p dir="auto"><a href="https://multidiffusion.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">MultiDiffusion：融合扩散路径以控制图像生成</font></font></a></p>
<p dir="auto"><a href="https://github.com/hako-mikan/sd-webui-regional-prompter"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">sd-webui-区域提示器</font></font></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（如果您想在此处添加更多链接，请打开问题或给我发送电子邮件）</font></font></p>
</article></div>
