# simulation_bacteria_growth

In this project, I developed a simulation to model the growth and diffusion of bacteria in a 2D grid environment, coupled with food consumption. I incorporated several adjustable parameters to observe their effects on bacterial growth, diffusion, and food dynamics. Below is a detailed breakdown of the main components I implemented:
<br><br>
1. **BacteriaGrowthSimulation Class**: This class is the heart of my project, and here's what I integrated within it:
  <br><br>
   - I initialized the grids for both bacteria and food.<br>
   
   - My `update` method serves as the core of the simulation. Here, I put forth the rules governing food growth, its reseeding, diffusion mechanisms, bacteria's food consumption, and the bacteria's own diffusion.<br>
   
   - To visualize the progress, I added the `observe_bacteria` and `observe_food` methods. They allow me to keep an eye on the bacterial and food states, respectively.<br><br>

2. **make_animation Function**: With a keen interest in visual representation, I crafted this function to animate the bacterial growth simulation over time. I employed the `FuncAnimation` from `matplotlib.animation` to make this come alive: <br> <img width="614" alt="Screenshot 2023-10-18 at 2 19 26 PM" src="https://github.com/miraslavats/simulation_bacteria_growth/assets/112869592/68162477-ba99-4189-8fcf-d5424ed5c7ea"><br><br>

3. **plot_average_population Function**: I graphed the average populations of bacteria and food over a predetermined number of steps. This visual representation lets me see the fluctuations in populations over time: <br> <img width="586" alt="Screenshot 2023-10-18 at 2 14 56 PM" src="https://github.com/miraslavats/simulation_bacteria_growth/assets/112869592/c1f1754c-09f2-4930-939a-d6bf9890f7f6"><br><br>

4. **Varying Parameters Function**: To dive deeper into understanding parameter influences, I've designed a function (although not fully provided here) that allows for the alteration of a single parameter across a specific range, while other parameters remain constant. It's particularly useful for a sensitivity analysis: <br> <img width="976" alt="Screenshot 2023-10-18 at 2 22 26 PM" src="https://github.com/miraslavats/simulation_bacteria_growth/assets/112869592/97ba1285-483a-45ba-9d8e-1ae3ce6be678">
<br>

## Key Features I Observed:
<br><br>
1. **Growth & Consumption**: I noticed that bacteria thrive by consuming food. The availability and consumption of this food directly influences the bacterial proliferation. <br>

2. **Food Growth**: I designed the food to follow a logistic growth pattern, hitting a ceiling at its carrying capacity.<br>

3. **Reseeding**: Every so often, I made sure to introduce new food into random cells.<br>

4. **Diffusion**: I introduced a diffusion mechanism for both the food and bacteria, facilitating their dispersion across the grid.<br>

5. **Bacteria Reproduction & Death**: Starving bacteria meet their demise in my simulation, whereas those that have ample food get to reproduce.<br>

<br><br> To wrap it up, this project offers a holistic simulation of bacterial proliferation in 2D. By tweaking the parameters, I can witness varied behaviors and pinpoint the major factors propelling bacterial growth and food consumption. For me, it underscores the power of computational methods in decoding intricate systems.
