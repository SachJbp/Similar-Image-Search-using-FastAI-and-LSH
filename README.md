# Similar-Image-Search-using-FastAI-and-LSH
Fast near neighbor search for images is a problem that has wide industry use cases. Here , I have used FastAI and LSH to enable fast similar image search. 

1) We use a Resnet-34 pretrained model  and use the last second last layer to get embeddings for Caltech-101 dataset 
2) Locality sensitive hashing is done using lshash library which enables fast near neighbor search
3) Given an image, we can pass it through pretrained Resnet-34 to get the embeddings which can then be fed to LSH object as a query to get its 'k' nearest neighbors

This is a demo work and for real life datasets, one would want to train the last few layers using the dataset to fine tune the model before fetching the embeddings.
