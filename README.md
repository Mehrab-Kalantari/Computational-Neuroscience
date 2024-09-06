# Computational Neuroscience Implementations
## Single Neurons
  * **LIF (Leaky Integrate-and-Fire Model):** A simplified neuron model where the membrane potential leaks over time (decays) and integrates incoming input until it reaches a threshold, at which point it "fires" (emits a spike) and resets.
    
  * **ELIF (Exponential Leaky Integrate-and-Fire Model):** This is an extension of the LIF model that includes an exponential term to better describe the action potential's shape. It models the sharp rise in membrane potential when nearing the firing threshold, which better matches biological neurons.
   
  * **ALIF (Adaptive Leaky Integrate-and-Fire Model):** An adaptation of the LIF model where the firing threshold or other properties of the neuron adapt over time based on the neuron's spiking history. This captures neural plasticity, simulating how neurons become less likely to fire after repeated spiking.
    
  * **AELIF (Adaptive Exponential Leaky Integrate-and-Fire Model):** Combines the exponential term from ELIF and the adaptation mechanism from ALIF. This model captures both the sharpness of spikes and the adaptability of the neuron's firing threshold, making it closer to the behavior of biological neurons.

######
## Neural Populations
  * **Inhibitory Population:** This refers to a group of inhibitory neurons, which reduce the likelihood of firing in their target neurons. They do this by releasing neurotransmitters (like GABA) that hyperpolarize the membrane potential of the post-synaptic neuron, making it less likely to reach the firing threshold.
    
  * **Excitatory Population:** This is a group of excitatory neurons, which increase the likelihood that their target neurons will fire. They release neurotransmitters (such as glutamate) that depolarize the membrane potential of the post-synaptic neuron, bringing it closer to the firing threshold.
    
  * **Excitatory and Inhibitory Population:** This refers to a neural network or system that contains both excitatory and inhibitory neurons. These populations interact to create balanced network activity. Excitatory neurons drive activation, while inhibitory neurons provide necessary feedback to stabilize the system, ensuring that neural circuits don’t become too active or too silent.
    
######
## Neural Networks
  * **Spiking Neural Network (SNN):** A type of artificial neural network that more closely mimics the behavior of biological neurons. In SNNs, neurons communicate by sending spikes (discrete events) rather than continuous values. These spikes represent action potentials, and the timing of spikes plays a key role in information processing. Neurons in SNNs integrate input over time and fire (or "spike") once the membrane potential crosses a certain threshold.
    
  * **Balanced Network:** A neural network where the excitatory and inhibitory inputs are balanced, ensuring that network activity remains stable and does not lead to runaway excitation or total suppression. In such networks, the overall strength of excitation (driving neuron firing) is counteracted by inhibition (which suppresses firing), keeping the network’s dynamics in check.
    
######
## Neural Learning
Learning in biological systems involves modifying the strength of synapses (connections between neurons) based on activity patterns. In computational models, this is often achieved through rules like Hebbian learning, where "neurons that fire together wire together," meaning synaptic strength increases when pre- and post-synaptic neurons are active simultaneously.


  * **STDP (Spike-Timing-Dependent Plasticity):** STDP is a biologically inspired learning rule that adjusts synaptic strengths based on the precise timing of spikes between pre- and post-synaptic neurons. It’s a form of synaptic plasticity. If the pre-synaptic neuron fires just before the post-synaptic neuron, the synapse is strengthened. If the post-synaptic neuron fires first, the synapse is weakened.
    
  * **Reward-Based STDP:** Reward-Based STDP combines spike-timing-dependent plasticity with a reinforcement learning mechanism, where the synaptic changes depend not only on the timing of spikes but also on a reward signal. In this model, when the network receives a reward, synaptic modifications are more likely to follow the STDP rule, enhancing or weakening connections based on timing. Over time, the system learns to produce actions that maximize rewards.
