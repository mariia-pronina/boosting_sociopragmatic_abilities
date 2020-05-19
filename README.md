# Script for group distribution

This algorithm was created for Pronina, Hübscher, Holler & Prieto (in preparation) study. It was used to guarantee a homogeneous distribution of participants across the three training conditions. The participants were preschool children who attended 5 differents classes in 2 different schools. Since the training was necessarily carried out within the class, the main aim of the algorithm is to allocate participants to 3 different training conditions while controlling for class distribution on the basis of pretest performance.

This algorithm measures the degree of similarity between different test scores and assigns the participants to experimental conditions while taking into account children's class distribution and preserving general similarity of the distributions by conditions. The participants are allocated to a certain condition on the the basis on four test scores: Emotion Understanding, Mental Verb Comprehension, ToM and the Pragmatic Test. The division of participants into groups is undertaken in three steps. First, the distance between two participants' scores is calculated. In order to do so, the cosine between four-dimentional vectors (corresponding to the four tests) is measured. Then, the distance matrix of all class participants is obtained. Thus, the closer the vectors are, the smaller the distantance is. Afterwards, a minimum of all distances and its location (a vector) are calculated, which results in close vector pairs. Finally, the algorithm stops when one of the groups contains half of the participants. The remaining children are assigned to the other group.

Pronina, Hübscher, Holler & Prieto (in preparation). Mental state conversational training boosts preschool children’s sociopragmatic abilities.
