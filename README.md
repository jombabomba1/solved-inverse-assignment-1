Download Link: https://assignmentchef.com/product/solved-inverse-assignment-1
<br>
<h1>Linear Tomography</h1>

We shall analyze first-arrivals of seismic waves from two earthquakes, recorded by 10 seismographs at the earth’s surface. We will consider a 13 × 11 km vertical cross section of the subsurface, located immediately below the seismographs.

Figure 1: The geometry of the problem. 10 seismographs (black squares) are deployed on a line with a 1 kilometer spacing. Rays from 2 earthquakes hit the seismographs with an angle of incidence of 45 degrees. Rays from earthquake 1 come “from left”, and rays from earthquake 2 come “from right”.

<strong>The direct problem (the forward problem)</strong>

Let us simplify the problem by assuming a homogeneous earth outside the considered 13×11 km area, with a seismic wave propagation velocity of <em>v </em>= 5000 m/s. Inside the area, the wave propagation velocity is also 5000 m/s, except in the central, rectangular zone (grey on the figure), where the velocity is 5200 m/s. The presence of the grey zone introduces an arrivaltime anomaly (a deviation of the arrival time from a situation where the entire 13×11 km area is homogeneous with wave propagation velocity 5000 m/s, that is, without the grey zone). The arrival-time anomaly <em>t<sub>γ </sub></em>for a wave propagating along a ray <em>γ</em>, is given by

Z

<em>t<sub>γ </sub></em>=         <em>s</em>(<em>u</em>)<em>du                                                   </em>(1)

<em>γ</em>

where <em>s</em>(<em>u</em>) is the slowness anomaly (the anomaly of the reciprocal velocity) along the ray, and <em>u </em>is a parameter determining the point we consider on the ray. In the following we will assume that all rays are straight lines (and hence independent of the velocity field) as shown on the figure. This assumption is reasonable when the velocity variations in the subsurface are small.

<ol>

 <li>Calculate arrival-time anomalies for each of the 10 seismographs, for each of the earthquakes.</li>

 <li>Discretize Equation (1), e.g., by subdividing the area in the figure in 13 × 11 squares of 1 by 1 km.</li>

</ol>

<strong>The inverse problem</strong>

We will here simulate the observed data vector <strong>t</strong><em><sup>obs </sup></em>by adding a noise vector <strong>n </strong>to the “pure” data vector, calculated in question 1:

<table width="643">

 <tbody>

  <tr>

   <td width="623"><strong>t</strong><em>obs </em>= <strong>t</strong><em>pure </em>+ <strong>n</strong>where <strong>n </strong>has independent, normal distributed components with mean value 0 s and</td>

   <td width="20">(2)</td>

  </tr>

 </tbody>

</table>

<em> .                                              </em>(3)

Subscript “2” after the norm symbol means that it is the usual “Euclidian” 2-norm. We wish to simulate that the unknowns are the 13×11 slowness anomaly values in the area. These values are arranged in one long vector <strong>s</strong>, to be estimated from the ”observed” arrival-time anomalies <strong>t</strong><em>obs</em>.

<ol start="3">

 <li>Formulate the discrete inverse problem.</li>

 <li>Show that the problem is linear.</li>

 <li>Determine if the solution to the problem is unique or not, by looking at the relationbetween data and model.</li>

 <li>Find a solution to the problem using the <em>Tikhonov Regularization</em>. The solution must be physically acceptable, give the best possible resolution of the model, but, at the same time, “barely fit the data within the noise”.</li>

 <li>Describe how well the model is resolved by the inverse operator. Plot for instance how adelta function (zero everywhere, except in a single 1 × 1 km square) in the true model is reconstructed in the estimated model.</li>

 <li>Discuss the differences between your solution and the true model.</li>

</ol>