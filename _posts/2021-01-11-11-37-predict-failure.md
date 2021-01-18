---
mathjax: true
key: 2021-01-11-11-37-predict-failure
title: Predict Failure 预测失效
date: 2021-01-11 11:37 +0800
tags: Physics 物理
---

![Stress Formula](https://tenetai.com/iclass/stress.jpg)

### Maximum Normal Stress Criterion

The maximum stress criterion, also known as the normal stress, Coulomb, or Rankine criterion, is often used to predict the failure of brittle materials.
The maximum stress criterion states that failure occurs when the maximum (normal) principal stress reaches either the uniaxial tension strength st, or the uniaxial compression strength sc,

$$-s_{c}<\left\{s_{1}, s_{2}\right\}<s_{t}$$

where $s_{1}$ and $s_{2}$ are the principal stresses for 2D stress.

Graphically, the maximum stress criterion requires that the two principal stresses lie within the green zone depicted below,

![Figure 1](https://tenetai.com/iclass/f1.gif)

### Mohr's Theory

The **Mohr Theory of Failure**, also known as the Coulomb-Mohr criterion or internal-friction theory, is based on the famous Mohr's Circle. Mohr's theory is often used in predicting the failure of brittle materials, and is applied to cases of 2D stress.

Mohr's theory suggests that failure occurs when Mohr's Circle at a point in the body exceeds the envelope created by the two Mohr's circles for uniaxial tensile strength and uniaxial compression strength. This envelope is shown in the figure below,

![Figure 2](https://tenetai.com/iclass/f2.gif)

The left circle is for uniaxial compression at the limiting compression stress sc of the material. Likewise, the right circle is for uniaxial tension at the limiting tension stress st.

The middle Mohr's Circle on the figure (dash-dot-dash line) represents the maximum allowable stress for an intermediate stress state.

All intermediate stress states fall into one of the four categories in the following table. Each case defines the maximum allowable values for the two principal stresses to avoid failure.

![Table 1](https://tenetai.com/iclass/t1.jpg)

Graphically, Mohr's theory requires that the two principal stresses lie within the green zone depicted below,

![Figure 3](https://tenetai.com/iclass/f3.gif)

Also shown on the figure is the [maximum stress](#) criterion (dashed line). This theory is less conservative than Mohr's theory since it lies outside Mohr's boundary.

![Mohr Theory](https://tenetai.com/iclass/mohr.jpg)

### Coulomb failure functions

The Coulomb failure criterion is commonly used to characterize failure in rocks. Both the shear and normal stress on a preexisting or an incipient fault plane satisfy conditions analogous to those of friction on a preexisting surface. The Coulomb stress, also referred to as Coulomb failure function, is given by

$$C F F=\tau_{\beta}+\mu\left(\sigma_{\beta}+p\right)$$

where τβ is the shear stress on the failure plane, σβ is the normal stress (positive for extension and negative for compression), p is the pore fluid pressure, and μ is the coefficient of friction. When CFF exceeds a critical value, failure occurs on the plane (Figure 1,left). Certain modifications to the above equation have been suggested for cases where rock stress is changed more rapidly than fluid pressure can change through flow. In a system where the x- and y-axes and fault displacements are horizontal and fault planes are vertical (z-axis), stress on a plane at an angle ψ from the x-axis (see Figure 1) is

$$\begin{array}{l}
\sigma_{11}=\sigma_{x x} \cos ^{2} \psi+2 \sigma_{x y} \sin \psi \cos \psi+\sigma_{y y} \sin ^{2} \psi \\
\sigma_{33}=\sigma_{x x} \sin ^{2} \psi-2 \sigma_{x y} \sin \psi \cos \psi+\sigma_{y y} \cos ^{2} \psi \\
\tau_{13}=\frac{1}{2}\left(\sigma_{y y}-\sigma_{x x}\right) \sin 2 \psi+\tau_{x y} \cos 2 \psi
\end{array}$$

For example, the Coulomb stress for a right-lateral motion on planes orientated at ψ with respect to the x-axis is

$$\sigma_{f}^{R}=\tau_{13}^{R}+\mu^{\prime} \sigma_{33}$$

<!--more-->
