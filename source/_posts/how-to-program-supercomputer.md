---
title: How To Program Supercomputer
date: 2014-4-06 09:30:00
category: programming
---

![](/images/3.jpg)

We felt that it had been essential to write a reserve reintroducing programming tactics that should be employed by software developers targeting the existing and future generation supercomputers. As the techniques have been around for a long time, many of today's developers are not aware of them. Let us explain.

The supercomputer is a shifting target for application programmers since its inception in the form of Seymour Cray's CDC 6600 in the first 1970s, forcing developers to adjust to new approaches together with the ever-changing hardware and software systems. This need of programmer adaptation is especially conspicuous in neuro-scientific high-effectiveness processing (HPC), where developers typically optimize for the prospective node architecture to squeeze out every previous ounce of available effectiveness. This continued through the CDC7600 and the vector-rich systems: Cray 1, Cray XMP, YMP, and C90.

Then, the "Attack of the killer micros" in the 1990s threw everything right into a tizzy. With raising node counts, request developers possessed to consider PVM, and MPI, within their quest to parallelize their applications across the multitude of nodes comprising commodity off-the-shelf (COTS) chips without the vector instructions. As can be seen in Figure 1, the COTS chips acquired more rapidly as their clock routine time decreased between 1995 and 2010. Software developers no more had to be worried about the node architecture.

<!-- more -->

With the advent of AVX256, AVX512, SVE, and GPUs in the last five years, vectors have begun to come back. More recently, many-core devices like Intel's Knight's Landing (KNL) in addition to fastened accelerators such as for example Nvidia's type of GPUs required a re-examination of the application form to progress performance from the brand new, more-powerful nodes. Because the application could not really always be vectorized and parallelized instantly by the compiler, the application form developer had to do something.

That something ranged from writing important kernels in particular programming models like CUDA for the Nvidia GPUs, to using compiler directives to greatly help the compiler translate the input user-level code into low-level vectorized code for the processors. In that case there was the issue of using those cores on the node / making a large number of threads for the GPU. Because jogging MPI across all the cores on and off the nodes proved helpful pretty much, the developers for the original multi core systems didn't should get into parallelizing with shared recollection threads. Even so, threading on Nvidia accelerators was definitely required. OpenACC and OpenMP 4.5 were developed for a performance-portable solution for threading and vectorization for the GPU.

Another revelation in different architectures is that memory space hierarchies have become more complex, especially if an application has a large memory space footprint. Knight's Landing, together with nodes with fastened GPU accelerators, possess two levels of recollection which introduces new issues that must be tackled by programmers. Shape 2 shows the dissimilarities between the recollection hierarchies of KNL and the hosted GPU. If an application fits in to the high-speed memory, then it'll enjoy excellent memory performance. Nevertheless, if the application form requires more memory, the info set must be managed to flow between the two within an efficient and timely approach.

The last four to five years have already been a culture shock to those creators who insisted on productivity over performance. They are actually confronted with the serious task of properly utilizing these new strong nodes. If indeed they continue with all-MPI codes and do not perform the required conversion to multi-level parallel code (through vectorization and threading), their performance will be a function of merely the amount of cores on the node and the clock cycle. While the amount of cores on the node is certainly going up gradually, the clock rate of those cores is going down, leading to poor returns on latest hardware investments without software optimization.

Our book Development for Hybrid Multi / Manycore MPP Devices discusses the architecture of the brand new nodes and programming techniques application developers may utilize to glean more performance. It'll be extremely useful for all those developers who are now confronted with the significant challenge of getting increased effectiveness from the vector capacity for the node together with improved scaling over the increased amount of cores or threading for the GPU. The reserve also looks at the memory space hierarchy of the KNL and discusses many approaches for managing the data. Finally, the reserve looks to the near future, which is extra of the same in lots of ways: extra cores with wider vectors and also more technical memory hierarchies.

If you'll be at SC17 in Denver, be a part of us at Cray booth #625 for a good meet-the-author session at 2 p.m. on Tuesday, November 14. You can purchase a reserve at the CRC Press booth #811 for a 30% discount through the show.

## Your Own Supercomputer in the Azure Cloud

Your organization depends on technology for a competitive advantage. You will need fast, reliable effectiveness. But high-performance computing can be a large expense, and challenging to manage in your IT infrastructure.

Cray and Microsoft produce it easy - and you get Cray supercomputing found in the Microsoft Azure cloud.
This convergence of supercomputing capabilities and the ease of cloud management enables disruptive innovation for new types of companies. It alleviates the operations burden and reduces barriers of access to HPC.

Supercomputing is no more out of grab smaller enterprises and corporations that can't or don't want to maintain their own datacenters.

Intersect360 analyst Addison Snell says, the mixture of Cray's systems and support capability, combined with access to Azure's robust services, can go well beyond traditional IT resources and unlock possibilities that have been previously impossible because of scaling and performance limitations.

### Topics include:

_Market dynamics_ - vertical industry distribution of HPC usage
_Cray found in Azure_ - differentiated capabilities, managing Cray in Azure, and expanding high-performance workloads
_Research analysis_ - searching toward AI, big data and HPC
He as well examines two industry tendencies: (1) big data and analytics, which inspire businesses to unlock the competitive positive aspects hiding unseen within their data; and (2) artificial cleverness (AI), fuelled by developments in equipment learning algorithms created by leading hyper scale processing companies such as for example Microsoft, Google, Facebook, and others.

Just as big info swept through the IT landscape, many companies are actually launching investigations of how AI might help them automate techniques, improve responsiveness, and increase competitiveness.

Download the full paper, "Azure Provides Clean On-Ramp to Cray Processing", to find out more on today's HPC and cloud landscape, and to find out how Cray in Azure could work for your enterprise.
