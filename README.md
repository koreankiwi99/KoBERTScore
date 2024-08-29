# Ko-BERTScore

## Dependencies
This fork is compatible with:

* NumPy: Version 1.24 or higher
* Transformers: Version 4.42.4 or higher

## Changes in This Fork
* NumPy Compatibility: Updated usage of np.int to np.int32 to align with recent NumPy updates.
* Transformers Compatibility: Refactored code to use the updated method signatures and attributes:
    * `Original`: _, _, hidden_states = bert_model(input_ids, attention_mask=attention_mask, output_hidden_states=True)
    * `Updated`: output = bert_model(input_ids, attention_mask=attention_mask, output_hidden_states=True); hidden_states = output.hidden_states

## Usage
The usage of KoBERTScore remains the same as in the original repository. Refer to the original documentation for more details on how to use the tool.

## Acknowledgement
This fork is based on the original [KoBERTScore](https://github.com/lovit/KoBERTScore) project.
