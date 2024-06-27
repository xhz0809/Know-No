## Datasets

This folder contains three datasets used in the KNOW-NO benchmark. Below is a brief description of each dataset included.

### 1. MC-TEST 1000
- **Source**: [Richardson et al., 2013](https://aclanthology.org/D13-1020/).
- **Description**: A multiple-choice reading comprehension benchmark.
- **Inputs**: Elementary-school-level stories.
- **Labels**: Each story is followed by four multiple-choice questions, with four unique answer options per question.
- **Label Scope**: Instance-level (each question has a unique set of labels).
- **Number of Instances**: 250 stories (1,000 questions).
- **Challenge Level**: Low.

#### Data Structure
 - `id`: unique story id.
 - `story`: the story.
 - `question_list`: a list of four multiple-choice questions.
   - `question`: question
   - `options`: a list of four options
   - `gold_option`: the ground truth option 

#### 2. BANK-77 1000
- **Source**: [Casanueva et al., 2020](https://arxiv.org/abs/2003.04807).
- **Description**: This dataset consists of customer service queries in the banking and financial domain.
- **Inputs**: Simple sentences.
- **Labels**: 77 intents.
- **Label Scope**: Task-level (all instances share the same set of labels).
- **Number of Instances**: 1,000 (subset from the original 13,083).
- **Challenge Level**: Moderate.

#### 3. EQUINFER 1049
- **Source: proposed by us and has never been seen by LLMs**
- **Description**: A new dataset designed to evaluate equation inference based on context in scientific papers.
- **Inputs**: LaTeX source code of the context (1,000 words) before and after an equation in NLP papers.
- **Labels**: Each instance includes one correct equation and three negative options.
- **Label Scope**: Instance-level.
- **Number of Instances**: 1,049.
- **Challenge Level**: High.

