# ML-Applications-to-Process-Engineering-PMMA-Reactor-Unit-
ML Applications to Process Engineering (PMMA Reactor Unit)

The PMMA production process involves a free-radical polymerization of methyl methacrylate (MMA) using a Continuous Stirred-Tank Reactor (CSTR) configuration. Azo-bis-isobutyronitrile (AIBN) serves as the initiator for the polymerization reaction, while toluene functions as the solvent.

Process Description:
A measured amount of MMA, AIBN, and toluene are continuously fed into the CSTR. AIBN decomposes upon heating within the reactor, releasing free radicals that initiate the polymerization of MMA molecules. Polymerization proceeds as MMA monomers react with the free radicals, forming PMMA chains. The exothermic nature of the reaction causes heat to be generated. The cooling jacket surrounding the reactor removes this heat to maintain a stable temperature within the reactor. As polymerization progresses, PMMA chains grow in length, leading to the formation of the desired polymer product. The polymer solution is continuously removed from the reactor for further processing or purification. Overall, this system enables the efficient and continuous production of PMMA through free-radical polymerization, with precise control over reaction conditions to ensure high-quality polymer output.

The process uses 7 input variables as
● Temperature (T): The temperature at the reactor outlet.
● Jacket Temperature (Tj): The temperature of the coolant outlet.
● Coolant water flow rate (Fcw): The rate at which water as a coolant flows through the system for temperature regulation.
● Monomer inlet Flow rate (F): The rate at which monomer is introduced into the system or reactor.
● Coolant inlet temperature of water (Two): The initial temperature of the coolant water entering the system.
● Inlet temperature (Tin): The initial temperature of the input material entering the reactor.
And target variable as
● Monomer concentration (Cm): The concentration or amount of the monomer at the reactor outlet.

The aim of this project is to optimize the free-radical polymerization process of methyl methacrylate (MMA) to produce Polymethyl methacrylate (PMMA) efficiently. The objective is to maintain a target monomer concentration within the reactor to ensure consistent product quality and reaction efficiency and reduce wastage. We aim to develop optimal predictive models for the monomer concentration required, based on multivariate regression techniques and compare the predictive performance of the developed models on the basis of R2 value, SSE, AIC, BIC.

For modelling, Fcw and Two were directly dropped as they remain constant for the entire data set. 
Parameters remaining, with index 0 to 4:
0: Initiator Concentration(CI)
1: Temperature (T)
2: Jacket Temperature (Tj)
3: Monomer inlet Flowrate (F)
4: Inlet temperature of Feed (Tin)

We then selected the optimal features/subsets on the basis of subset selection method, and applied various linear and non linear regression models, like lasso regression, PCA, LSTM, Shallow and Deep Neural Networks (ANN), KNN, and then analyzed the performance of each model to reach certain conclusions, as explained in the ppt attached.

Note: The project was part of my course of Machine Learning and its Applications, and is based on the reactor details from a published paper (https://www.semanticscholar.org/paper/Comparison-of-unconstrained-nonlinear-state-on-a-Shenoy-Prasad/01ab779dfa5f84b71b224d007e40f23b83535564) and simulated data provided by the professor. 
