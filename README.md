# VidLife 

VidLife contains personal life events with triple forms from The Big Bang Theory, eg. (Leonard, visit, Penny), which is designed for training and evaluating personal life event extraction systems.

You could download part of the life events annotations, which is released in this repository.
The complete dataset will be made available online after our paper is accepted.

# Data Description

VidLife contains 14,343 training examples, 1,793 examples for validation and 1,793 examples for testing.
We distinguish life events into high-level life events and low-level life events, and regard an activity that comprises a specific action only, and the action acts on a concrete object as a low-level activity. High-level activities which consist of several low-level activities express relatively complex life events.

In the paper, we initiate a novel life event extraction task and present a life event extraction system, LifeEventMiner as a baseline model.

## Data Format 

Each example in VidLife is a video clip with its corresponding bounding box, subtitle from TVQA+ dataset and multi-label life event annotation.

```json
"vid_name": "s01e01_seg01_clip_00",
"img_path_ts": "[[img_path, timestamp], ..]",
"bbox": "[[label, left, top, height, width], ..]"
"subtitle_ts": "Sheldon: "...", .."
"labeled_SVO_ts": "[['Leonard', 'put', 'a piece of paper', timestamp], ['Leonard', 'hold', 'hand', timestamp]]"
"labeled_train_SVO_ts": "[[0, 2, 1, timestamp], [0, 41, 18, timestamp]]"
"ground_truth_QA_pair(or sentence)": "[['Question', 'Answer'], ..]"
```

For the use of video clips with bounding box, subtitle and ground truth question-answer pair, please find TVQA+ dataset website:https://tvqa.cs.unc.edu/.

## Data Statistics

VidLife includes 29 sorts of high-level activities and 14 sorts of low-level activities.

## How to Cite the Corpus

Please cite the following papers when referring to the VidLife in academic publications and papers.

Tai-Te Chu, An-Zi Yen, Wei-Hong Ang, Hen-Hsen Huang, and Hsin-Hsi Chen. 2021. VidLife: A Dataset for Life Event Extraction from Videos. In Proceedings of the 30th ACM International Conference on Information and Knowledge Management.

## Contact Us

This work is done by Natural Language Processing laboratory from National Taiwan University (NTU).
If you would like to share feedback or report concerns, please e-mail us at <tdjhu@nlg.csie.ntu.edu.tw>



