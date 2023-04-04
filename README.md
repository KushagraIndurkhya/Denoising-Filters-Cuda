Title: Efficient Implementation of Nonlinear,edge-preserving denoising Filters on CUDA GPUs

1. Introduction
   1. Need for denoising, Origin of noise
   1. Importance of denoising
   1. Need for time
   1. Need for edge perseverance
   1. Leveraging GPU
1. Literature Review
   1. GPU architecture
   1. Nvidia docs
   1. Choosing algorithm
   1. Why bilateral
   1. Current Works
   1. NL Means + Bilateral
   1. Adaptive Bilateral Filter
   1. Metrics used for results
   1. Other techniques looked at Guided filter, iterative bilateral, and anisotropic diffusion: Ask sir if I should add
1. Work done
   1. Bilateral Filter
      1. CPU Implementation: Sequential
      1. CPU Implementation: Parallel
      1. GPU Implementation: Naive
      1. GPU Implementation: Optimization by caching spatial kernel
         1. Global
         1. Shared
         1. Const memory
      1. GPU Implementation: Optimization by using Shared Memory Implementation
    2. NL Means Filter
      1. CPU Implementation: Sequential
      1. CPU Implementation: Parallel
      1. GPU Implementation: Naive
      1. GPU Implementation: Optimization by caching spatial kernel
         1. Shared
         1. Const memory
      1. GPU Implementation: Texture Memory, Tiling
    3. Adaptive Bilateral Filter
      1. GPU Implementation: Naive
      1. GPU Implementation: Optimization by caching spatial kernel
         1. Shared
         1. Const memory
      1. GPU Implementation: Shared Memory Implementation

4. Results and Discussions

    1. Experiments
      1. a (i,ii,iii,iv,v)
         1. Time vs Vary sigma s,sigma r
         1. PSNR vs Vary sigma s,sigma r
         1. Vary Noise
      1. a.v vs b.iii vs c.iii
          1. Time vs Vary sigma s,sigma r
          1. PSNR vs Vary sigma s,sigma r
          1. Vary Noise
    2. Result Study
5. Summary and conclusions
    1. Summary
    1. Results
    1. Future Scope
6. References
