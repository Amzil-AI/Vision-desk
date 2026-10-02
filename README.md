# Vision Desk

Capstone case for **Computer Vision in Finance** (Master's Finance, Data & AI).

Parallel to Signal Desk (LSTM): here students fine-tune a **ViT**, expose it via **MCP** tools, and judge whether an LLM answer is **grounded** or invented.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LikhitaYerra/vision-desk/blob/main/vision_desk_colab.ipynb)

## Fastest path (Colab)

1. Open the badge above  
2. Runtime → GPU (T4) if available → Run all  
3. Check: document split, ViT vs majority baseline, grounded trace, refusal

## Files

| File | Audience |
|---|---|
| `vision_desk_colab.ipynb` | Student lab (Colab) |
| `Computer-Vision-Finance-M2-Cas-Vision-Desk.pdf` | Student brief (FR) |
| `Computer-Vision-Finance-M2-Cas-Vision-Desk-EN.pdf` | Student brief (EN) |
| `Computer-Vision-Finance-M2-Corrige-Vision-Desk.pdf` | Teacher solution (FR) |
| `Computer-Vision-Finance-M2-Corrige-Vision-Desk-EN.pdf` | Teacher solution (EN) |

Matching `.tex` sources are included for edits.

## Closed task

Build a Vision Desk on a financial image: what can the vision model assert, which MCP tool justifies each claim, and what do you refuse when a tool fails?

## Lab outline

1. Synthetic finance images (candlestick / line / bilan / notes)  
2. Split **by document**  
3. Fine-tune `vit_tiny_patch16_224` (head)  
4. JSON contract via `vision.extract`  
5. MCP stubs + grounded answer + refusal
