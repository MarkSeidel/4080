# Physics 4080/5080 - Artificial Intelligence and Machine Learning Methods with Applications to Physics

Ethan Nussinov, Mark Seidel

Project: 
1. Simulate the evolution of a two-qubit quantum system
   - Using the Lindblad master equation. Model the system's decoherence and amplitude damping over time.
   - This equation is widely used to model open quantum systems interacting with their environment, and especially when noise and decoherence are present. This is a standard way to simulate quantum systems in quantum physics and information theory.
   - Decoherence and damping are realistic features of quantum systems in practice, especially in experimental settings where it is difficult to isolate from the environment.
  
2. Extract features from the system's density matrices
   - During its time evolution, include purity, entropy, eigenvalues, and expectation values of Pauli matrices for each qubit.
   - Density matrices are used to describe the state of a quantum system, espeically when there are mixed/partially known states.


3. Calculate the concurrence of the system's density matrices
   - In order to quantify the level of quantum entanglement at each time step.
   - Concurrence is a well established measure of quantum entanglement for two-qubit systems. Ranges from 0 (seperable) to 1 (maximally entangled).

4. Classify the system's states as either 'entangled' or 'seperable'
   - Based on the concurrence using a machine learning model.
   - Current approach uses random forest - a non parametric model is useful when working with complex data like the features we extract from quantum states, handles mixed data types well, and are robust to overfitting.
