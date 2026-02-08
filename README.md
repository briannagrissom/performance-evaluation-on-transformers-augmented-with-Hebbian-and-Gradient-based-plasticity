## Overview

This project is an extension of the original research "[Enabling Robust In-Context Memory and Rapid Task Adaptation in Transformers with Hebbian and Gradient-Based
Plasticity](https://arxiv.org/pdf/2510.21908)".

In this report, a performance evaluation on decoder-only Transformers augmented with "fast weights" is completed, allowing the model to update its weights during inference. 

The first fast weight update is a Hebbian rule update, a biologically inspired mechanism that updates the fast weights based on pre-and post-synaptic activity correlations. 
The second fast weight update is a Gradient update, a modern framework that makes use of gradient descent on global information to update the pre- and post-synaptic weights.

The performance evaluations are completed on copying, one-shot image classification, and three-shot text category classification tasks, where we discovered that the Gradient rule 
had the highest relative performance when the number of training iterations is increased for complex tasks. 
