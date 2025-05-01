# UniOVA Dataset

This repository contains the datasets used in our research paper [UniOVA: Universal On-demand Video Analytics with Edge-Cloud Collaborative Multimodal LLM]. 
It includes processed data for two main datasets: **CG-Bench-Interest** and **UCF-Crime-Interest**. 
These datasets are structured specifically for our research focus and support the findings and conclusions outlined in our paper.

## Datasets

1. **CG-Bench-Interest**
   - This dataset is derived from the original CG-Bench dataset. It includes additional annotations and preprocessing specific to our research.
   - Original Dataset: [CG-Bench on Hugging Face](https://huggingface.co/datasets/CG-Bench/CG-Bench)

2. **UCF-Crime-Interest**
   - This dataset is a modified version of the UCF-Crime dataset, with a selection of videos and annotations relevant to our study.
   - Original Dataset: [UCF-Crime Project Page](https://www.crcv.ucf.edu/projects/real-world/)

## Description of CG-Bench-Interest Dataset Parameters
Each element in the CG-Bench-Interest dataset is structured as a JSON object containing the following parameters:
- **`video_uid`**: Unique identifier for the video. This serves as a reference to match the data with the original video dataset.
- **`question`**: A textual question based on the context or elements presented in the video.
- **`answer`**: The correct answer to the provided question.
- **`choices`**: An array containing multiple-choice options relevant to the question..
- **`right_answer`**: The code (e.g., "E") corresponding to the correct answer within the `choices` array.
- **`duration`**: The total length of the video in seconds.
- **`interest`**: A keyword indicating the primary element or theme of interest within the video, used for focusing research efforts on particular aspects (e.g., "fire").
- **`mcq_questions`**: A formatted string of the multiple-choice question, presenting both the question and array choices in a human-readable format suitable for direct examination or transcription.
- **`question_index`**: An index that specifies the order or position of the question within a dataset sequence.

## Description of UCF-Crime-Interest Dataset Parameters
Each element in the UCF-Crime-Interest dataset is structured as a JSON object containing the following parameters:
- **`video_uid`**: The unique identifier for the video file. The filename (e.g., "Arson024_x264.mp4") is used to reference or locate the video within the dataset.
- **`question`**: A textual question based on the context or elements presented in the video.
- **`answer`**:  The correct answer to the provided question.
- **`interest`**: A keyword indicating the primary element or theme of interest within the video, used for focusing research efforts on particular aspects (e.g., "fire").
- **`question_index`**: An index that specifies the order or position of the question within a dataset sequence.
- **`duration`**: The total length of the video in seconds.


## Important Note

This repository **does not** include the original video files for CG-Bench or UCF-Crime datasets. 
To obtain these files, you must download them from their respective sources linked above.
