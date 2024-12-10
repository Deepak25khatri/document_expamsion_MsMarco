# document_expansion_MsMarco
# Advanced Document Ranking with BART, T5, and BERT

This repository documents our efforts in enhancing document ranking using combinations of BART, T5, BM25, RM3, and BERT for reranking. We replicate existing methods and propose our improvements to achieve superior results in Mean Reciprocal Rank (MRR) at 10.

## Results Summary

Our experiments leverage techniques from the [doc2query](https://github.com/nyu-dl/dl4ir-doc2query) project by NYU, enhancing them with our unique modifications. Below is a summary of our findings:

| Model Combination    | MRR@10 |
|----------------------|--------|
| BART + BM25          | 19.33  |
| BART + BM25 + RM3    | 17.42  |
| BART + BM25 + BERT(Reranking) | 35.2   |
| T5 + BM25            | 27.6   |
| T5 + BM25 + RM3      | 21.5   |
| T5 + BM25 + BERT(Reranking)   | 37.5   |

![Results Overview](path/to/image.png)  <!-- Please adjust the path to where your image is hosted -->

## Dataset and Resources

To facilitate replication and further research, we provide links to all necessary datasets and resources used in our training and inference processes:

- **MS MARCO Passage Ranking Dataset**: [Download](https://microsoft.com/msmarco)
- **Anserini Toolkit for Indexing and Retrieval**: [GitHub](https://github.com/castorini/anserini)
- **BERT, BART, and T5 Models**: [Hugging Face Model Hub](https://huggingface.co/models)

## Setup and Replication

Follow these steps to replicate our experiments and further explore document ranking enhancements:

1. **Environment Setup**:
   Ensure you have Python and Java installed, along with all necessary libraries and frameworks like PyTorch, Transformers, and Anserini.

2. **Data Preparation**:
   Download and prepare the MS MARCO dataset by converting the collection and filtering queries without relevance.

3. **Model Training**:
   Train your BART and T5 models using the provided scripts, adjusting parameters as needed for your specific hardware and dataset.

4. **Evaluation**:
   Use the provided evaluation scripts to measure the MRR@10 of your models, comparing them against our baseline and improved results.

## Conclusion

Our experiments demonstrate significant improvements in document ranking, particularly with the use of BERT for reranking. For further details, refer to our full experimentation logs and analysis provided in this repository.

