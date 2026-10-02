# Vision Desk

Capstone for **Computer Vision in Finance** (Master's Finance, Data & AI).

Parallel to Signal Desk (LSTM): fine-tune a **ViT**, expose it via **MCP** tools, and check whether an LLM answer is **grounded** or invented.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Amzil-AI/Vision-desk/blob/main/vision_desk_colab.ipynb)

## Quick start

1. Open the Colab badge above  
2. Runtime → GPU (T4) if available → **Run all**  
3. Check: document split, ViT vs majority baseline, grounded trace, refusal  

```bash
pip install -r requirements.txt
# or use the notebook in Colab / Jupyter
```

## Layout

```
vision_desk_colab.ipynb   # student lab
requirements.txt
case/                     # student brief (FR + EN, PDF + TeX)
solution/                 # teacher solution (FR + EN) + lab-reference/
```

| Path | Audience |
|---|---|
| `vision_desk_colab.ipynb` | Students |
| `case/*.pdf` | Students |
| `solution/*.pdf` | Teachers |
| `solution/lab-reference/` | Recorded metrics & MCP traces (`SEED=42`) |

## Closed task

Build a Vision Desk on a financial image:

1. What can the vision model assert?  
2. Which MCP tool / JSON field justifies each claim?  
3. What do you refuse when a tool fails or returns null?  

## Lab outline

1. Synthetic finance images (candlestick / line / balance sheet / notes)  
2. Split **by document**  
3. Fine-tune `vit_tiny_patch16_224` (head)  
4. JSON contract via `vision.extract`  
5. MCP stubs → grounded answer + refusal  
