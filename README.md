# Binary_Classification_of_Populist_Discourse
 Binary Classification of Populist Discourse

The code can be run all together with no issues given the right GPU and Database path.

The code was run in Google Colab using a high-ram A100 GPU, which could withstand a highest batch size of 128 for BERT-tiny and of 20 for the larger models, and this can be replicated.

Results with local CPU or GPU can be obtained if the batch size is reduced to 8 for single-model runs and to 2 to 4 for running the whole code, depending on the memory of the hardware.