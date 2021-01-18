---
$
key: 2021-01-11-11-37-predict-failure
title: Predict Failure 预测失效
date: 2021-01-11 11:37 +0800
tags: Physics 物理
---

### Maximum Normal Stress Criterion

The maximum stress criterion, also known as the normal stress, Coulomb, or Rankine criterion, is often used to predict the failure of brittle materials.
The maximum stress criterion states that failure occurs when the maximum (normal) principal stress reaches either the uniaxial tension strength st, or the uniaxial compression strength sc,

$-s_{c}<\left\{s_{1}, s_{2}\right\}<s_{t}$

where $s_{1}$ and $s_{2}$ are the principal stresses for 2D stress.

Graphically, the maximum stress criterion requires that the two principal stresses lie within the green zone depicted below,

![Figure 1](https://tenetai.com/iclass/f1.gif)

### Mohr's Theory

The **Mohr Theory of Failure**, also known as the Coulomb-Mohr criterion or internal-friction theory, is based on the famous [Mohr's Circle](https://www.efunda.com/formulae/solid_mechanics/mat_mechanics/mohr_circle.cfm). Mohr's theory is often used in predicting the failure of brittle materials, and is applied to cases of 2D stress.

Mohr's theory suggests that failure occurs when Mohr's Circle at a point in the body exceeds the envelope created by the two Mohr's circles for uniaxial tensile strength and uniaxial compression strength. This envelope is shown in the figure below,

![Figure 2](https://tenetai.com/iclass/f2.gif)

The left circle is for uniaxial compression at the limiting compression stress sc of the material. Likewise, the right circle is for uniaxial tension at the limiting tension stress st.

The middle Mohr's Circle on the figure (dash-dot-dash line) represents the maximum allowable stress for an intermediate stress state.

All intermediate stress states fall into one of the four categories in the following table. Each case defines the maximum allowable values for the two principal stresses to avoid failure.

![Table 1](https://tenetai.com/iclass/t1.jpg)

Graphically, Mohr's theory requires that the two principal stresses lie within the green zone depicted below,

![Figure 3](https://tenetai.com/iclass/f3.gif)

Also shown on the figure is the [maximum stress](#maximum-normal-stress-criterion) criterion (dashed line). This theory is less conservative than Mohr's theory since it lies outside Mohr's boundary.

<!--more-->
