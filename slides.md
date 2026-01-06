---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /sundog.jpg
# some information about your slides (markdown enabled)
title: iRAD 2026
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: false
pointer: true

slideNumber: true
---

## A Novel Numerical Method for Radar Cross Section Computation Using the Lattice Boltzmann Framework

<div class="mt-7 text-center leading-relaxed">
  <span class="text-l font-semibold">Mohd Meraj Khan<sup>a</sup></span>,
  <span class="text-l">Sumesh P. Thampi<sup>b</sup></span>
  and
  <span class="text-l">Anubhab Roy<sup>a</sup></span>
</div>


<div class="mt-8 text-3.5 leading-tight text-center">
  <sup class="text-3.5 align-super">a</sup> Department of Applied Mechanics<br>
  <sup class="text-3.5 align-super">b</sup> Department of Chemical Engineering
</div>


<div class="mt-4 text-4 text-center ">
  Indian Institute of Technology Madras, Chennai, India
</div>




<div class="my-18 flex justify-center items-center">
  <img src="/figures/IITM_Logo.png" alt="IIT Madras logo" class="h-24 w-24 opacity-90">
</div>

<div class="text-l leading-tight text-center mt-10 mb-10">
  iRAD 2026
</div>



<div class="abs-br m-1.5 text-2">
  Background image: https://pixabay.com
</div>

---

## Scattering of EM waves in climate studies

<!-- <div v-click="1" class="text-center mt-5">
Scattering of electromagnetic waves in nature
</div> -->

<div class="grid grid-cols-3 gap-15 mt-10">
  <figure class="text-center">
    <img src="/figures/scattering/sky_unsplash.jpg" alt="Image 1" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Blue sky and white cloud
      <div class="text-2">(Source: unsplash.com)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/scattering/rainbow_unsplash.jpg" alt="Image 2" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Rainbow
      <div class="text-2">(Source: unsplash.com)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/scattering/halo_wgrz.com.png" alt="Image 3" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Sundog and Halo
      <div class="text-2">(Source: wgrz.org)</div>
    </figcaption>
  </figure>
</div>

<div v-click="1" class="grid grid-cols-3 gap-15 mt-10">
  <figure class="text-center">
    <img src="/figures/energy-budget.jpg" alt="Image 1" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Radiation budget
      <div class="text-2">(Source: climatesight.org)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/dust_storm.png" alt="Image 2" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Dust storm
      <div class="text-2">(Source: icarda.org)</div>
    </figcaption>
  </figure>
  
  <figure class="text-center">
    <img src="/figures/hydrometeor.jpg" alt="Image 3" class="w-full h-auto">
    <figcaption class="text-3 mt-2">
      Precipitation
      <div class="text-2">(Source: pexels.com)</div>
    </figcaption>
  </figure>
</div>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>


<!--






## Scattering of EM waves in remote sensing applications



<div class="grid grid-cols-2 gap-5 mt-5 justify-center">
  <figure v-click="1" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/aerosol.jpg" alt="Image 1" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Aerosol in the atmosphere
      <div class="text-2">(Source: wikipedia.org)</div>
    </figcaption>
  </figure>
  
  <figure v-click="2" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/ocean_optics.jpg" alt="Image 2" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Ocean optics
      <div class="text-2">(Source: wikipedia.org)</div>
    </figcaption>
  </figure>
</div>


<div class="grid grid-cols-2 gap-5 mt-3 justify-center">
  <figure v-click="3" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/soil_moisture.jpg" alt="Image 1" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Soil moisture
      <div class="text-2">(Source: nasa.gov)</div>
    </figcaption>
  </figure>
  
  <figure v-click="4" class="flex flex-col items-center text-center">
    <div class="flex justify-center">
      <img src="/figures/cloud.jpg" alt="Image 2" class="w-3/4 h-auto">
    </div>
    <figcaption class="text-3 mt-2">
      Cloud composition
      <div class="text-2">(Source: unsplash.com)</div>
    </figcaption>
  </figure>
</div>


<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

-->

---
layout: default
---

## Macroscopic Maxwell Equations and LBM Framework

<div class="grid grid-cols-2 gap-6 mt-4">

  <!-- Left Column -->
<div class="pl-0">

<div class="text-4" >
<p class="text-lg mb-3">Maxwell's equations</p>

$$
\begin{alignedat}{3}
\nabla \cdot \mathbf{D} &= \rho 
&\quad\quad &
\nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\[1.2em]
\nabla \cdot \mathbf{B} &= 0
&\quad\quad &
\nabla \times \mathbf{H} &= \mathbf{J} + \frac{\partial \mathbf{D}}{\partial t}
\end{alignedat}
$$
</div>

<div v-click='1' class="text-4" >
<p class="mt-4 ">For linear media</p>
$$
\mathbf{D} = \varepsilon \mathbf{E}, \quad \mathbf{B} = \mu \mathbf{H}
$$
</div>

<div v-click='2' class="text-4" >
<p class="mt-4 ">Boundary conditions at the interface of two media</p>
$$
\begin{array}{cc}
\begin{aligned}
\hat{n} \cdot (\mathbf{D}_{2} - \mathbf{D}_{1}) &= \sigma \\[1.2em]
\hat{n} \times (\mathbf{E}_{2} - \mathbf{E}_{1}) &= 0
\end{aligned}
&
\begin{aligned}
\hat{n} \cdot (\mathbf{B}_{2} - \mathbf{B}_{1}) &= 0 \\[1.2em]
\hat{n} \times (\mathbf{H}_{2} - \mathbf{H}_{1}) &= \mathbf{K}
\end{aligned}
\end{array}
$$
</div>
</div>


<div class="pl-0">
  <!-- Right Column -->


<div v-click='3'>
<p class="text-lg mb-3">Lattice Boltzmann method</p>


<div class="relative w-full mt-0">

<div v-click='3' v-click.hide='7' absolute inset-0 >
<div >
<div class="flex justify-between items-center text-3.5 mt-2">
  <div class="text-center mr-15 ml-10">
    Post collision
  </div>
  <div class="text-center ml-15 mr-15">
    Pre collision
  </div>
</div>

<figure v-click='3' class="text-center item-center my-1">
  <img src="/figures/LBM_Kruger.png" alt="Image 1" class="h-auto">
</figure>



<div class="flex justify-between items-center text-2.75 mt--5">
<div v-click='4' class="text-center mx-0">
$$
f_i^* (\mathbf{r}, t) = f_i (\mathbf{r}, t) + \frac{\Delta t}{\tau} \left[f_i^{eq} (\mathbf{r}, t) - f_i (\mathbf{r}, t) \right]
$$
</div>
<div v-click='5' class="text-center mx-5">
$$
f_i (\mathbf{r} + \mathbf{c}_i \Delta t, t + \Delta t) = f_i^* (\mathbf{r}, t)
$$
</div>
</div>



<div v-click='6' class="text-3 text-left mt--2">
$$
{\bf e}_i^{eq} ({\bf r} ,t) = 
    \begin{cases}
      \frac{1}{6}\Big(\mathbf{E} ({\bf r} ,t) -   {\bf c}_i \times \mathbf{H} ({\bf r} ,t) \Big) & \text{if $i \neq 0$}\\
      (\varepsilon_{r} - 1 ) \mathbf{E} ({\bf r} ,t) & \text{if $i = 0$}
    \end{cases},  \\
    {\bf h}_i^{eq} ({\bf r} ,t) = 
    \begin{cases}
      \frac{1}{6}\Big(\mathbf{H} ({\bf r} ,t) +  {\bf c}_i \times \mathbf{E} ({\bf r} ,t) \Big) & \text{if $i \neq 0$}\\
      (\mu_{r} - 1 ) \mathbf{H} ({\bf r} ,t) & \text{if $i = 0$}
    \end{cases},  
$$
</div>



</div>
</div>


<div v-click="7" absolute inset-0  >
<figure class="text-center item-center">
  <video autoplay loop muted class="w-11/12 h-auto">
    <source src="/figures/lattice_boltzmann.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</figure>
</div>

</div>


</div>



<div class="flex justify-between items-center text-3.5 mt-2 abs-br mr-5 ">
  <div v-click='3' class="m-2 text-2.5">
    Timm Kruger (2017)
  </div>
  <div v-click='6' class="m-2 text-2.5">
    Hauser and Verhey (2017)
  </div>
  <div v-click='6' class="m-2 text-2.5">
    Khan et al. (2024)
  </div>
</div>



<div class="flex justify-between items-center text-3.5 mt-2 abs-bl mr-5 ">
  <div class="m-2 text-2.5">
    Griffiths (2013)
  </div>
</div>




</div>





<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

</div>

---

## Methods to solve Maxwell's equations

<table class="w-full border-collapse border text-center text-3.5 mt-5">
  <thead>
    <tr class="bg-gray-100">
      <th class="border px-3 py-2 text-center font-bold">Method Category</th>
      <th class="border px-3 py-2 text-center font-bold">Method</th>
      <th class="border px-3 py-2 text-center font-bold">Domain</th>
      <th class="border px-3 py-2 text-center font-bold">Applicable Shapes</th>
      <th class="border px-3 py-2 text-center font-bold">Challenges</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="border px-3 py-2" rowspan="2">Series expansion of basis function</td>
      <td class="border px-3 py-2">Mie</td>
      <td class="border px-3 py-2">Frequency domain</td>
      <td class="border px-3 py-2">Sphere, circular cylinder</td>
      <td class="border px-3 py-2"></td>
    </tr>
    <tr>
      <td class="border px-3 py-2">T-matrix</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Shapes with symmetries</td>
      <td class="border px-3 py-2"></td>
    </tr>
    <tr>
      <td class="border px-3 py-2" rowspan="2">Solves IE at grids</td>
      <td class="border px-3 py-2">DDA</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Arbitrary shape</td>
      <td class="border px-3 py-2">Size parameter 10 <div class="text-2" style="color: red"> Kahnert (2016) </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2">MoM</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Low accuracy <div class="text-2" style="color: red"> Mishchenko (2014) </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2" rowspan="2">Solves PDE at grids</td>
      <td class="border px-3 py-2">FEM</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Size parameter 10 <div class="text-2" style="color: red"> Mishchenko et. al (2000)  </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2">FDTD</td>
      <td class="border px-3 py-2">Time domain</td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">Size parameter 20 <div class="text-2" style="color: red"> Kahnert (2016)  </div> </td>
    </tr>
    <tr>
      <td class="border px-3 py-2" colspan="1">Solves particle populations at grids</td>
      <td class="border px-3 py-2"><span v-mark.circle.red="1">Lattice Boltzmann method</span></td>
      <td class="border px-3 py-2">''</td>
      <td class="border px-3 py-2">''</td>
    </tr>
  </tbody>
</table>

<v-drag pos="765,36,155,_">
<div class="text-3 ">
$$
\text{Size parameter}  = 2 \pi \frac{a}{\lambda}
$$
</div>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Normal Incidence at a Plane Wall

<div  class="text-center text-4 mb-1 mt-5">
  Permeability of the wall is fixed
</div>

<div class="grid grid-cols-2 gap-10 place-items-center">
  <figure class="text-center">
    <img src="/figures/JCP/Normal_Inc_E_er_20.svg" alt="Image 1" class="w-auto h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/JCP/Normal_Inc_H_er_20.svg" alt="Image 2" class="w-auto h-auto">
  </figure>
</div>

<div v-click="1" class="text-center text-4 mt-2 mb-1">
  Permittivity of the wall is fixed
</div>

<div v-click="1" class="grid grid-cols-2 gap-10 place-items-center mt-1">
  <figure class="text-center">
    <img src="/figures/JCP/Normal_Inc_E_mur_20.svg" alt="Image 3" class="w-auto h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/JCP/Normal_Inc_H_mur_20.svg" alt="Image 4" class="w-auto h-auto">
  </figure>
</div>




<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a circular cylinder

Considering size

<div class="text-center text-3 mb-0 mt-0">
  Perfect electric conductor
</div>

<div class="grid grid-cols-3 gap-0 place-items-center mb-0">
  <figure class="text-center">
    <img src="/figures/SW_PEC_Rayleigh.svg" alt="Image 1" class="w-7/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/SW_PEC_Mie.svg" alt="Image 2" class="w-7/8 h-auto">
  </figure>

  <figure class="text-center">
    <img src="/figures/SW_PEC_GO.svg" alt="Image 3" class="w-7/8 h-auto">
  </figure>
</div>

<div v-click="1" class="text-center text-3 mt-0 mb-0">
Dielectric constant
</div>





<div v-click="1" class="relative w-full mt-0">
 
  <div v-click="1" v-click.hide="2" class="absolute inset-0 grid grid-cols-3 gap-0 place-items-center transition-opacity duration-500 opacity-100">
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_0.02.svg" alt="Image 1" class="w-7/8 h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_0.1.svg" alt="Image 2" class="w-7/8 h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_1.0.svg" alt="Image 3" class="w-7/8 h-auto">
    </figure>
  </div>

  <!-- Second group of images -->
  <div v-click="2" class="absolute inset-0 grid grid-cols-2 gap-6 place-items-center transition-opacity duration-500 opacity-100">
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_10.0.svg" alt="Image 4" class="w-7/8 h-auto">
    </figure>
    <figure class="text-center">
      <img src="/figures/SW_polar_er_2_ratio_50.0.svg" alt="Image 5" class="w-7/8 h-auto">
    </figure>
  </div>
</div>








<v-drag pos="541,315,55,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 2
$$
</div>
</v-drag>

<v-drag pos="36,461,55,_">
<div v-click="1" v-click.hide="2"  class="text-3 text-left">
$$
\frac{a}{\lambda} = \frac{1}{50}
$$
</div>
</v-drag>

<v-drag pos="327,455,55,_">
<div v-click="1" v-click.hide="2" class="text-3 text-left">
$$
\frac{a}{\lambda} = \frac{1}{10}
$$
</div>
</v-drag>

<v-drag pos="76,441,55,_">
<div v-click="2" class="text-3 text-left">
$$
\frac{a}{\lambda} = 10
$$
</div>
</v-drag>


<v-drag pos="810,427,55,_">
<div v-click="2" class="text-3 text-left">
$$
\frac{a}{\lambda} = 50
$$
</div>
</v-drag>


<v-drag pos="862,464,55,_">
<div v-click="1" v-click.hide="2" class="text-3 text-left">
$$
\frac{a}{\lambda} = 1
$$
</div>
</v-drag>



<v-drag pos="773,29,160,_">
<div class="text-3 text-left">
$$
\sigma = \lim_{r \to \infty} 2 \pi r \frac{|\mathbf{E}^S|^2}{|\mathbf{E}^I|^2}
$$
</div>
</v-drag>






<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a circular cylinder

Considering size


<v-drag pos="402,106,171,_">
<div  class="text-3">
Perfect electric conductor
</div>
</v-drag>



<div class="grid grid-cols-3 gap-0 place-items-center my-0">
  <figure class="text-center">
    <img src="/figures/EzTot_PEC_Real_0.02.svg" alt="Image 1" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_PEC_Real_1.0.svg" alt="Image 2" class="w-full h-auto">
  </figure>

  <figure class="text-center">
    <img src="/figures/EzTot_PEC_Real_50.0.svg" alt="Image 3" class="w-full h-auto">
  </figure>
</div>

<div v-click="1" class="text-center text-3 mt-0 mb-0">
  Dielectric constant
</div>

<div v-click="1" class="grid grid-cols-3 gap-0 place-items-center my-0">
  <figure class="text-center">
    <img src="/figures/EzTot_er_2_Real_0.02.svg" alt="Image 4" class="w-full h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_er_2_Real_1.0.svg" alt="Image 5" class="w-full h-auto">
  </figure>

  <figure class="text-center">
    <img src="/figures/EzTot_er_2_Real_50.0.svg" alt="Image 6" class="w-full h-auto">
  </figure>
</div>

<v-drag pos="548,313,55,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 2
$$
</div>
</v-drag>

<v-drag pos="33,297,55,_">
<div class="text-2.5 text-left">
$$
\frac{a}{\lambda} = \frac{1}{50}
$$
</div>
</v-drag>

<v-drag pos="313,301,55,_">
<div class="text-2.5 text-left">
$$
\frac{a}{\lambda} = 1
$$
</div>
</v-drag>

<v-drag pos="869,300,55,_">
<div class="text-2.5 text-left">
$$
\frac{a}{\lambda} = 50
$$
</div>
</v-drag>




<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric circular cylinder

Considering dielectric constant

<div class="grid grid-cols-3 gap-0 place-items-center mt-10">
  <figure class="text-center">
    <img src="/figures/SW_er_5_1.svg" alt="Image 1" class="w-6/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/SW_er_10_1.svg" alt="Image 2" class="w-6/8 h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/SW_er_20_1.svg" alt="Image 2" class="w-6/8 h-auto">
  </figure>
</div>

<div v-click="1" class="grid grid-cols-3 gap-0 place-items-center mt-10">
  <figure class="text-center">
    <img src="/figures/EzTot_er_5_Real_1.svg" alt="Image 3" class="w-auto h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_er_10_Real_1.svg" alt="Image 4" class="w-auto h-auto">
  </figure>
  
  <figure class="text-center">
    <img src="/figures/EzTot_er_20_Real_1.svg" alt="Image 4" class="w-auto h-auto">
  </figure>
</div>



<v-drag pos="152,308,55,_">
<div class="text-3 text-left">
$$
\varepsilon_r = 5
$$
</div>
</v-drag>

<v-drag pos="442,314,55,_">
<div class="text-3 text-left">
$$
\varepsilon_r = 10
$$
</div>
</v-drag>

<v-drag pos="741,311,55,_">
<div class="text-3 text-left">
$$
\varepsilon_r = 20
$$
</div>
</v-drag>



<v-drag pos="773,29,160,_">
<div class="text-3 text-left">
$$
\sigma = \lim_{r \to \infty} 2 \pi r \frac{|\mathbf{E}^S|^2}{|\mathbf{E}^I|^2}
$$
</div>
</v-drag>




<v-drag pos="440,85,55,_">
<div  class="text-3 text-left">
$$
a / \lambda = 1
$$
</div>
</v-drag>

<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a regular hexagonal dielectric cylinder


<div class="relative w-full mt-10">



<div v-click.hide="2"  class="absolute inset-0 items-center justify-center">

  <div  class="grid grid-cols-3 mt-5 gap-2 place-items-center justify-center transition-opacity duration-500 opacity-100">
    <figure class="flex flex-col items-center">
      <img src="/figures/SW_TM_Hexgon_polar_er_1.721_ratio_0.1.svg" alt="Image 1" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/SW_TM_Hexgon_polar_er_1.721_ratio_1.svg" alt="Image 2" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/SW_TM_Hexgon_polar_er_1.721_ratio_10.svg" alt="Image 3" class="w-7/8 h-auto">
    </figure>
  </div>
  <div v-click="1"  class="grid grid-cols-3 mt-10 gap-2 place-items-center justify-center transition-opacity duration-500 opacity-100">
      <figure class="flex flex-col items-center">
        <img src="/figures/SW_TE_Hexgon_polar_er_1.721_ratio_0.1.svg" alt="Image 4" class="w-7/8 h-auto">
      </figure>
      <figure class="flex flex-col items-center">
        <img src="/figures/SW_TE_Hexgon_polar_er_1.721_ratio_1.svg" alt="Image 5" class="w-7/8 h-auto">
      </figure>
      <figure class="flex flex-col items-center">
        <img src="/figures/SW_TE_Hexgon_polar_er_1.721_ratio_10.svg" alt="Image 5" class="w-7/8 h-auto">
      </figure>
  </div>
  
</div>





<div v-click="2"
       class="absolute inset-0 grid grid-cols-3 gap-2 mt-15 place-items-center justify-center transition-opacity duration-500 opacity-100">
    <figure class="flex flex-col items-center">
      <img src="/figures/Ez_Hexagon_TM_Tot_er_1.721_Real_0.1.svg" alt="Final 1" class="w-full h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/Ez_Hexagon_TM_Tot_er_1.721_Real_1.svg" alt="Final 2" class="w-full h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/Ez_Hexagon_TM_Tot_er_1.721_Real_10.svg" alt="Final 3" class="w-full h-auto">
    </figure>
</div>

</div>


<v-drag pos="-28,197,137,_,270">
<div class="text-3 text-left">
$$
TM^z \text{polarization}
$$
</div>
</v-drag>

<v-drag pos="-29,417,137,_,270">
<div v-click="1" v-click.hide="2"  class="text-3 text-left">
$$
TE^z \text{polarization}
$$
</div>
</v-drag>


<v-drag pos="442,73,90,_">
<div class="text-3 text-left">
$$
a/\lambda = 1
$$
</div>
</v-drag>


<v-drag pos="737,76,90,_">
<div class="text-3 text-left">
$$
a/\lambda = 10
$$
</div>
</v-drag>


<v-drag pos="153,75,90,_">
<div class="text-3 text-left">
$$
a/\lambda = 1/10
$$
</div>
</v-drag>


<v-drag pos="848,47,90,_">
<div class="text-3 text-left">
$$
\varepsilon_r = 1.721
$$
</div>
</v-drag>



<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric sphere


<div class="relative flex flex-col items-center justify-center mt-10">

<figure v-click.hide="1" class="flex flex-col items-center">
  <img src="/figures/3D_schematic.png" alt="Main Figure" class="w-1/2 h-auto">
</figure>

<div v-click="1" class="absolute inset-0 flex flex-col items-center justify-center">
  <div class="grid grid-cols-3 gap-10 place-items-center justify-center transition-opacity duration-500 opacity-100">
    <figure class="flex flex-col items-center">
      <img src="/figures/RCS_Polar_0.02_2_90.svg" alt="Image 1" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/RCS_Polar_0.1_2_90.svg" alt="Image 2" class="w-7/8 h-auto">
    </figure>
    <figure class="flex flex-col items-center">
      <img src="/figures/RCS_Polar_1_2_90.svg" alt="Image 3" class="w-7/8 h-auto">
    </figure>
    <div class="col-span-3 flex justify-center gap-10 transition-opacity duration-500 opacity-100">
      <figure class="flex flex-col items-center">
        <img src="/figures/RCS_Polar_2_2_90.svg" alt="Image 4" class="w-7/8 h-auto">
      </figure>
      <figure class="flex flex-col items-center">
        <img src="/figures/RCS_Polar_5_2_90.svg" alt="Image 5" class="w-7/8 h-auto">
      </figure>
    </div>
  </div>
</div>

</div>


<v-drag pos="647,20,90,_">
<div v-click="1"  class="text-3 text-left">
$$
\varepsilon_r = 2
$$
</div>
</v-drag>


<v-drag pos="184,75,91,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1/50
$$
</div>
</v-drag>

<v-drag pos="442,75,90,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1/10
$$
</div>
</v-drag>

<v-drag pos="717,75,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 1
$$
</div>
</v-drag>

<v-drag pos="332,302,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 2
$$
</div>
</v-drag>

<v-drag pos="587,306,55,_">
<div v-click="1"  class="text-3 text-left">
$$
a / \lambda = 5
$$
</div>
</v-drag>



<v-drag pos="794,12,160,_">
<div v-click="1"  class="text-3 text-left">
$$
\sigma_{3D} = \lim_{r \to \infty} 4 \pi r^2 \frac{|\mathbf{E}^S|^2}{|\mathbf{E}^I|^2}
$$
</div>
</v-drag>




<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>

---

## Scattering from a dielectric sphere



<div  class="grid grid-cols-2 gap-5 place-items-center justify-center mt-10 my-15">
  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_0.02.svg" alt="Image 1" class="w-full h-auto">
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_0.1.svg" alt="Image 2" class="w-full h-auto">
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_1.svg" alt="Image 3" class="w-full h-auto">
  </figure>

  <figure class="flex flex-col items-center">
    <img src="/figures/sphere_er_2_ratio_5.svg" alt="Image 4" class="w-full h-auto">
  </figure>
</div>



<v-drag pos="53,177,84,_">
<div class="text-3 text-left">
$$
a / \lambda = 1/50
$$
</div>
</v-drag>

<v-drag pos="519,182,80,_">
<div class="text-3 text-left">
$$
a / \lambda = 1/10
$$
</div>
</v-drag>

<v-drag pos="71,359,60,_">
<div  class="text-3 text-left">
$$
a / \lambda = 1
$$
</div>
</v-drag>

<v-drag pos="524,381,59,_">
<div class="text-3 text-left">
$$
a / \lambda = 5
$$
</div>
</v-drag>



<div class="abs-br m-2 text-3">
  <SlideCurrentNo />
</div>


---

# Thank You!

<div class="grid grid-cols-2 gap-12 items-center mt-10">

  <!-- LEFT: Advisor photos (small) -->
<div class="flex flex-row justify-center space-x-12">


<figure class="text-center">
  <img src="/figures/Anubhab.jpg" class="w-auto h-32 shadow-md" />
  <figcaption class="text-sm mt-2 opacity-80">
    Prof. Anubhab Roy
  </figcaption>
</figure>

<figure class="text-center">
  <img src="/figures/sumesh.jpeg" class="w-auto h-32 shadow-md" />
  <figcaption class="text-sm mt-2 opacity-80">
    Prof. Sumesh P. Thampi
  </figcaption>
</figure>



</div>

  <!-- RIGHT: Big QR Code -->
  <div class="flex flex-col items-center">
    <img src="/figures/QR_github.png" class="w-7/8 h-auto shadow-xl" />
    <p class="text-base opacity-80 text-center mt-4">
      Scan for code and preprint
    </p>
  </div>

</div>





<div class="flex justify-between items-center text-3.5 mt-2 abs-br mr-5 ">
  <div class="m-2 text-2.5">
    Khan et al. (2024)
  </div>
  <div class="m-2 text-2.5">
    Khan et al. (2025)
  </div>
  <div class="m-2 text-2.5">
    Khan et al. (2025)
  </div>
</div>
