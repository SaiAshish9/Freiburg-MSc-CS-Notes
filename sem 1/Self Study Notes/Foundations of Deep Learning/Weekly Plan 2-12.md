

### [[MLP|MLPs (Multi-Layer Perceptrons)]]

#concept #mlp #deep-learning

- The foundational feedforward deep learning model that bridges traditional machine learning to deep networks.
- Utilizes multiple stacked hidden layers with non-linear activation functions to learn complex representations from input data.

### [[SGD|SGD (Stochastic Gradient Descent)]]

#concept #sgd #optimization

- A fundamental iterative optimization algorithm used to train neural networks on non-convex loss landscapes.
- Computes gradients and updates weights using small, randomly sampled batches of data to speed up convergence and escape local minima.

### [[CNN|CNNs (Convolutional Neural Networks)]]

#concept #cnn #computer-vision

- Specialized neural network architectures designed for grid-structured data like images.
- Uses mathematical convolution operations and shared weight kernels to capture spatial hierarchies and translation invariance.

### [[RNN|RNNs (Recurrent Neural Networks)]]

#concept #rnn #sequence-modeling

- Architectures designed to handle sequential and temporal data by maintaining hidden states across time steps.
- Enables context persistence, with advanced variants like LSTMs and GRUs addressing the vanishing gradient problem.

### [[Attention|Attention Mechanism]]

#concept #attention #deep-learning

- A mechanism that allows neural networks to dynamically focus on specific, relevant parts of input sequences.
- Computes alignment scores across inputs, dramatically improving network performance on long-range dependencies.

### [[Transformer|Transformer Architecture]]

#concept #transformer #nlp

- A deep learning architecture that relies entirely on self-attention mechanisms rather than recurrent or convolutional layers.
- Serves as the backbone for modern state-of-the-art models in natural language processing and computer vision.

### [[ViT|ViT (Vision Transformer)]]

#concept #vit #computer-vision #transformer

- An adaptation of the standard Transformer architecture applied directly to computer vision tasks.
- Processes images by splitting them into a sequence of non-overlapping patches treated similarly to word tokens.

### [[BERT|BERT]]

#concept #bert #nlp #language-model

- A large, pretrained bidirectional language model based on the Transformer encoder architecture.
- Pretrained on vast text corpora using masked language modeling, making it fine-tunable for various downstream NLP tasks.

### [[HPO|HPO (Hyperparameter Optimization)]]

#concept #hpo #automl #tuning

- The process of finding optimal configuration settings (e.g., learning rates, batch sizes, layer counts) for deep learning models.
- Encompasses manual tuning, black-box optimization algorithms (like Bayesian Optimization), and multi-fidelity speedup techniques.

### [[Autoencoder|Autoencoders]]

#concept #autoencoder #generative

- Unsupervised neural networks designed to compress input data into a lower-dimensional latent representation and reconstruct it.
- Composed of an encoder and a decoder, serving as a baseline for feature learning and generative modeling.

### [[VAE|VAEs (Variational Autoencoders)]]

#concept #vae #generative #probabilistic

- Generative models that extend standard autoencoders by mapping inputs to a continuous, probabilistic latent space.
- Uses variational inference to enable sampling and generation of realistic new data points.

### [[GAN|GANs (Generative Adversarial Networks)]]

#concept #gan #generative #adversarial

- Generative frameworks trained through a two-player game between a Generator and a Discriminator network.
- The Generator learns to produce realistic data to fool the Discriminator, while the Discriminator learns to distinguish real data from generated data.

### [[Diffusion Models|Diffusion Models]]

#concept #diffusion #generative

- State-of-the-art generative models that learn to synthesize data by reversing a gradual noise-addition process.
- Generates high-quality samples by iteratively removing noise from random Gaussian input.

### [[Bayesian Neural Networks|Bayesian Neural Networks]]

#concept #bayesian #uncertainty

- Probabilistic neural networks that place probability distributions over weights rather than fixed deterministic point estimates.
- Provides principled estimates of model uncertainty (epistemic uncertainty) alongside predictions.

### [[MCMC|MCMC (Markov Chain Monte Carlo)]]

#concept #mcmc #bayesian #sampling

- A class of sampling-based algorithms used for approximate Bayesian inference in deep learning.
- Generates samples from complex posterior probability distributions to quantify model uncertainty when exact inference is intractable.

### [[AutoML|AutoML]]

#concept #automl #optimization

- Automated Machine Learning techniques aimed at automating end-to-end machine learning pipelines.
- Reduces manual effort by automating model selection, hyperparameter tuning, and neural architecture design.

### [[NAS|NAS (Neural Architecture Search)]]

#concept #nas #automl #architecture

- An automated subfield of AutoML focused on automatically discovering optimal neural network architectures for specific tasks.    
- Uses search strategies like reinforcement learning, evolutionary algorithms, or gradient-based methods to design efficient models.

---

## [[Week 2: From Logistic Regression to MLPs]]
#week2 #deep-learning #MLP #logistic-regression #loss-functions

* **Loss Function**: Focuses on optimizing cross-entropy loss.
* **Model Transition**: Bridges standard machine learning models to the simplest deep learning model.
* **Architectural Properties**: Examines the core properties of Multi-Layer Perceptrons (MLPs).

---

## [[Week 3: Backpropagation]]
#week3 #backpropagation #gradients #optimization #calculus

* **Foundation**: Establishes the mathematical foundation for gradient-based optimization of loss functions.
* **Mechanics**: Breaks down the basics of backpropagation.
* **Implementation**: Details backpropagation formulated in matrix form.

---

## [[Week 4: Optimization for Deep Learning]]
#week4 #optimization #SGD #Adam #learning-rate #momentum

* **Landscape**: Addresses non-convex optimization challenges in deep learning.
* **Gradient Descent**: Covers Stochastic Gradient Descent (SGD).
* **Parameter Updates**: Explores learning rates and momentum.
* **Advanced Optimizers**: Studies adaptive gradient algorithms, including Adam.

---

## [[Week 5: Regularization]]
#week5 #regularization #dropout #data-augmentation #generalization

* **Parameter Sharing**: Utilizes parameter sharing to constrain model complexity.
* **Dropout**: Applies dropout techniques to prevent overfitting.
* **Data Augmentation**: Enhances training robustness through data augmentation.
* **Weight Penalties**: Applies a preference for small weights ($L_1$ / $L_2$ regularization).

---

## [[Week 6: Convolutional Neural Networks (CNNs)]]
#week6 #CNN #computer-vision #convolutions #spatial-data

* **Core Operations**: Studies mathematical convolutions and pooling mechanisms.
* **Spatial Context**: Incorporates spatial context and translation invariance into neural networks.

---

## [[Week 7: Recurrent Neural Networks (RNNs)]]
#week7 #RNN #LSTM #sequence-modeling #nlp #time-series

* **Sequence Handling**: Designed for processing sequential and temporal data.
* **Temporal Context**: Adds temporal context capabilities to neural networks.
* **Advanced Variants**: Explores Long Short-Term Memory (LSTM) networks and GRUs to handle vanishing gradients.

---

## [[Week 8: Attention & Transformers]]
#week8 #attention #transformers #BERT #ViT #nlp

* **Attention Mechanism**: Implements self-attention and multi-head attention to focus on specific parts of input data.
* **Transformer Architectures**: Explores the Transformer architecture and variations such as Vision Transformers (ViT).
* **Pretrained Models**: Investigates large, pretrained language models like BERT.

---

## [[Week 9: Practical Methodology]]
#week9 #methodology #troubleshooting #hyperparameters #self-supervised

* **Training Best Practices**: Covers practical methodology and troubleshooting to ensure networks train successfully.
* **Architectures & Learning**: Examines special network architectures and self-supervised learning techniques.
* **Tuning**: Studies manual hyperparameter optimization (HPO) in deep learning.

---

## [[Week 10: Auto-Encoders, VAEs, GANs, Diffusion Models]]
#week10 #generative-models #autoencoders #VAE #GAN #diffusion

* **Variational Autoencoders**: Covers traditional autoencoders and probabilistic Variational Autoencoders (VAEs).
* **GANs**: Explores Generative Adversarial Networks and adversarial training dynamics.
* **Diffusion Models**: Introduces modern score-based and diffusion models.

---

## [[Week 11: Uncertainty in Deep Learning]]
#week11 #uncertainty #bayesian-dl #variational-inference #mcmc

* **Bayesian Networks**: Introduces Bayesian neural networks for probabilistic modeling.
* **Approximate Inference**: Covers approximate Bayesian inference methods, including variational inference, MCMC, and prior-data fitted networks.
* **Uncertainty Estimates**: Explores non-Bayesian methods for estimating epistemic and aleatoric uncertainty.

---

## [[Week 12: AutoML for Deep Learning]]
#week12 #AutoML #HPO #NAS #optimization

* **Hyperparameter Optimization**: Focuses on automated HPO strategies in deep learning.
* **Optimization Methods**: Explores black-box optimization methods (e.g., Bayesian Optimization) for HPO.
* **Efficiency**: Discusses multi-fidelity and speedup techniques for HPO.
* **Architecture Search**: Studies Neural Architecture Search (NAS).