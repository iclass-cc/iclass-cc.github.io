---
mathjax: true
pageview: true
key: 2022-03-14-21-33-rocket-equation
title: Rocket Equation 火箭方程
date: 2022-03-14 21:33 +0800
tags: Physics 物理
---

<img src="https://marslink.in/images/rocket.jpg" width="222" align="right">

**Rocket equation** is a mathematical equation that describes the motion of vehicles that follow the basic principle of a rocket: a device that can apply acceleration to itself using thrust by expelling part of its mass with high velocity can thereby move due to the conservation of momentum.

## Ideal Rocket Equation

$$
\Delta v=v_{\mathrm{e}} \ln \frac{m_{0}}{m_{f}}=I_{\mathrm{sp}} g_{0} \ln \frac{m_{0}}{m_{f}}
$$

where:

> $\Delta v$ is delta-v – the maximum change of velocity of the vehicle (with no external forces acting).
>
> ${m_{0}}$ is the initial total mass, including propellant, a.k.a. wet mass.
>
> ${m_{f}}$ is the final total mass without propellant, a.k.a. dry mass.
>
> $v_{\mathrm{e}} = I_{\mathrm{sp}} g_{0}$ is the effective exhaust velocity, where:
>
>> $I_{\mathrm{sp}}$ is the specific impulse in dimension of time.
>>
>> $g_{0}$ is standard gravity.
>
> $\ln$ is is the natural logarithm function.

Given the effective exhaust velocity $v_{\mathrm{e}}$ (determined by a rocket motor's design), a desired delta-v (for example, escape velocity), and a given dry mass ${m_{f}}$, the equation can be used to find the required wet mass ${m_{0}} - {m_{f}}$ :

$$
m_{0}=m_{f} e^{\frac{\Delta v}{v_{\mathrm{e}}}}
$$

<img src="/assets/images/rocket.svg" width="123" align="right">

So the necessary wet mass grows exponentially with the desired delta-v, as illustrated in the chart.

## Terms of the equation

### Delta-v

Delta-v (literally "change in velocity"), symbolised as ${\Delta v}$ and pronounced delta-vee, as used in spacecraft flight dynamics, is a measure of the impulse that is needed to perform a maneuver such as launching from, or landing on a planet or moon, or an in-space orbital maneuver. It is a scalar that has the units of speed. As used in this context, it is not the same as the physical change in velocity of the vehicle.

Delta-v is produced by reaction engines, such as rocket engines and is proportional to the thrust per unit mass, and burn time, and is used to determine the mass of propellant required for the given manoeuvre through the rocket equation.

For multiple manoeuvres, delta-v sums linearly.

For interplanetary missions delta-v is often plotted on a porkchop plot which displays the required mission delta-v as a function of launch date.

### Mass fraction

In aerospace engineering, the propellant mass fraction is the portion of a vehicle's mass which does not reach the destination, usually used as a measure of the vehicle's performance. In other words, the propellant mass fraction is the ratio between the propellant mass and the initial mass of the vehicle. In a spacecraft, the destination is usually an orbit, while for aircraft it is their landing location. A higher mass fraction represents less weight in a design. Another related measure is the payload fraction, which is the fraction of initial weight that is payload.

### Effective exhaust velocity

The effective exhaust velocity is often specified as a specific impulse and they are related to each other by:

$$
v_{\mathrm{e}}=g_{0} I_{\mathrm{sp}}
$$

where

> $I_{\mathrm{sp}}$ is the specific impulse in seconds,
>
> $v_{\mathrm{e}}$ is the specific impulse measured in $m/s$, which is the same as the effective exhaust velocity measured in $m/s$ (or $ft/s$ if g is in $ft/s^{2}$),
>
> $g_{0}$ is the standard gravity, 9.80665 $m/s^{2}$ (in Imperial units 32.174 $ft/s^{2}$).

## Examples

- [Single-stage-to-orbit](https://en.m.wikipedia.org/wiki/Single-stage-to-orbit) rocket: $1-e^{-9.7 / 4.5}=0.884$, therefore 88.4% of the initial total mass has to be propellant. The remaining 11.6% is for the engines, the tank, and the payload.
- [Two-stage-to-orbit](https://en.m.wikipedia.org/wiki/Two-stage-to-orbit): suppose that the first stage should provide a ${\Delta v}$ of 5,000 meters per second (16,000 $ft/s$); $1-e^{-5.0 / 4.5}=0.671$, therefore 67.1% of the initial total mass has to be propellant to the first stage. The remaining mass is 32.9%. After disposing of the first stage, a mass remains equal to this 32.9%, minus the mass of the tank and engines of the first stage. Assume that this is 8% of the initial total mass, then 24.9% remains. The second stage should provide a ${\Delta v}$ of 4,700 meters per second (15,000 $ft/s$); $1-e^{-4.7 / 4.5}=0.648$, therefore 64.8% of the remaining mass has to be propellant, which is 16.2% of the original total mass, and 8.7% remains for the tank and engines of the second stage, the payload, and in the case of a space shuttle, also the orbiter. Thus together 16.7% of the original launch mass is available for all engines, the tanks, and payload.

## Stages

In the case of sequentially thrusting rocket stages, the equation applies for each stage, where for each stage the initial mass in the equation is the total mass of the rocket after discarding the previous stage, and the final mass in the equation is the total mass of the rocket just before discarding the stage concerned. For each stage the specific impulse may be different.

For example, if 80% of the mass of a rocket is the fuel of the first stage, and 10% is the dry mass of the first stage, and 10% is the remaining rocket, then

$$
\begin{aligned}
\Delta v &=v_{\mathrm{e}} \ln \frac{100}{100-80} \\
&=v_{\mathrm{e}} \ln 5 \\
&=1.61 v_{\mathrm{e}}
\end{aligned}
$$

With three similar, subsequently smaller stages with the same $v_{\mathrm{e}}$ for each stage, we have

$$
\Delta v=3 v_{\mathrm{e}} \ln 5=4.83 v_{\mathrm{e}}
$$

and the payload is 10% × 10% × 10% = 0.1% of the initial mass.

A comparable [SSTO](https://en.m.wikipedia.org/wiki/Single-stage-to-orbit) rocket, also with a 0.1% payload, could have a mass of 11.1% for fuel tanks and engines, and 88.8% for fuel. This would give

$$
\Delta v=v_{\mathrm{e}} \ln (100 / 11.2)=2.19 v_{\mathrm{e}}
$$

If the motor of a new stage is ignited before the previous stage has been discarded and the simultaneously working motors have a different specific impulse (as is often the case with solid rocket boosters and a liquid-fuel stage), the situation is more complicated.

## Derivations

Consider the following system:

<img src="/assets/images/mass.svg" width="222" align="right">

In the following derivation, "the rocket" is taken to mean "the rocket and all of its unexpended propellant".

Newton's second law of motion relates external forces ($F_{i}$) to the change in linear momentum of the whole system (including rocket and exhaust) as follows:

$$
\sum F_{i}=\lim _{\Delta t \rightarrow 0} \frac{P_{2}-P_{1}}{\Delta t}
$$

where $P_{1}$ is the momentum of the rocket at time $t = 0$ :

$$
P_{1}=(m+\Delta m) V
$$

and $P_{2}$ is the momentum of the rocket and exhausted mass at time $t = \Delta t$ :

$$
P_{2}=m(V+\Delta V)+\Delta m V_{\mathrm{e}}
$$

and where, with respect to the observer:

$V$ is the velocity of the rocket at time $t = 0$

$V+\Delta V$ is the velocity of the rocket at time $t = \Delta t$

$V_{\mathrm{e}}$ is the velocity of the mass added to the exhaust (and lost by the rocket) during time $\Delta t$

$m+\Delta m$ is the mass of the rocket at time $t = 0$

$m$  is the mass of the rocket at time $t = \Delta t$

The velocity of the exhaust $V_{\mathrm{e}}$ in the observer frame is related to the velocity of the exhaust in the rocket frame $v_{\mathrm{e}}$ by (since exhaust velocity is in the negative direction)

$$
V_{\mathrm{e}}=V-v_{\mathrm{e}}
$$

Solving yields:

$$
P_{2}-P_{1}=m \Delta V-v_{\mathrm{e}} \Delta m
$$

and, using $dm = - \Delta m$ , since ejecting a positive $\Delta m$ results in a decrease in mass in time,

$$
\sum F_{i}=m \frac{d V}{d t}+v_{\mathrm{e}} \frac{d m}{d t}
$$

If there are no external forces then $\sum F_{i} = 0$ (conservation of linear momentum) and

$$
-m \frac{d V}{d t}=v_{\mathrm{e}} \frac{d m}{d t}
$$

Assuming $v_{\mathrm{e}}$ is constant, this may be integrated as follows:

$$
-\int_{V}^{V+\Delta V} \mathrm{~d} V=v_{e} \int_{m_{0}}^{m_{f}} \frac{1}{m} \mathrm{~d} m
$$

This then yields

$$
\Delta V=v_{\mathrm{e}} \ln \frac{m_{0}}{m_{f}}
$$

or equivalently

$$
m_{f}=m_{0} e^{-\Delta V / v_{\mathrm{e}}}
$$

or

$$
m_{0}=m_{f} e^{\Delta V / v_{\mathrm{e}}}
$$

or 

$$
m_{0}-m_{f}=m_{f}\left(e^{\Delta V / v_{\mathrm{e}}}-1\right)
$$

where $m_{0}$ is the initial total mass including propellant, $m_{f}$ the final mass, and $v_{\mathrm{e}}$ the velocity of the rocket exhaust with respect to the rocket (the specific impulse, or, if measured in time, that multiplied by gravity-on-Earth acceleration).

The value $m_{0} - m_{f}$ is the total working mass of propellant expended.

$\Delta V$ is the integration over time of the magnitude of the acceleration produced by using the rocket engine (what would be the actual acceleration if external forces were absent). In free space, for the case of acceleration in the direction of the velocity, this is the increase of the speed. In the case of an acceleration in opposite direction (deceleration) it is the decrease of the speed. Of course gravity and drag also accelerate the vehicle, and they can add or subtract to the change in velocity experienced by the vehicle. Hence delta-v may not always be the actual change in speed or velocity of the vehicle.

### Impulse-based

The equation can also be derived from the basic integral of acceleration in the form of force (thrust) over mass. By representing the delta-v equation as the following:

$$
\Delta v=\int_{t_{0}}^{t_{f}} \frac{|T|}{m_{0}-t \Delta m} d t
$$

where $T$ is thrust, $m_{0}$ is the initial (wet) mass and $\Delta m$ is the initial mass minus the final (dry) mass,

and realising that the integral of a resultant force over time is total impulse, assuming thrust is the only force involved,

$$
\int_{t_{0}}^{t_{f}} F d t=J
$$

The integral is found to be:

$$
J \frac{\ln \left(m_{0}\right)-\ln \left(m_{f}\right)}{\Delta m}
$$

Realising that impulse over the change in mass is equivalent to force over propellant mass flow rate (p), which is itself equivalent to exhaust velocity,

$$
\frac{J}{\Delta m}=\frac{F}{p}=V_{\mathrm{exh}}
$$

the integral can be equated to

$$
\Delta v=V_{\mathrm{exh}} \ln \left(\frac{m_{0}}{m_{f}}\right)
$$

### Acceleration-based

Imagine a rocket at rest in space with no forces exerted on it (Newton's First Law of Motion). From the moment its engine is started (clock set to 0) the rocket expels gas mass at a constant mass flow rate $R$ ($kg/s$) and at exhaust velocity relative to the rocket $v_{e}$ ($m/s$). This creates a constant force $F$ propelling the rocket that is equal to $R \times v_{e}$. The rocket is subject to a constant force, but its total mass is decreasing steadily because it is expelling gas. According to Newton's Second Law of Motion, its acceleration at any time $t$ is its propelling force $F$ divided by its current mass $m$:

$$
a=\frac{d v}{d t}=-\frac{F}{m(t)}=-\frac{R v_{\mathrm{e}}}{m(t)}
$$

Now, the mass of fuel the rocket initially has on board is equal to $m_{0} – m_{f}$. For the constant mass flow rate $R$ it will therefore take a time $T = (m_{0} – m_{f})/R$ to burn all this fuel. Integrating both sides of the equation with respect to time from $0$ to $T$ (and noting that $R = dm/dt$ allows a substitution on the right), we obtain

$$
\Delta v=v_{f}-v_{0}=-v_{\mathrm{e}}\left[\ln m_{f}-\ln m_{0}\right]=v_{\mathrm{e}} \ln \left(\frac{m_{0}}{m_{f}}\right)
$$

### Limit of finite mass "pellet" expulsion

The rocket equation can also be derived as the limiting case of the speed change for a rocket that expels its fuel in the form of $N$ pellets consecutively, as $N \rightarrow \infty$, with an effective exhaust speed $v_{\mathrm{eff}}$ such that the mechanical energy gained per unit fuel mass is given by $\frac{1}{2} v_{\mathrm{eff}}^{2}$ .

In the rocket's center-of-mass frame, if a pellet of mass $m_{p}$ is ejected at speed $u$ and the remaining mass of the rocket is $m$ , the amount of energy converted to increase the rocket's and pellet's kinetic energy is

$$
\frac{1}{2} m_{p} v_{\mathrm{eff}}^{2}=\frac{1}{2} m_{p} u^{2}+\frac{1}{2} m(\Delta v)^{2}
$$

Using momentum conservation in the rocket's frame just prior to ejection, $u=\Delta v \frac{m}{m_{p}}$ , from which we find

$$
\Delta v=v_{\mathrm{eff}} \frac{m p}{\sqrt{m\left(m+m_{p}\right)}}
$$

Let $\phi$ be the initial fuel mass fraction on board and $m_{0}$ the initial fueled-up mass of the rocket. Divide the total mass of fuel $\phi m_{0}$ into $N$ discrete pellets each of mass $m_{p} = \phi m_{0} / N$ . The remaining mass of the rocket after ejecting $j$ pellets is then $m=m_{0}(1-j\phi /N)$
. The overall speed change after ejecting $j$ pellets is the sum

$$
\Delta v=v_{\mathrm{eff}} \sum_{j=1}^{j=N} \frac{\phi / N}{\sqrt{(1-j \phi / N)(1-j \phi / N+\phi / N)}}
$$

Notice that for large $N$ the last term in the denominator $\phi / N \ll 1$ and can be neglected to give

$$
\Delta v \approx v_{\mathrm{eff}} \sum_{j=1}^{j=N} \frac{\phi / N}{1-j \phi / N}=v_{\mathrm{eff}} \sum_{j=1}^{j=N} \frac{\Delta x}{1-x_{j}} \text { where } \Delta x=\frac{\phi}{N} \text { and } x_{j}=\frac{j \phi}{N}
$$

As $N \rightarrow \infty$ this Riemann sum becomes the definite integral

$$
\lim _{N \rightarrow \infty} \Delta v=v_{\mathrm{eff}} \int_{0}^{\phi} \frac{d x}{1-x}=v_{\mathrm{eff}} \ln \frac{1}{1-\phi}=v_{\mathrm{eff}} \ln \frac{m_{0}}{m_{f}}
$$

since the final remaining mass of the rocket is $m_{f}=m_{0}(1-\phi)$ .

### Special relativity

If special relativity is taken into account, the following equation can be derived for a relativistic rocket, with $\Delta v$ again standing for the rocket's final velocity (after expelling all its reaction mass and being reduced to a rest mass of $m_{1}$) in the inertial frame of reference where the rocket started at rest (with the rest mass including fuel being $m_{0}$) , and $c$ standing for the speed of light in a vacuum:

$$
\frac{m_{0}}{m_{1}}=\left[\frac{1+\frac{\Delta v}{c}}{1-\frac{\Delta v}{c}}\right]^{\frac{c}{2 v_{\mathrm{e}}}}
$$

Writing $\frac{m_{0}}{m_{1}}$ as $R$ allows this equation to be rearranged as

$$
\frac{\Delta v}{c}=\frac{R^{\frac{2 v_{\mathrm{e}}}{c}}-1}{R^{\frac{2 v_{\mathrm{e}}}{c}}+1}
$$

Then, using the identity

$$
R^{\frac{2 v_{\mathrm{e}}}{c}}=\exp \left[\frac{2 v_{\mathrm{e}}}{c} \ln R\right]
$$

(here "$\exp$" denotes the exponential function; see also Natural logarithm as well as the "power" identity at Logarithmic identities)

and the identity $\tanh x=\frac{e^{2 x}-1}{e^{2 x}+1}$ (see [Hyperbolic function](https://en.wikipedia.org/wiki/Hyperbolic_function)), this is equivalent to

$$
\Delta v=c \tanh \left(\frac{v_{\mathrm{e}}}{c} \ln \frac{m_{0}}{m_{1}}\right)
$$

<!--more-->
