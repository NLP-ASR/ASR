# ASR
Automatic Speech Recognition

# USAGE
Navigate to `ASR/Bigfoot/examples/wav2vec2_compression_demo` and run `wav2vec2_compression_demo.py`. To specify the config modify the `demo_config.yaml`. The default params shows how to run 4 layer transformer wave2vec model with weight sharing in conv layers sperified by `conv_groups: 2` parameter. Set `change_conv_layers: False` to run default architechure. We modified the code at [kdtoolkit](https://github.com/georgian-io/Knowledge-Distillation-Toolkit) for our task.

# Pretrained weights:

1. Weight shared(cnn) student model with 4 Transformer layers: https://drive.google.com/file/d/10fbt3q-a4MyNRTHkeqvccj0sOIa79hB9/view?usp=sharing


## Timeline(comments for the team)

STEP 1: Due (Apr 10, Monday)
These are the minimal requirements, we can do anything else that benefits the overall project.

All of us should be thouroughly comfortable with [wav2vec](https://arxiv.org/abs/2006.11477) and [bigfoot paper](https://arxiv.org/abs/2103.15760) - the details of dataset used,size,preprocessing, data-augmentation(SpecAugmen),loss. **We should make an attempt at gaining clarity, not a vague idea. We will not use fancy names, words != understanding.** Do what ever necessary for this before our next meet. If we can learn to handle ambiguity , and gain the skill of figuring things out - that would be good bang for our effort.


Some useful tools/suggestions:(how to get unstuck)

1. ipdb/pdb -> putting breakpoints in code and running line by line . We use this all the time in the industry.

2. Understand one component at a time. For instance wav2vec uses CTC loss. look for implementations of CTC loss and step through the code with ipdb/pdb. pay attention to shapes,types of tensors and form a mental model of the code.

3. Annotate/commenting the code - your future version or others will greatly appreciate this.

4. Make a mental model of what you need to thorughly understand vs can ignore.(for instance detail of CTC loss is useless as we are tranining on a different objective)




`Ronitde`

Load the full dataset and prepare it for model training. 

`Vinay`

Implement a working prototype of Knowledge distillation + write the first draft of the report.

`Govind`

Run an end-end Wave2vec2.0 model.


## Lessons

1. install fairseq_mod.
2. torch._overrides to torch.overrides
