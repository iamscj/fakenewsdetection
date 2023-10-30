# Fake News Detection with Various RNN and Transformer Models

This project focuses on fake news detection using different recurrent neural network (RNN) and transformer models. The analysis is performed on the Liar Dataset, which contains statements labeled as true or false. The primary goal is to assess the performance of various models in distinguishing between true and false statements.

## Dataset

- **Liar Dataset**: The dataset used for this project consists of statements labeled as "true" or "false," along with additional information.

## Models Implemented

1. **LSTM Model**: A Long Short-Term Memory (LSTM) neural network model was developed for fake news detection. LSTM is a type of RNN known for its effectiveness in processing sequences.

2. **SimpleRNN Model**: A Simple RNN model was implemented. Simple RNNs are fundamental RNNs used for sequential data analysis.

3. **GRU Model**: A Gated Recurrent Unit (GRU) model was employed. GRUs are similar to LSTMs but have a reduced number of parameters.

4. **Transformer BERT Model**: A transformer model based on BERT (Bidirectional Encoder Representations from Transformers) was used. Transformers have achieved state-of-the-art results in various natural language processing tasks.

## Training and Evaluation

- Each model was trained on the Liar Dataset using a common preprocessing pipeline.
- The evaluation included calculating accuracy and generating confusion matrices to assess model performance.
- The dataset was divided into training and test sets, with test samples being used for evaluation.

## Results

### SimpleRNN Model

- **Accuracy**: 0.570
- **Confusion Matrix**:

[[ 446, 760],
[ 694, 1479]]

![image](https://github.com/iamscj/fakenewsdetection/assets/91722818/5b3c8bbe-7547-4296-a730-27596aca971e)


### GRU Model

- **Accuracy**: 0.582
- **Confusion Matrix**:

[[ 482, 724],
[ 688, 1485]]

![image](https://github.com/iamscj/fakenewsdetection/assets/91722818/c5196b2e-e470-4ae8-9801-6a6565a36119)

**Why GRU Proved to Be the Best**:
The GRU model outperformed the LSTM model and other models in fake news detection due to its ability to effectively capture sequential patterns while having a more efficient architecture. The GRU's gating mechanism allows it to mitigate the vanishing gradient problem and retain important information. Its lower parameter count also contributes to faster training.

### Transformer BERT Model

- **Accuracy**: 0.530
- **Confusion Matrix**:
[[1244, 2394],
[2419, 4182]]

![image](https://github.com/iamscj/fakenewsdetection/assets/91722818/cffa6139-9a2e-4f5f-8693-8255944696c3)


### LSTM Model

- **Accuracy**: 0.579
- **Confusion Matrix**:

[[ 490, 716],
[ 706, 1467]]

![image](https://github.com/iamscj/fakenewsdetection/assets/91722818/f8dac046-1da1-4d6f-9c99-3e607f530a52)


## Conclusion

- Among the models evaluated, the **GRU Model** achieved the highest accuracy at 0.582. This indicates its suitability for fake news detection on the Liar Dataset.
- While the Transformer BERT Model showed potential, it had a slightly lower accuracy of 0.530.
- The LSTM and SimpleRNN models also demonstrated reasonable performance, with accuracy scores of 0.579 and 0.570, respectively.

In summary, the GRU Model stands out as the most effective model for fake news detection on the Liar Dataset, thanks to its ability to capture sequential patterns efficiently and mitigate the vanishing gradient problem.

## Usage

Provide instructions on how to use the code, including any necessary installations, preprocessing steps, and model training.

## License

This project is licensed under the XYZ License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Mention any individuals, organizations, or resources you would like to acknowledge.

## References

- Liar Dataset: [Link to Dataset](https://example-link.com)
- Transformer Models: [Hugging Face Transformers](https://huggingface.co/transformers/)

Feel free to adapt this template to include your specific dataset and results while maintaining the structured format. The README provides a clear structure for summarizing your work.
