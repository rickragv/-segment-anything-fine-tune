# segment-anything-fine-tune
![Alt text](./data/section-3.1c.gif?raw=true "Title")

SAM is a powerful image semantic segmentation model designed to accurately predict pixel-level masks for a wide range objects within an image. It consists of three parts:

#### Image encoder 
- a heavy vision transformer backbone that generates image features.
#### Prompt encoder 
- a lightweight embedding module that creates sparse and dense embeddings out of prompt inputs (points, boxes and or masks).
Mask 
#### decoder 
- a decoder that takes outputs of the image encoder and the prompt encoder to produce masks.


![Alt text](./data/sam.jpg?raw=true "Title")

 Image is passed through the image encoder, then its latent features are combined with prompt features before feeding into the mask decoder. Finally, output masks are generated.

## Custom fine-tuned SAM output for Road segmentation 


![Alt text](./data/sat.JPG?raw=true "Title")

SAM paper: https://arxiv.org/pdf/2304.02643.pdf​

Link to the dataset used in this demonstration: https://www.kaggle.com/insaff/massachusetts-roads-dataset