# LV-model
LV model attempts to simulate competition between resistant and sensitive bacterial populations in the presence of an antibiotic.

## Description

This a project for the SABS modelling and scientific computing module. This attempts to make a Lotka-Volterra model that simulates competition between resistant and sensitive bacterial populations.

Lotka-Volterra model is a model made of a collection of nonlinear differential equations that are used to describe the relationship between two biological entities. It is usually applied to prey and predator interactions, but it can be modified to describe the dynamics of a slightly different nature, like in this case, resistant against sensitive bacterial populations in a closed system in the presence of an antibiotic.

Equations

dRdt = r_R * R * (1 - (R + alpha_RS * S) / K_R) - beta_R * A * R

The rate of change of the resistant bacteria over time illustrates competition between sensitive and resistant and antibiotics.

dSdt = r_S * S * (1 -(S + alpha_SR * R) / K_S) - beta_S * A * S + mu * S

The rate of change of the sensitive bacteria population over time illustrates competition between sensitive, resistant and antibiotics. It also considers the sensitive population's mutation rate, which converts it to the resistant population.

dAdt = -delta_A * A

Describes the change of the antibiotic over time in a system. This is an exponential decay equation.




Model assumption:


- Homogenous mixing of the resistant and sensitive bacterial populations plus antibiotic
- Parameters are constant
- Environment is constant
- DeltaA: The degradation rate of the antibiotic is constant- which needs to be corrected as this constant does not consider antibiotics with a minor secondary mechanism of action, pharmacokinetics, environmental degradation and potential active metabolites.

## Parameters of the model

#Parameters of the equation:

rR, the growth rate of the resistant population.

S, the growth rate of the sensitive population

KR, the carrying capacity of the resistant population

KS, the carrying capacity of the sensitive population

AlphaRS, the competition coefficient representing the effect of the sensitive population on the growth rate of the resistance population

AlphaSR, The competition coefficient representing the effect of the resistant population on the growth rate of the sensitive population

AlphaR, the effectiveness of the antibiotic against the resistant population.

AlphaS, the effectiveness of the antibiotic against the sensitive pop.

Mu, the mutation or acquisition rate at which sensitive bacteria become resistant.
DeltaA, the degradation rate of the antibiotic concentration over time.

## Installation

You can clone this repository or download it as a py file and run it on your computer.

