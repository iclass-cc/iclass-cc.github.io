---
mathjax: true
mathjax_autoNumber: true
key: 2021-01-07-05-25-divergence-curl
title: Divergence & Curl 散度和旋度
date: 2021-01-07 05:25 +0800
tags: Physics 物理
---

## Divergence

Divergence is an operation on a vector field that tells us how the field behaves toward or away from a point. Locally, the divergence of a vector field $\mathbf{F}$ in $\mathbb{R}^2$ or $\mathbb{R}^3$ at a particular point $P$ is a measure of the “outflowing-ness” of the vector field at $P$. If $\mathbf{F} represents the velocity of a fluid, then the divergence of $\mathbf{F}$ at $P$ measures the net rate of change with respect to time of the amount of fluid flowing away from $P$ (the tendency of the fluid to flow “out of” P). In particular, if the amount of fluid flowing into $P$ is the same as the amount flowing out, then the divergence at $P$ is zero.

### Definition: divergence in $\mathbb{R}^3$

If $\mathbf{F} = \langle P,Q,R \rangle$ is a vector field in $\mathbb{R}^3$ and $P_x, \, Q_y,$ and $R_z$ all exist, then the divergence of $\mathbf{F} is defined by

$$\begin{align} \text{div}\, F &= P_x + Q_y + R_z \\
[4pt] &= \dfrac{\partial P}{\partial x} + \dfrac{\partial Q}{\partial y} + \dfrac{\partial R}{\partial z}. \end{align}$$

Note the divergence of a vector field is not a vector field, but a scalar function. In terms of the gradient operator

$$\vecs \nabla = \langle \dfrac{\partial}{\partial x}, \dfrac{\partial}{\partial y}, \dfrac{\partial}{\partial z} \rangle$$

divergence can be written symbolically as the dot product

$$\text{div}\, \vecs F = \vecs \nabla \cdot \mathbf{F}.$$

## Curl

The second operation on a vector field that we examine is the curl, which measures the extent of rotation of the field about a point. Suppose that $\mathbf{F}$ represents the velocity field of a fluid. Then, the curl of $\mathbf{F}$ at point $P$ is a vector that measures the tendency of particles near $P$ to rotate about the axis that points in the direction of this vector. The magnitude of the curl vector at $P$ measures how quickly the particles rotate around this axis. In other words, the curl at a point is a measure of the vector field’s “spin” at that point. Visually, imagine placing a paddlewheel into a fluid at $P$ , with the axis of the paddlewheel aligned with the curl vector (Figure below). The curl measures the tendency of the paddlewheel to rotate.

![Figure Curl](https://tenetai.com/iclass/c1.jpg)

<!--more-->
