---
title: "High-Performance Domain-Specific Compilation without Domain-Specific Compilers"
collection: publications
type: "PhD Thesis"
date: 2020-08-24
authors: "<b>Bastian Hagedorn</b>"
venue: "PhD Thesis, University of Münster"
paperurl: '/files/publications/2020/thesis.pdf'
projects: ['Thesis']
---

<a href="/files/publications/2020/thesis.pdf" style="margin-right:1em; text-decoration: none;"><span class="fa-stack fa-1x"><i class="fa fa-trophy fa-2x"></i></span>Awarded with the highest possible grade: Summa cum Laude</a>

Developing efficient software for scientific applications with high computing power demands, like physics simulations or deep learning, becomes increasingly difficult due to the ever-changing hardware landscape consisting of multi-core CPUs, many-core GPUs, and domain-specific accelerators. Domain-specific compilers pose a viable solution to this problem. They provide convenient high-level programming abstractions in the form of Domain-Specific Languages ( DSL s) while automatically performing the heavy lifting of generating high-performance code for the target architecture. However, this places the burden of high-performance code generation solely on the developers of the domain-specific compiler. Typically, there is little to no reuse between domain-specific compilers: A domain-specific compiler is specific to one domain and is generally not reusable for generating code for another domain. Therefore, developing a domain-specific compiler, especially its Intermediate Representation ( IR ) and optimization passes, is difficult because of the need to start from scratch for every new compiler. 

This thesis presents a novel approach to achieving the benefits of high-performance domain-specific compilation without the need to develop domain-specific compilers. The key idea of our approach is decomposing both domain-specific computations and their optimizations into a small set of generic building blocks. Using only those building blocks, we develop a domain-agnostic compilation approach to generating high-performance code. This approach allows us to achieve the benefits of domain-specific compilation by simply expressing both domain-specific computations and their
optimizations as compositions of generic building blocks.

The thesis starts with a case study highlighting the benefits and potential of domain-specific compilation and demonstrates the drawbacks of developing a domain-specific compiler from scratch. Specifically, we show why domain-specific compilation is far superior to using high-performance libraries or manually developing high-performance implementations. At the same time, we highlight the limitations of representing computations in a domain-specific compiler’s IR that is optimized using domain-specific optimization strategies. We then show how to decompose both computations and optimizations into generic building blocks, and discuss how to re-compose those to express domain-specific computations and optimizations. Finally, we show that our approach achieves competitive performance to state-of-the-art domain-specific compilers without having their drawbacks.
