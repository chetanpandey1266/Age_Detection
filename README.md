# Age_Detection_of_Actors
Analytics Vidya CV competition

### Practices I followed
1. I used 4 different pretrained models.

(a) Resnet50 - 0.66109-0.73312

(b) Densenet121 - 0.6675-0.8292

(c) Efficientnet_b0 - 0.8725-0.9082

(d) Efficientnet_b1 - o.9082-0.91305


2. I have used 40-50 epochs for each model. I have used Adam and SGD optimizer together, first 20 with Adam to finetune the model(i.e. to train the last layer and the last 20-30 epochs with SGD to train full model.


3. Finetuning is to be used for resnet and densenet only as they have more parameters than efficientnet, which can be trained without finetuning for 30-40 epochs. 


4. For the first 20 epochs I have used learning rate= 1e-3 and for the next 20-30 epochs used 1e-4. 


5. I have also used ReduceOnPlateau scheduler with 3-4 patiece.


### Future Plans

1. Straightified K-fold
2. Test Time Augmentation
3. Ensembling 
4. Pseudolabeling
