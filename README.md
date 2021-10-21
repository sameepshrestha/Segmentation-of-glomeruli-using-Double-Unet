# Segmentation-of-glomeruli-using-Double-Unet
Hacking the kidney

The best estimates show there are over 7 billion people on the planet and 300 billion stars in the Milky Way galaxy. By comparison, the adult human body contains 37 trillion cells. To determine the function and relationship among these cells is a monumental undertaking. Many areas of human health would be impacted if we better understand cellular activity.

This notebook attempts to detect functional tissue units (FTUs) across different tissue preparation pipelines. An FTU is defined as a “three-dimensional block of cells centered around a capillary, such that each cell in this block is within diffusion distance from any other cell in the same block” (de Bono, 2013). The goal of this notebook is the implementation of a successful and robust glomeruli FTU detector.

Implementation used was Double U-net based on the paper
https://arxiv.org/abs/2006.04868

The architecture of the model was changed with various encoder implementation but the basic structure follows- 

![architecture](https://user-images.githubusercontent.com/66662839/138275574-8db6af68-376a-4274-beaa-e39de5db84a5.PNG)

Both training with and without freezing of the encoder was tested and no significant change with training without freezing was observed.
Segmentation 
comparision between the real and predicted results
![segment](https://user-images.githubusercontent.com/66662839/138274734-b44a82c9-c642-4ada-bcad-574541fe774a.PNG)
