---
layout: page
permalink: /research/index.html
title: Research
---

<div class="container">
    <div class="page-header">
        <h2>Selected Research Work</h2>
    </div>
    <div class="page-header">
        <h4>RAIN: Social Role-Aware Information Diffusion (AAAI'15)</h4>
        <p style="margin:3px;">Yang Yang, Jie Tang, Cane Wing-ki Leung, Yizhou Sun, Qicong Chen, Juanzi Li, and Qiang Yang</p>
    </div>
    <img width="350" src="/research/active_n.jpg" align="left" style="margin-left:20px;margin-right:20px">
    <p><small>Information diffusion, which studies how information is propagated in social networks, has attracted considerable research effort recently. However, most existing approaches do not distinguish between different social roles that nodes may play in the diffusion process.</small></p>
    <p><small>We study the interplay between users’ social roles and their influence on information diffusion. In particular, we propose a generative model that integrates social role extraction and diffusion modeling into a unified framework. We then estimate the unknown parameters of the proposed model based on historical diffusion data. The proposed model can be applied in several scenarios. For instance, at the micro-level, the proposed model can be used to predict whether a user will repost a given message; while at the macro-level, it is able to predict both the scale and the duration of a diffusion process. We evaluate the proposed model on a real social media data set. Compared with several alternative methods, our model shows better performance in both micro- and macro-level prediction tasks.</small></p>
    <p style="margin-left:20px">Paper:<img height="20" src="img/pdf.jpeg" style="margin: 3px;"><a href="works/roleaware/roleaware.pdf" style="margin-left:-3px; margin-right: 3px;">roleaware.pdf</a> | Data: <img height="20" src="img/cpp.jpeg" style="margin-right: 3px;margin-left: -3px"><a href="http://arnetminer.org/rain#b2967" style="margin-left:-3px; margin-right: 3px;">Details</a></p>
</div>

# Research Projects

## [OpenTuner]
[OpenTuner] is an extensible framework for building domain-specific
multi-objective program autotuners. OpenTuner supports fully customizable
configuration representations, an extensible technique representation to
allow for domain-specific techniques, and an easy to use interface for
communicating with the tuned program.


## [PetaBricks]
[PetaBricks] is a language and compiler where algorithmic choices are
exposed explicitly to create programs that define a search space of possible
algorithms.  The PetaBricks compiler then uses empirical autotuning to search
over these algorithms for an optimal version.


## [Kendo]
[Kendo] is a library that allows multithreaded programs, that would
normally produce nondeterministic output, to execute deterministically by
enforcing a dynamically computed and efficient ordering of lock acquisitions.


## [DMTCP]

[DMTCP][DMTCP] (Distributed MultiThreaded Checkpointing) is a tool to transparently
checkpoint and restart the state of a distributed cluster computation that
communicates through MPI or sockets.  It works on unmodified binaries at
the user level.


# Side Projects

## [LendingClubChecker]

[LendingClubChecker] is a python script to perform automated trading on the
peer to peer lending site Lending Club.

{% comment %}
## [ShowDB]

[ShowDB] is a script to index and automatically download TV shows with
Bit Torrent.
{% endcomment %}

# Open Source Contributions

While at Google I added support for sandboxing self-modifying code to Native
Client (part of Google Chrome).  I have also submitted bug fixes and minor
enhancements to a number of other open source projects.


[ShowDB]: https://github.com/jansel/showdb
[LendingClubChecker]: https://github.com/jansel/lendingclubchecker
[OpenTuner]: http://opentuner.org/
[PetaBricks]: http://projects.csail.mit.edu/petabricks/
[Kendo]: http://projects.csail.mit.edu/kendo/
[DMTCP]: http://dmtcp.sourceforge.net/


