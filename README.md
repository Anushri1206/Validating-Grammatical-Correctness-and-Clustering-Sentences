# Validating-Grammatical-Correctness-and-Clustering-Sentences

This project parses sentences and checks the grammatical correctness of sentences and clusters similar sentences.

Sample Input and Module Wise Output

Input Paragraph - hummingbirds are the smallest birds in the world. they are the only birds to be able to fly backwards. anacondas are the biggest snakes in the world. pythons are the longest snakes in the world.

PoS Tagging - [('hummingbirds', 'NNS'), ('are', 'VBP'), ('the', 'DT'), ('smallest', 'JJS'), ('birds', 'NNS'), ('in', 'IN'), ('the', 'DT'), ('world', 'NN'), ('.', '.')] [('they', 'PRP'), ('are', 'VBP'), ('the', 'DT'), ('only', 'JJ'), ('birds', 'NNS'), ('to', 'TO'), ('be', 'VB'), ('able', 'JJ'), ('to', 'TO'), ('fly', 'VB'), ('backwards', 'NNS'), ('.', '.')] [('anacondas', 'NNS'), ('are', 'VBP'), ('the', 'DT'), ('biggest', 'JJS'), ('snakes', 'NNS'), ('in', 'IN'), ('the', 'DT'), ('world', 'NN'), ('.', '.')] [('pythons', 'NNS'), ('are', 'VBP'), ('the', 'DT'), ('longest', 'JJS'), ('snakes', 'NNS'), ('in', 'IN'), ('the', 'DT'), ('world', 'NN'), ('.', '.')]

Grammar Validation Output - hummingbirds are the smallest birds in the world - accepted
they are the only birds to be able to fly backwards - accepted
anacondas are the biggest snakes in the world - accepted
pythons are the longest snakes in the world - accepted

Clustering Output - 
cluster 0 :
sentence 0 :
hummingbirds are the
smallest birds in the
world
sentence 1 :
they are the only birds
to be able to fly
backwards
Keys : {'birds'}
Jaccard Similarity
Score: 0.14
cluster 1 :
sentence 0 :
anacondas are the
biggest snakes in the
world
sentence 1 :
pythons are the
longest snakes in the
world
Keys : {'world',
'snakes'}
Jaccard Similarity
Score: 0.33
