# stable_diffusion_amani

## Best way to learn is be doing

Latent diffusion models (stable diffusion) from scratch in PyTorch. 

Classifier-Free Guidance
Text-to-image
Image-to-image
inpainting

what is a generative model?

- a generative model learns a probability distribution of the data set such that we can then sampel from the distribution to create new instances of data. 

- model the data as a probability distribution network then learns the parameters; that can then be sampled across to generate new data.

fixed process to add noise -- reverse process neural network.

joint distribution of parameterized model is called the reverse process, and is defined as a Markov chain with learned guassian transitions starting at p(xT) which is just a guassian distribution in I dimensional space.

the approximate posteriror is called the forward process or diffusion process, which fixd to a markov chain that adds gaussian noise to the data. ( Markov chians as each successive step is dependent on the previous step )

image + amount of noise + prompt e.g. cat ---> model predicts amount of noise added.

classifier-free guidance, -> sometimes you give it a prompt sometime you dont

CLIP ( text encoder ) only

compress image : Latent diffusion model -> autoencoder: input -> encoder -> x -> decoder -> reconstructed input... issue is there is no semantic relation. hence Variational Autoencoder.

