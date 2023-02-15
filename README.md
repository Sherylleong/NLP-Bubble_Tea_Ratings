# NLP-Bubble_Tea_Ratings
Training a sequential network with NLP to predict ratings my friend would give based on his compiled reviews of different bubble teas.

_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 embedding_1 (Embedding)     (None, 88, 16)            6336      
                                                                 
 global_average_pooling1d_1   (None, 16)               0         
 (GlobalAveragePooling1D)                                        
                                                                 
 dense_2 (Dense)             (None, 24)                408       
                                                                 
 dense_3 (Dense)             (None, 1)                 25        
                                                                 
=================================================================
Total params: 6,769
Trainable params: 6,769
Non-trainable params: 0
_________________________________________________________________

When testing custom reviews, the review string "the best milk tea i have ever had, tastes heavenly and worth every penny, highly recommended" achieved a rating of 5.95/10, while the string  "tastes bad, very bland, too expensive, not worth the money. do not buy" achieved 5.92/10, so the effectiveness of the model is suspect. May need more advanced NLP labelling techniques or more data.
