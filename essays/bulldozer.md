---
layout: essay
type: essay
title: AMD Bulldozer
published: false
# All dates must be YYYY-MM-DD format!
date: 2019-11-27
labels:
  - Computer Architecture
  - AMD
---
## Introduction 
From the early breakthroughs in computer design, the processor has continually been improved upon due to the efficient use of transistors, while being able to scale them down. Through scaling them down, much more transistors can be implemented onto a single chip, improving the speed and performance, ultimately resulting in a faster computational and processing speed for the computer. In order to cater to all individuals, different classes of processors were created with varying speeds and computational power based on the price consumers are willing to pay for them. Advanced Micro Devices, a processor company (AMD) has been a clear competitor for other companies such as Intel, in creating processors. 

Many different processors have been created following Moore’s law to create the best performance processor while conserving price and cost to create using innovative pipelining methods. AMD has been in the technology industry for the past 50 years as one of the competitors for Intel, where both are able to create semiconductor technology to be used in processors for higher computing and application needs. AMD has continually been able to innovate new microarchitectures throughout the years that work towards having better performance in a way that is not only efficient but reduces fabrication cost that could cascade down to an overall reasonable product for typical consumers [3]. 

Throughout time, these processor companies have experimented between the incorporation of a different number of cores ranging from a single core up to an octa-core. Continually in the computer processor industry, Intel and AMD gain knowledge and experience to create new innovative designs to improve performance in a competitive setting against each other. Along with the experimentation on the number of cores, the operating frequencies were also varied, to create faster-operating processors ultimately reaching a speed of up to 5GHz back in the year 2011 [5]. The speed of the designs has continually increased, which continually pushes the boundaries. 

In the following write up, each member contributed to equal number of pages each, through the help of collaboration. Each member contributed to research and analysis, along with proofreading the overall report. The following write up discusses the technology of processors in Section 2, processor architecture in Section 3, pipeline structure in Section 4, along with memory in Section 5. The overall write up is concluded in Section 6 summarizing the processor, along with concluding statements. 


## Technology

Through the process of designing and creating cheaper end processors that could compete with current processors at the time, Advanced Micro Devices created the AMD FX processor. In application, the processor was designed to operate at higher frequencies up to a value of 5kHz. With a cheap and decent design, many of these processor chips were able to be commonly found in entertainment systems like the Xbox One and also used in Radeon graphics cards. For this type of processor, a discrete graphics card is needed to be able to use it in a system, as normal with any other typical processor. Using the common Complementary Metal-Oxide Semiconductors (CMOS), with 32nm Silicon-on-Insulator (SOI) technology, the main processors were created ranging from a minimum quad-core, up to a maximum octa-core design. Despite the cheaper design with decent performance, the design was anticipated to outperform the previous generation by a large factor. When tested, however, the performance of the processor did not meet the overall expectations of which the designers had hoped for. Even though the processor used decent pipeline processes compared to normal [6], it was able to perform at temperatures of up to 70.5℃ [1]. Using the advanced technological fabrication processes, this cheaper ended processor was able to be manufactured with ease with the mindset that it will be able to perform at a speed more than adequate enough for the average consumer at a price that is fair and not overpriced during the time. In order to expand on the design, there were many different variations on the AMD FX processor made to tackle the constraints on the frequency and pipeline structure [2]. These chips can be seen on the wafer in Fig. 2 below. The lithography processes continually grow, where better fabrication processes are being created which make it easier to create different designs that will not cost a fortune. Through making multiple processors that are both affordable and efficient, the industry can build upon different designs to cater to consumer needs. The AMD FX processor is seen below in Fig. 1. 
 
{% include image.html url="/images/bulldozer/fig1-amd-fx-processor.png" description="Fig. 1: AMD FX Processor [1]" %}

As with all processors, there is a significant amount of power dissipation through use, which also results in the generation of heat. In order to tackle on the heat problems and reduce the temperature of the processor, a common heat sink is used to cool down the system and allow for continual use under harsh conditions. With the use of the heat sink, the processors are also able to run for longer periods of time without severe damage. Within the Bulldozer architecture, testing done on the processor showed that the main design was not able to be successfully implemented as hoped, showing that there is a large amount of unfavored power consumption [8]. Unfortunately, there was some misleading, saying that the processor was an octa-core when it was a quad-core due to the module count in the overall design [2]. Aside from the problems faced, the processor is still implemented in many gaming systems due to the low price. 


{% include image.html url="/images/bulldozer/fig2-processors-on-silicon-wafer.png" description="Fig. 2: Processors on Silicon Wafer [3]" %}



## Architecture

At the time, the AMD FX was the first natively claimed octa-core processor amongst all competitors. With the creation of the AMD FX processor, a new Bulldozer architecture was introduced back in 2011 [9]. This design was the successor to the previous Piledriver architecture. Such a design was created from scratch, under the codename Zambezi [4]. At the time, the focus was to compete against the Sandy-Bridge/Ivy-Bridge architecture from their competitors at Intel. The Bulldozer architecture was created with the mindset that the processor would be able to be overclocked in order to speed up the instruction execution speeds, ultimately resulting in an overall increased speed performance. The design was devised to also increase the CPU to operate at higher frequencies while being able to maintain the same amount of instructions per cycle at 6-cores from the previous predecessors. In the Bulldozer architecture, there are common stages seen in all processors such as a fetch/decode stage, along with a form of pipeline [7]. Along with such, there are multiple schedulers to take in the instructions and memory caches for storage [5]. The effect of combining the schedules allowed for the chance to scale down the CPU. This design was used in order to conserve space in an attempt to not only save chip area but also scale down designs for better large-scale fabrication. Specifically, in the Bulldozer architecture, there are four modules that can have x86-64 instruction sets. These types of instructions are able to deal with larger amounts of data. These two cores in each module are separated for splitting up computation, each having their own separate caches. Initially, the known date is shared between the two cores at the top of the stage and gets pushed through the system. Towards the end of the computation, the processor combines the instructions executed into a shared cache at the bottom of the processor at the end of the stage. This design is considered very abstract and radical, with the intention of gaining better power efficiency as well as reduce the size of the chip overall. 
Most programs and games at the time were not able to make use of the full octa-core design from the Bulldozer architecture, thus resulting in the disparity in performance between that seen in the other competitors. After releasing the design back in 2011, AMD quickly set to resolve the shortcomings of the Bulldozer architecture by building upon the previous working generation. The Bulldozer architecture was then later succeeded by a redesigned Piledriver in the year 2012 [4]. A piece of the Bulldozer architecture can be seen below in Fig. 3 showing the stages on the processor, involving the fetch and decode stage, branching off into separate schedulers, then to the pipeline and back together in the bottom shared cache. 
 

{% include image.html url="/images/bulldozer/fig3-bulldozer-architecture.png" description="Fig. 3: Bulldozer Architecture [2]" %}


## Pipeline Structure
   
With the new Bulldozer design, there are 4 modules within the processor, each with 4 separate pipeline structures in each core. A close-up structure of a single module is seen in Fig.3. When quantifying the performance of this processor in comparison to other processors that operate at around the same frequency, a single core speed was tested to see how it ranked compared to others seen in Fig. 4. The single core was subjected to its branch prediction capabilities, where the scores reflected the accuracy of predicting branches correctly along with misprediction penalties by subjecting the processor to operate a specific program known as the “Queens Problem”. As seen in the benchmark test, the AMD FX is seen to have the lowest score, negatively impacting the view of the processor at the initial launch, causing a loss in revenue for the company. Low scores were seen across all similar performance tests done, causing AMD to abandon most of their interesting in the Bulldozer pipeline and revert to the previous design. 

A critical factor in why the performance ratings are not as impressive is due to design testing where the turbo core feature was not able to work well with the operating system at the time [7]. Due to the very different design compared to those from other processors at the time, the pipeline intended was not able to be clearly carried out [8]. With the current version of Windows at the time, the operating system was not able to differentiate which cores needed to be turned off. Through the pipeline design, there were some cores that would need to be shut off to help with the power consumption, however, was disrupted and ineffective due to the inconsistent pairing between the processor and operating system itself. Despite the two cores sharing a schedule, the operating system sees 8 individual cores, thus making it difficult for the system to understand the way in which resources are allocated within the Bulldozer architecture, scaling down to reducing the impact of the two sets of pipelines in the two cores. As time went on, the next generation updates on operating systems were created with the introduction of Windows 8, the full capabilities of the AMD FX pipeline were then realized [8]. Once the operating system was able to fully make use and understand the pipeline effect of the AMD FX, being able to understand when to turn off a certain core to optimize the power consumption. The processor truly was able to allow for great performance at a reasonable price. With the power consumption limitation along with the limitation on the number of instructions able to be handled, the pipeline was restricting the overall potential of the processor, resulting in a loss of performance speed. In total, the four-way pipeline was still able to dedicate a single core to execute a specific instruction while another core was in sleep mode. 
Upon the initial launch of the processor, the overclocking abilities were very high, seen in 2011 where the AMD FX was able to surpass the previous record for an overclocked speed of 8.309GHz at a new value of 8.429GHz [10]. The unorthodox pipeline design allowed for faster overclock speeds to be obtained. With the ultimate shortcoming of the processor due to many unfortunate mishaps, the pipeline was significantly slower compared to the others of the same price and operation speed, leading to a large loss in revenue for AMD. 
 
{% include image.html url="/images/bulldozer/fig4-single-core-queens-benchmark-test.png" description="Fig. 4: Single Core Queens Benchmark Test [8]" %}


## Memory

As part of the redesigned dual-core modules, the Bulldozer architecture consists of three levels of caches, allowing easy access of data for the CPU. The first level L1 cache resides within each core and is used by the corresponding four pipelines [8]. This level of cache requires the fastest rates for reading and writing, thus it trades size for speed as its capacity ranges from 192KB to 384KB depending on which model of processor. However, the L2 and L3 caches take a different approach by holding a heftier amount of storage. The second level L2 cache holds a capacity of 4MB to 8MB depending on which model and is shared amongst two conjoined modules for more efficient data access [8]. This cache is further supplemented by a third level L3 cache that is shared amongst all four modules that make up the processor and holds a capacity of 8MB. The tradeoff for larger cache sizes is apparent in the added time between when a memory request is initiated and when the memory is retrieved by the processor, or what is otherwise known as cache latency. This loss becomes even more dramatic when compared to that of the competition as shown in Fig. 5. 
     
{% include image.html url="/images/bulldozer/fig5-cache-latency-comparison-test.png" description="Fig. 5: Cache Latency Comparison Test [8]" %}

We see here that the L3 cache of Bulldozer architecture performs rather poorly at 16.7 ns with Turbo on, and at 19.2 ns with Turbo off. When compared to its rival, Sandy Bridge, the competition triumphs with cache latency of less than half that of Bulldozer architecture with Turbo on or off. In fact, the AMD FX is outperformed by its own predecessor, the Phenom II. These drastic variances that exist in the comparison of latency between Bulldozer and its competitors contribute to lacking performance and speed that is unfortunately inherent of this microarchitecture. 

As for system memory, this processor supports DDR3 memory up to a frequency of 1.866MHz. The latency situation for the main memory suffers the same fate to that of the L3 cache. That is, despite the Bulldozer’s superior clock speed and scaled down design, it is beat ever so slightly by Intel’s Sandy Bridge and AMD’s own Piledriver architecture. With Turbo turned on, the clock speed drives to a reported 3.9GHz and latency is reduced by 5.7ns, beating out the Phenom II X4, but still falling short of the competition. Fig.6 graphically depicts the latencies of these architectures. 
 
 
{% include image.html url="/images/bulldozer/fig6-memory-latency-comparison-test.png" description="Fig. 6: Memory Latency Comparison Test [8]" %}




Overall, the vision behind this three-level, shared hierarchical approach to caching was in hopes to create more efficient data access while also allowing the processor design to be scaled down. In the new Bulldozer design, AMD decided to use three levels of caches that are shared amongst each module and are of a larger size than its predecessors. As a result, these processors lack the speed that encompasses a smaller cache capacity. It is made clear that the AMD FX was intended for use with Turbo on to maximize its potential speeds to catch up to its competition, but even so, this processor still barely beats its own predecessors and is leagues away from the speed of Sandy Bridge.


## Conclusion

The AMD FX processor represents an ambitious attempt for a company to make a revolutionary breakthrough in processor technology. The exclusive Bulldozer architecture was completely redesigned and, using the x86 instruction set, combining schedules together into modules. Within each module are the Fetch and Decode stages that are shared by two cores, with each core containing 4 pipelines. While this technology succeeds in multithreading pipelines, speeds stall when performing single threaded instructions. Additionally, cache leveling is done in three levels with an L1 cache for each core, L2 cache shared by each module, and L3 cache shared encompassing all modules. This allowed the overall design of the processor to be scaled down to make large scale fabrication more feasible. Thus, what the AMD FX lacks in performance is made up for in value, costing less than its competitors by foregoing increased performance. The Bulldozer architecture has been succeeded by an improved Piledriver architecture released the following year. Most of the efforts done in creating the AMD FX processor were not made in vain, as they were able to be utilized a few years later, with the newer development of software and upgraded operating systems. The processor was ahead of its time, where it was not able to fully be utilized in computers. The design idea behind the Bulldozer architecture is in a way ingenious, and creative, in that it the first of its kind, using a design different from all previous processors. The AMD FX can be viewed as a pioneer, but was limited by other technology at the time, unable to realize the true capability and power. As of today, Advanced Micro Devices remains a leading competitor in the industry of processor manufacturing. 


## References

[1]    Advanced Micro Devices. AMD FX Processor Specifications. Santa Clara, CA. 
Advanced Micro Devices Inc. 2018. Print. 


[2]    G. Torres. [2018 November 9]. Inside the AMD Bulldozer Architecture. [Online]. https:
//www.hardwaresecrets.com/inside-the-amd-bulldozer-architecture/3/


[3]    R. Hodgin. [2018 November 9]. From Sand to Hand: How a CPU is made. [Online]. htt
ps://www.geek.com/chips/from-sand-to-hand-how-a-cpu-is-made-832492/


[4]    Wikipedia. [2018 November 9]. AMD FX. [E-book]. https://en.wikipedia.org/wiki/AM
D_FX


[5]    Hexus. [2018 November 9]. AMD FX-Series. [Online]. https://hexus.net/tech/tech-expla
ined/cpu/32240-amd-fx-series/


[6]    C. Chen, K. Shimano. [2018 November 9]. RISC Architecture-Pipelining. [Online]. 
https://cs.stanford.edu/people/eroberts/courses/soco/projects/risc/pipelining/index.html


[7]    J. Hruska. [2018 November 9]. Analyzing Bulldozer: Why AMD’s Chip is so 
disappointing. [Online]. https://www.extremetech.com/computing/100583-analyzing
-bulldozers-scaling-single-thread-performance


[8]    A.L.Shimpi. [2018 November 9]. The Bulldozer Review: AMD FX-8150 Tested. [Online]. 
https://www.anandtech.com/show/4955/the-bulldozer-review-amd-fx8150-tested/5


[9]    University of Denmark. The microarchitecture of Intel, AMD and VIA CPUs. Denmark. 
Technical University of Denmark. 1996- 2018. Print.


[10]    Wikichip. [2018 November 9]. Bulldozer - Microarchitectures - AMD. [E-book].https://en
.wikichip.org/wiki/amd/microarchitectures/bulldozer 

