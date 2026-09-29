# LifeLink Command Center

On-device AI triage for offline disaster SOS traffic, built for Snapdragon-powered HP PCs.

## Problem
Disasters can knock out cellular and internet networks. SOS messages that still get through are messy (text, voice, photos, many languages) and have no clear priority.

## What it does
- Receives SOS from the LifeLink BLE smartphone mesh
- Voice SOS to text, triage and priority scoring, multilingual summaries, damage photo check
- Ranked SOS dashboard and offline map

## Architecture
Phones -> BLE mesh -> Snapdragon laptop -> On-device AI -> Dashboard -> Rescue dispatch

## Models
| Task | Model | Source |
|---|---|---|
| Speech to text | (add) | Qualcomm AI Hub |
| Triage / summary | (add) | Qualcomm AI Hub / open source |
| Damage photo | (add) | Qualcomm AI Hub |

## Snapdragon optimization
Models are quantized and run on the Snapdragon NPU with ONNX Runtime (QNN).

## Setup
1. Snapdragon-powered Windows PC with Python installed
2. Install dependencies
3. Run the command app

## Credits
BitChat, Qualcomm AI Hub, UNDRR