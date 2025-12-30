# HAM10k_with_DenseNet121
Skin lesions' images classification with Dense121

Ham10K is an ISIC 2018 challenge's dataset with 7 classes of skin cancer diseases with over 10,000 iamges.
But the training dataset suffers a huge inter-classes data imbalance making it more difficult for models to learn the features of dataset.
Thus harder to make correct predictions. Even from the sources of the Ham10k dataset, doctor still struggle to confidently predict and verify 50% skin lesions without years follow-up cases, microscopic and colleges assitance. Making the rest 50% of the dataset is pathologic verification.

On approaching this matter, the first things come to mind is create augmented or synthetic data to cover up for the imbalance. But as stated in the Ham10 paper, the dataset had gone through histogram contrast adjusting already. So I just gonna ONLY try to randomly rotate and flip 2-side-way, not affecting the color contrast of the dataset. 