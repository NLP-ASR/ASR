# ASR
Automatic Speech Recognition

## Timeline

STEP 1: Due (Apr 10, Monday)
These are the minimal requirements, we can do anything else that benefits the overall project.

All of us should be thouroughly comfortable with [wav2vec](https://arxiv.org/abs/2006.11477) and [bigfoot paper](https://arxiv.org/abs/2103.15760) - the details of dataset used,size,preprocessing, data-augmentation(SpecAugmen),loss. **We should make an attempt at gaining clarity, not a vague idea.** Do what ever necessary for this before our next meet. If we can learn to handle ambiguity , and gain the skill of figuring things out - that would be good bang for our effort.


Some useful tools:(how to get unstuck)

1. ipdb/pdb -> putting breakpoints in code and running line by line . We use this all the time in the industry.

2. Understand one component at a time. For instance wav2vec uses CTC loss. look for implementations of CTC loss and step through the code with ipdb/pdb. pay attention to shapes,types of tensors and form a mental model of the code.

3. Annotate/commenting the code - your future version or others will greatly appreciate this.




`Ronitde`

Load the full dataset and prepare it for model training. 

`Vinay`

Implement a working prototype of Knowledge distillation + write the first draft of the report.

`Govind`

Run an end-end Wave2vec2.0 model.
