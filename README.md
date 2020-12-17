# Face-Aging-using-GANS

In particular, our contributions are as following:
1. Age-cGAN (Age Conditional Generative Adversarial Network), the first GAN to generate high quality synthetic images within required age categories.
2. We propose a novel latent vector optimization approach which allows Age-cGAN to reconstruct an input face image preserving the original person’s identity.

Once Age-cGAN is trained, the face aging is done in two steps:
1. Given an input face image x of age y0, find an optimal latent vector z∗ which allows to generate a reconstructed face x_bar = G(z∗, y0) as close as possible to the initial one.
2. Given the target age y_target, generate the resulting face image xtarget = G(z∗, y_target) by simply switching the age at the input of the generator.
