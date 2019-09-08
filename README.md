# VQA

The Visual Question Answering (VQA) systems predict the answer of the question related to an image. We have performed Visual
Question Answering on COCO-VQA dataset which has open-ended questions and open-ended answers associated with
an image. We studied prior work related to VQA and built a base model which uses the VGG16 architecture for image and GloVe
Embedding for question processing. We further improved upon the base model by using attention features of an image. It helps the algorithm to focus on the specific region of an image related to a question. Additionally, we explored the different
hyperparameters and we compare our results with state-of-the-art models.

The COCO-VQA dataset can be downloaded from the link - https://visualqa.org/
It consists of approximately 83K training images, 41K validation images, and 81K testing images of MS COCO dataset, this is best suited for our project as it provides a broad category of object. Each image contains 3 questions and each question has 10 answers answered by 10 different human annotators. We have used train-test-validation data split from [1] same as MS COCO dataset.

The main goal of the system is classification. Predicting the answer given a question related to an image. It will use the
combine features of input image and question and succeeded by the multinomial classifier which classifies into the answer.
This was done by implementing and comparing the results of two models with open-ended question from COCO-VQA Dataset - one base model and one attention model. Moreover, instead of GloVe embedding, as was used here, different other types of embedding can be explored like FastText word embedding or ELMo (Deep Contextualized word representations). Also, the attention model can be made more complex, like bilinear attention networks, to explore further options. Knowledge from external sources can be
embedded into the system to help it to answer the factual question like Fire extinguisher seen in the image can resolve
the fire? These can be considered as options for future enhancements for the project.
