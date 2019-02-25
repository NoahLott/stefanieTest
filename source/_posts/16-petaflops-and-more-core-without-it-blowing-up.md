---
title: 16 Petaflops and More Core Without It Blowing Up 
date: 2010-8-13 13:20:00
category: programming
---

![](/images/4.jpg)

## With 16 petaflops and 1.6M cores, DOE supercomputer is world's fastest

Every six months, Earth's most important supercomputers have a huge race to see that may lay claim to getting the world's most effective high-performance computing cluster.

In the most recent Top 500 Supercomputer Sites list unveiled Monday morning hours, a newly assembled cluster constructed with IBM hardware at the Department of Energy's Lawrence Livermore National Laboratory (LLNL) takes the most notable prize. Its speed? An impressive 16.32 petaflops, or 16 thousand trillion calculations per second. With 96 racks, 98,304 compute nodes, 1.6 million cores, and 1.6 petabytes of memory across 4,500 square feet, the IBM Blue Gene/Q system installed at LLNL overtakes the 10-petaflop, 705,000-core computer in Japan's RIKEN Advanced Institute for Computational Research.

<!-- more -->

The Japanese computer have been world's quickest twice in a row. Before that, the most notable spot happened by a Chinese program. The DOE pc, named "Sequoia", was sent to LLNL between January and April. It is the first US system to be ranked #1 since November 2009.

To access 16 petaflops, Sequoia ran the Linpack benchmark for 23 hours with out a single main failing, LLNL division head Kim Cupps told Ars Friday in advance of the list's release. The system is capable of hitting a lot more than 20 petaflops-during the checks it ran at 81 percent proficiency.

For a equipment with 1.6 million cores to perform for over 23 hours six weeks after the keep going rack arrived on our floor is nothing short of astounding, she said.

The cluster is incredibly efficient for one so large, with 7,890 kilowatts of power, in comparison to 12,659 kilowatts for the second-best K Computer. It's generally cooled by drinking water running through small copper pipes encircling the node cards. Each cards retains 32 chips, with each chip having 16 cores.

The entire cluster is Linux-based. Compute Node Linux is run on almost 98,000 nodes, and Red Hat Business Linux runs on 768 I/O nodes which hook up to the file program, Cupps said.

To start out, the cluster is about a comparatively open network, allowing various scientists to use it. But after IBM's debugging method is over around February 2013, the cluster will be transferred to a categorized network that isn't available to academics or outside corporations. At that point, it'll be devoted almost specifically to simulations targeted at extending the lifespan of nuclear weapons.

The sort of science we must carry out is lifetime extension programs for nuclear weapons, Cupps said. That will require suites of codes jogging. What we're in a position to do upon this machine is to perform many calculations simultaneously on the device. You can turn various knobs in a brief time frame.

Blue Gene/Q runs on the PowerPC architecture that includes components support for transactional memory space, allowing more comprehensive real-world assessment of technology.

In November 2011's Top 500 list, three of the top five clusters employed NVIDIA GPUs (graphics processing units) in combo with CPUs to accomplish very high speeds. This time around, just one of the very best five integrates GPUs, although the entire number in the most notable 500 integrating GPUs or identical accelerators rose from 39 to 58.

The use of GPUs in supercomputing tends to be experimental up to now, said Dave Turek, IBM vice president of high performance computing. The aim of this is to accomplish real technology, he said. GPUs are a bit more difficult to method for, he said.

While the majority of Top 500 computers use Ethernet or Infiniband as their primary interconnects, Sequoia uses IBM's proprietary 5D Torus. It's an optical network that delivers 40 Gbps throughput to IBM's Blue Gene/Q clusters. I/O nodes are linked to the file program via Infiniband and the administration network uses Ethernet, Cupps stated.

IBM leads the most notable 500 list with 213 systems, before HP's 138. Practically 80 percent-372 of the 500 systems-use Intel processors, accompanied by 63 employing AMD Operton and 58 using IBM Power.

Three DOE systems happen to be in the very best 10. The others hail from Japan, Germany, China, Italy, and France. All 10 have effectiveness of at least at least 1.27 petaflops.

Petascale computers have become relatively commonplace because the IBM Roadrunner program in Los Alamos National Laboratory was first the first to hit a petaflop in 2008. Actually, each of the top 20 devices on the brand new list hit at least a petaflop. Exascale, which would be 1,000 times faster, is the next big breakthrough for the IBMs, HPs, and Crays of the universe to aspire to.

But a big progress in price-performance is necessary. Today's technology could level up a lot higher-it merely wouldn't be practical. Supercomputers are naturally pricey (a lot more expensive than the latest MacBook Pro). The K Computer in Japan, for instance, cost a lot more than $1 billion to build and $10 million to operate each year. Livermore informed us it spent approximately $250 million on Sequoia.

We're able to get another order of magnitude with this technology if somebody would compose a check, Turek stated. But no one would want to write that check.”

### How to use a good million-core supercomputer-without it blowing up in that person
_Throwing more cores by science: risky for high reward._

At the Lawrence Livermore National Laboratory in California, a supercomputer named "Sequoia" puts almost every other computer on earth to shame. With 1.6 million processor cores (16 per CPU) across 96 racks, Sequoia can perform 16 thousand trillion calculations per second, or 16.32 petaflops.

Who would demand such horsepower? The IBM Blue Gene/Q-based program was designed for the Section of Strength for simulations designed to lengthen the lifespan of nuclear weapons. But also for a limited time, the device is being distributed around outside researchers to execute a variety of tests, a couple of hours at a time.

One of the first to have good thing about this opportunity was Stanford University's Center for Turbulence Research-and it wasn't hesitant about seeing what this equipment is really capable of. For three hours on Tuesday of last week, researchers from the center remotely logged in to Sequoia to perform a computational liquid dynamics (CFD) simulation on a million cores at once-1,048,576 cores, to be exact.

It's part of a good project to test noise made by supersonic jet engines and support design engines that happen to be a bit quieter. The work is sponsored partly by the united states Navy, which is concerned about "hearing damage that sailors on aircraft carrier decks come across as a result of jet noise," Study Associate Joseph Nichols of the guts for Turbulence Exploration told Ars.

Using huge supercomputers to solve complex scientific problems is usually in no way unique nowadays. Larger amounts of cores don't necessarily translate to the most effective speed, either, as a result of dissimilarities between processors and the styles of supercomputers. The million-core run is normally intriguing, but it additionally poses extreme issues in trying to work with all those cores simultaneously without things going incorrect.

Believe it or not, three several hours with a million cores wasn't enough to generate a real dent in the plane noise project. Despite planning work aimed at reducing out bottlenecks, it was just enough time to make certain the code ran properly also to get yourself a sense of the possibilities that million-core PCs can offer.

"This is really showing what we are able to do later on," Nichols said. "The simulations take some time to boot up and go through initialization. We performed tune the I/O for the Blue Gene architecture, but it is nonetheless slower than the blindingly quickly computation and interaction speeds. Depending on how much info gets written, the I/O can truly add an extra chunk of period to the overhead."

The problems are all over the area, including "How can you write into one file from a million processors that are trying to step on one another?" Nichols said. "That was an interesting thing. It kind of depended on the interconnect, too. Only a number of the processors happen to be linked to the disk, and that means you need to rearrange data to achieve the right performance."

## Extra cores, or better cores?

Sequoia was named the world's quickest supercomputer in June 2012. Sequoia soon after fell to second place behind a 17.59-petaflop system at the Oak Ridge Countrywide Laboratory, but it is still the only system at the top 500 supercomputers list with a million or even more cores.

Of course, choosing "more cores" isn't necessarily the easiest method to tackle a supercomputing problem. That Oak Ridge pc, named Titan, hit 17.59 petaflops using "only" 560,640 cores. The Titan program was developed by the supercomputer producer Cray, and it uses Nvidia design processing units furthermore to classic CPUs to get dramatic increases in quickness.

There are pros and cons to different approaches. Dave Turek, IBM vice president of powerful computing, told Ars this past year that GPUs happen to be more difficult to program for, and the GPU-significantly less Sequoia is for "real science." Titan, it should be noted, does plenty of real technology, tackling problems linked to climate transformation, astrophysics, and more. With both CPUs and GPUs in something, Titan's CPUs guide the simulations but hand off do the job to the GPUs, which can handle a lot more calculations at once despite using only slightly more electricity.

Throwing more cores at a problem doesn't invariably result in performance gains. Code needs to be carefully well prepared to take into account the bottlenecks that come up when information is transmitted from one core to another (unless the request is so parallel that each core could work on split calculations without ever talking to each other).

Previously, Nichols' biggest calculation was performed for approximately 100 hours on 131,072 cores on a Blue Gene/P system. The same calculation could possibly be done on a million Sequoia cores in about 8 to 12 time, he said.

Besides accelerating lengthy calculations, even more cores and faster supercomputers will let scientists tackle a lot more complicated problems.

"Having more cores, either you reduce the time to choice or you solve more technical problems, problems involving circulation that involve, say, chemical substance reactions, combustion," stated Parviz Moin, director of the guts for Turbulence Research. "These are grand challenge problems that involve many, many more equations and lots of work that will be distributed among the processors."

## Getting code geared up for the million-core run
Nichols and team use the Navier-Stokes equations and codenamed CharLES for the plane noise simulations (LES means large eddy simulation). They're employing the same code for different projects to research scram jets (supersonic combustion ramjets), which could travel at 10 situations the speed of audio.

We've written before about large supercomputing runs-for example, one using 50,000 cores on the Amazon Elastic Compute Cloud. That one was "embarrassingly parallel," where the calculations are all independent of each other. Which means the swiftness of the interconnect, the connections between each processing key, didn't really matter.

The million-core run was not only substantially bigger, it was more complicated. "It is parallel but there is connection [between processors] included," Moin explained. "Each core is not independent."

As we wrote in August 2011, Blue Gene/Q uses "transactional memory space" to solve many of the issues that help to make highly scalable parallel development so hard. But prep function by humans is still required.

Nichols caused the Lawrence Livermore individuals to optimize the code for Sequoia, avoiding slowdowns found in I/O efficiency and minimizing the communication needed in each step.

Sequoia uses IBM's proprietary 5-dimensional Torus interconnect. Nichols explains:

"Each compute node is linked to 10 of its nearest neighbours. There will be five measurements and it goes forwards and backward along each dimension. That's 5x2 and you get 10 connections with these optical links."

"You can communicate with processors that are even more away, but it includes a bigger latency. Latency for the nearest neighbour is normally 80 nanoseconds, which is very amazing. The calculation uses the interconnect so that communication overhead was very little actually at a million processors."

Performance scaled almost in a one-to-1 ratio with the increase in cores, with 83 percent efficiency. Nichols clarifies that since heading from 131,000 cores to at least one 1 million multiplies the amount of cores by 8, one would want a speed-up of 8 as well.

The true speed-up was 6.6, which is "83 percent of the perfect speed-up we would like to see. It signifies that as we're adding considerably more cores the code gets faster and faster, also at the million level. This is amazing for a CFD simulation, because in CFD simulations each one of these sub-domains features to talk to its neighbours at each time step to talk about wave information."

Modelling plane engines is sophisticated, as Stanford notes in a description of the project: "These complex simulations let researchers to peer inside and measure processes happening within the tough exhaust environment that's otherwise inaccessible to experimental devices."

The simulations allow Stanford to test how adjustments to the engine nozzle and chevrons impact noise. With supercomputers these simulations can be carried out without building physical designs or tests in wind tunnels.

"That's a really complicated difficulty because you possess shock waves found in engines which are incredibly thin scales when compared to amount of the combustion," Nichols said. "And then you have combustion as well as turbulence in everything. The theory is that people can predict the behaviour. If given enough resolution we can predict what will happen with various kinds of designs."

The analysis of scram jets and the conditions under which they might fail involves similar complexity. "NASA is very much enthusiastic about such vehicles for access to space," Moin stated. "These will be air-breathing vehicles instead of rockets. They take their personal oxygen to orbit; they're heavier due to that. They have to carry liquid oxygen."

For now, the researchers must continue this work with paltry sub-million-main supercomputers. But most likely it won't be a long time before supercomputers as powerful as Sequoia will be the standard for such research.

As a high school student in 1994, Nichols attended a summer season course at Lawrence Livermore and done the Cray Y-MP. At that time, it was among the faster machines on earth.

"Now Sequoia is 10 million times stronger than that equipment," Nichols said. "This is presenting us a glimpse into the future, that it is really possible to run on a million cores."
