# Computational Neuroscience Implementations
## Single Neurons
  * LIF (Leaky Integrate-and-Fire Model): A simplified neuron model where the membrane potential leaks over time (decays) and integrates incoming input until it reaches a threshold, at which point it "fires" (emits a spike) and resets.
    
  * ELIF (Exponential Leaky Integrate-and-Fire Model): This is an extension of the LIF model that includes an exponential term to better describe the action potential's shape. It models the sharp rise in membrane potential when nearing the firing threshold, which better matches biological neurons.
   
  * ALIF (Adaptive Leaky Integrate-and-Fire Model): An adaptation of the LIF model where the firing threshold or other properties of the neuron adapt over time based on the neuron's spiking history. This captures neural plasticity, simulating how neurons become less likely to fire after repeated spiking.
    
  * AELIF (Adaptive Exponential Leaky Integrate-and-Fire Model): Combines the exponential term from ELIF and the adaptation mechanism from ALIF. This model captures both the sharpness of spikes and the adaptability of the neuron's firing threshold, making it closer to the behavior of biological neurons.

######
* neural population
  * inhibitory population
  * excitatory population
  * excitatory and inhibitory population
######
* neural networks
  * Spiking neural network
  * balanced network
######
* neural learning
  * STDP
  * Reward-Based STDP
