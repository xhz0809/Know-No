## Datasets

This folder contains three datasets used in the KNOW-NO benchmark. Below is a brief description of each dataset included.

### 1. MC-TEST 1000
- **Source**: [Richardson et al., 2013](https://aclanthology.org/D13-1020/).
- **Description**: A multiple-choice reading comprehension benchmark.
- **Number of Instances**: 250 stories (1,000 questions, instance-level labels).
- **Challenge Level**: Low.

 #### Data Structure
  - `id`: unique story id.
  - `story`: the story.
  - `question_list`: a list of four multiple-choice questions.
    - `question`: question
    - `options`: a list of four options
    - `gold_option`: the ground truth option 

### 2. BANK-77 1000
- **Source**: [Casanueva et al., 2020](https://arxiv.org/abs/2003.04807).
- **Description**: This dataset consists of customer service queries in the banking and financial domain.
- **Number of Instances**: 1,000 (subset from the original 13,083).
- **Challenge Level**: Moderate.

 #### Data Structure
  - `text`: customer service query.
  - `label`: intent class index.
  - `label_text`: intent class.
   
### 3. EQUINFER 1049
- **Source: proposed by us and has never been seen by LLMs**
- **Description**: A new dataset designed to evaluate equation inference based on context in scientific papers.
- **Number of Instances**: 1,049.
- **Challenge Level**: High.

 #### Data Structure
  - `context_before`: LaTeX source code of 1000-word-context before the equation.
  - `context_after`: LaTeX source code of 1000-word-context after the equation.
  - `options_list`: a list of four equation options in LaTex format.
  - `gold_option`: the gold equation in LaTex format.
  - `gold_option_index`: the gold equation in LaTex format.
