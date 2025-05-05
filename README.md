# ce295-hw-5-optimal-phev-energy-management-via-dynamic-programming-solved
**TO GET THIS SOLUTION VISIT:** [CE295 HW 5-Optimal PHEV Energy Management via Dynamic Programming Solved](https://www.ankitcodinghub.com/product/ce295-hw-5-optimal-phev-energy-management-via-dynamic-programming-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95660&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CE295 HW 5-Optimal PHEV Energy Management via Dynamic Programming Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

This assignment will provide hands-on practice for dynamic programming (DP) with application to energy management in plug-in hybrid electric vehicles (PHEVs). PHEVs are microgrids on wheels. Namely, their powertrains (i.e. power systems) include a local generator (internal combustion engine), energy storage (the battery), and local power demand (from the driver’s right foot). The goal is to manage energy flows to minimize fuel consumption.

Reading

The following readings are intended to provided context and background for this homework assignment.

• “Hybrid and Electrified Vehicles: The Role of Dynamics and Control” by Rizzoni and Peng.

• “Smart, Connected &amp; Electric: The Future of the Automobile” by Phillips, McGee, Kristinsson, &amp; Yu.

Problem Data

<ul>
<li>You will optimize for the Urban Dynamic Driving Schedule (UDDS) power demand, provided in bCourses.</li>
<li>Minimize total fuel consumption J = 􏰋N−1 α∆t Pfuel(k). k=0</li>
<li>Engine power is given by Peng(k) = η(Peng(k)) · Pfuel(k), where η(·) is the engine efficiency as a function of power demand. This function is computed by eta_eng (a separate .m file in Matlab and integrated directly in the iPython Notebook).</li>
<li>The battery dynamics are given by: SOC(k + 1) = SOC(k) − ∆t Pbatt(k) Qcap Voc</li>
<li>The battery SOC, battery power, and engine power are limited according to:</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
Formulate

</div>
</div>
<div class="layoutArea">
<div class="column">
Problem 1: Formulate an optimization problem. Provide the following: Page 1 of 4

</div>
</div>
<div class="layoutArea">
<div class="column">
SOCmin ≤ SOC(k) ≤ SOCmax −Pmax ≤ P (k) ≤ Pmax

</div>
</div>
<div class="layoutArea">
<div class="column">
batt batt batt

</div>
</div>
<div class="layoutArea">
<div class="column">
0 ≤ P (k) ≤ Pmax eng eng

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ol>
<li>(a) &nbsp;Write down the objective function.</li>
<li>(b) &nbsp;Write down ALL the constraints, after eliminating the variable Peng(k) as done in lecture. Label the physical meaning of each constraint.</li>
<li>(c) &nbsp;What is the control variable? What is the state variable?</li>
</ol>
Problem 2:

(a) Define – in words – an appropriate value function, as done in lecture and the CH 5 notes. (b) Write down the principle of optimality equation and boundary condition.

Problem 3: This problem assists you to write the code. You should have formulated three pairs of upper/lower limits, i.e. inequalities.

<ol>
<li>(a) &nbsp;Re-arrange each pair as upper/lower limits on Pbatt(k).</li>
<li>(b) &nbsp;Clearly, one of the lower limits and one of the upper limits will dominate the others, at each time step. Collapse the three pairs into the form: max{·, ·, ·} ≤ Pbatt(k) ≤ min{·, ·, ·}. This produces simple bounds on Pbatt(k), for each time step. This will greatly assist our coding of the principle of optimality.</li>
</ol>
Data

Problem 4: Download the files { HW5_Skeleton.m, UDDS_Pdem.csv. eta_eng.m } for Matlab or {HW5_Skeleton.ipynb, UDDS_Pdem.csv } for Python from bCourses. The data file UDDS_Pdem.csv contains vectors t, v_dc, P_dem,

which respectively give the time [sec], drive cycle speed [m/s], and corresponding power demand [kW].

<ol>
<li>(a) &nbsp;In one figure, create two subplots. The top subplot plots the UDDS speed vs. time. The bottom subplot includes power demand vs. time. Use appropriate line styles, axis labels, font sizes, etc. Include the figure in your report.</li>
<li>(b) &nbsp;In a second figure, plot the engine efficiency curve: Peng on the x-axis versus η(Peng) on the y-axis.</li>
</ol>
Code

Problem 5: For all the following subproblems, you may include the entire code in your report.

<ol>
<li>(a) &nbsp;Encode the value function’s boundary condition in the skeleton code.</li>
<li>(b) &nbsp;For each time-step and each state in the SOC grid, find the lower/upper bounds for Pbatt(k). Use these bounds to create a grid of feasible Pbatt values.</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
(c) Implement the recursive principle of optimality equation in your code. This includes (i) the cost- per-time-step calculation, (ii) computing SOC(k + 1), and (iii) interpolation of Vk+1(SOC(k + 1)). Interpolation is necessary because Vk is defined on the SOC grid, and SOC(k + 1) will never fall exactly on a grid-point. Therefore we interpolate between grid points to find Vk+1(SOC(k + 1)). The key idea is that the sub-optimization is done by griding Pbatt and selecting the value which minimizes the min operator’s argument.

Problem 6: Simulate optimal energy management results. Provide the code and plots in your report.

<ol>
<li>(a) &nbsp;Suppose the initial SOC is 0.75. Write a for loop that simulates the discrete-time battery dynamics,
using the optimal battery power P∗ (k). This includes (i) interpolating P∗ (k) over the SOC grid, batt batt

(ii) computing the accumulated fuel consumption, and (iii) the SOC dynamics.
</li>
<li>(b) &nbsp;What is the minimum fuel consumption?</li>
<li>(c) &nbsp;Create a figure with four subplots, using appropriate line-styles, axis labels, and legends:
• [Subplot 1] UDDS speed versus time.

• [Subplot 2] SOC versus time

• [Subplot 3] Accumulated fuel consumption [g] versus time. • [Subplot 4] Battery and engine power [kW] versus time.
</li>
<li>(d) &nbsp;Are all the inequality constraints satisfied?</li>
</ol>
Additional Analysis

Problem 7: Note that DP computes the optimal energy management strategy for all possible initial SOC values. Use this fact to complete Table 1.

Table 1: PHEV Energy Management Results

</div>
</div>
<div class="layoutArea">
<div class="column">
Initial SOC

0.9 0.75 0.6 0.45 0.3

</div>
<div class="column">
Final SOC

</div>
<div class="column">
Total Fuel Cons. [kg]

</div>
</div>
<div class="layoutArea">
<div class="column">
Problem 8: Comment on the SOC and engine power trajectories. As the initial SOC decreases, how does the SOC trajectory change? How does the total fuel consumption change? Explain why.

Deliverables

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Submit the following on bCourses. Be sure that the function files are named exactly as specified (including spelling and case). Please do NOT zip files.

LASTNAME_FIRSTNAME_HW5.PDF

LASTNAME_FIRSTNAME_HW5.xyz which contains your respective Matlab or Python files, i.e. xyz ∈ {m, ipynb}.

Remark

In Spring 2015, two students modified this homework slightly for application to solar generation and storage, and launched energy analytics start-up eLum &lt;http://elum-energy.com/&gt;. They received a number of investments, and are now selling software to deploy microgrid technologies in Africa.

In Fall 2018, one student combined HW5 and HW3 in a presentation as part of a job interview at Siemens’s power system division. Siemens was very impressed, and offered the student a lucrative full-time position.

</div>
</div>
<div class="layoutArea">
<div class="column">
Perhaps a story like this is in your future.

</div>
</div>
<div class="layoutArea">
<div class="column">
Page 4 of 4

</div>
</div>
</div>
