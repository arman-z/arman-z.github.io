Note: we suggest using tools similar to "gifview" to examine each frame of a gif file separately.

The given *.gif files explore a spectrum of tree regularization parameter \lambda for parametric t-SNE (on MNIST) and elastic embedding (on 20 newsgroups). Each image in a gif is similar to the fig. 3 in the main paper: it shows 2D projections obtained by different methods (bottom) and the corresponding tree (top) for each value of \lambda (regularization parameter for TAO). We also plot objective function value after each iteration of our method (bottom-right).

Regarding decision trees:
- for 20 newsgroups (internal nodes), we show the sparsity of the weight vector (in titles) and up to top 7 words which correspond to the largest positive (blue) or negative (red) non-zero weights.
- for mnist (internal nodes), we show non-zero entries of the weight vector (reshaped into 28x28 matrix to represent an MNIST image).

At each leaf (in both datasets), we show the region of its responsibility and provide histogram counts of classes. We draw the region as follows: we collect all instances falling into that leaf and apply projection mapping to obtain 2D embeddings. Then we calculate the convex hull using these 2D embeddings and draw them using the red line.

Encoding of the x axis in leaf histograms for 20 newsgroups. b: 'rec.motorcycles', h: 'rec.sport.hockey', c: 'sci.cryptography', s: 'sci.space', m: 'talk.politics.mideast', g: 'talk.politics.guns'.
