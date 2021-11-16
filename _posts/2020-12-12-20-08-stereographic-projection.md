---
mathjax: true
key: 2020-12-12-20-08-stereographic-projection
title: Stereographic Projection 球面投影
date: 2020-12-12 20:08 +0800
tags: Math 数学
---

In geometry, the **stereographic projection** is a particular mapping (function) that projects a sphere onto a plane. The projection is defined on the entire sphere, except at one point: the projection point. Where it is defined, the mapping is smooth and bijective. It is conformal, meaning that it preserves angles at which curves meet. It is neither isometric nor area-preserving: that is, it preserves neither distances nor the areas of figures.

Intuitively, then, the stereographic projection is a way of picturing the sphere as the plane, with some inevitable compromises. Because the sphere and the plane appear in many areas of mathematics and its applications, so does the stereographic projection; it finds use in diverse fields including complex analysis, cartography, geology, and photography. In practice, the projection is carried out by computer or by hand using a special kind of graph paper called a stereographic net, shortened to stereonet, or Wulff net.

<img src="/assets/images/projection.gif" width="444">

Stereographic projections have a very simple algebraic form that results immediately from similarity of triangles. In the above figures, let the stereographic sphere have radius r, and the z-axis positioned as shown. Then a variety of different transformation formulas are possible depending on the relative positions of the projection plane and z-axis.

The transformation equations for a sphere of radius R are given by

$$
\begin{aligned}
&x=k \cos \phi \sin \left(\lambda-\lambda_{0}\right) \\
&y=k\left[\cos \phi_{1} \sin \phi-\sin \phi_{1} \cos \phi \cos \left(\lambda-\lambda_{0}\right)\right]
\end{aligned}
$$

where $\lambda_{0}$ is the central longitude, $\phi_{1}$ is the central latitude, and

$$
k=\frac{2 R}{1+\sin \phi_{1} \sin \phi+\cos \phi_{1} \cos \phi \cos \left(\lambda-\lambda_{0}\right)}
$$

The inverse formulas for latitude $\phi$ and longitude $\lambda$ are then given by

$$
\begin{aligned}
&\phi=\sin ^{-1}\left(\cos c \sin \phi_{1}+\frac{y \sin c \cos \phi_{1}}{\rho}\right) \\
&\lambda=\lambda_{0}+\tan ^{-1}\left(\frac{x \sin c}{\rho \cos \phi_{1} \cos c-y \sin \phi_{1} \sin c}\right)
\end{aligned}
$$

where

$$
\begin{aligned}
&\rho=\sqrt{x^{2}+y^{2}} \\
&c=2 \tan ^{-1}\left(\frac{\rho}{2 R}\right)
\end{aligned}
$$

and the two-argument form of the [inverse tangent](https://mathworld.wolfram.com/InverseTangent.html) function is best used for this computation.

For an [oblate spheroid](https://mathworld.wolfram.com/OblateSpheroid.html), $R$ can be interpreted as the "local radius," defined by

$$
R=\frac{R_{e} \cos \phi}{\left(1-e^{2} \sin ^{2} \phi\right) \cos \chi}
$$

where $R_{e}$ is the equatorial radius and $\chi$ is the [conformal latitude](https://mathworld.wolfram.com/ConformalLatitude.html).

通过球心的面在赤平面上的投影称为大圆，未通过球心的面在赤平面上的投影称为小圆。

由于构造特点各不相同，为了清楚反映构造起见，采用两种不同的投影方法：

- 一是面的极点图解，即π图解，就是用面的法线作为点来投影，
例如圆柱状褶皱的褶皱面的极点成一个大圆环带通过极点画出最合适的大圆，称为π圆，π圆的极点就是π轴。

- 另一种是面的大圆图解，即β图解，把所测量的每个面作为大圆来投影；
如果将圆柱状褶皱的褶皱面投影，所有大圆轨迹相交于一点，称为β轴，代表褶皱轴的产状。

<!--more-->
