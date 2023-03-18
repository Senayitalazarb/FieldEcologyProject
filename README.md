
<div style="text-align: center;">
                      <h1 style="text-align:justify; font-size:24px;">Predation Rates between Cryptic and Aposematic Strategies</h1>
                                    <h2 style="text-align:center;font-size:10px">using artificial caterpillars</h2>

This note discusses the importance of caterpillars in the food chain and their vulnerability to predation. Caterpillars adopt different defense strategies such as cryptic, mimicry, and aposematism to protect themselves from predators. The `cinnabar moth` caterpillar is an example of a caterpillar that uses aposematism to signal toxicity and camouflage to avoid predation. The effectiveness of these defense strategies can be measured by studying the predation rates of predators using artificial caterpillar models. 

In this study, we used AC in four different areas of Freiburg(Germany) to test the following hypothesis: `(1) The predation rates of the cryptic and aposematic caterpillars are the same (null hypothesis) or significantly different (alternative hypothesis`) and `(2) The color types of plant where these dummy caterpillars are installed have no effect (null hypothesis) or have a significant effect on the predation (alternative hypothesis)`


## Method Adapted
--------

The objective of the conducted research was to investigate how caterpillar coloration and their surroundings determine the risk of being preyed upon. The study took place in four randomly selected locations in Freiburg im Breisgau, Germany. Non-hardening plasticine was used to create two types of caterpillars: pure green and yellow with black stripes. These artificial caterpillars (AC) were positioned on two different types of plants: Rockrose Polygala (RP) and any green plant (GP) without flowers. The distance between the plants with the AC was at least 4m. After 72 hours, the AC were gathered and analyzed for signs of predation. The study found that the yellow and black striped caterpillars were more susceptible to predation, and their predation rate was significantly influenced by their surroundings. 

<p align="center">
  <img src="Freiburg_map.png" alt="Uni_freiburg">
</p>


### Statistical Analysis
--------

The color values were obtained by extracting the RGB values of the caterpillar and plant background using ImageJ® software. These values were then transformed into HSV values using the matplotlib.colors.rgb_to_hsv function in Python. This facilitated the testing of hypotheses that examined the impact of color and color contrast on predation risk through statistical methods such as `General Linear Mixed Models (GLMM)` and` Chi-square`. The incorporation of the site variable as a random effect in the GLMM accounted for the differences between locations. The study provided valuable insights into the factors that determine predation risk in caterpillars by analyzing the effects of COLOR_caterpillar, plant_color, and CONTRAST as fixed effects.

<p align="center">
  <img src="Color_analysis.png" alt="Color_analysis">
</p>


### Experimental Design!
--------

- Hypothesis 1:  P(predated | aposematic) = P(predated | cryptic)
- Hypothesis 2:  P(predation) ⊥ plant 

<p align="center">
  <img src="design.png" alt="design">
</p>


### Main Findings
--------
Two hypotheses were tested in the study:

- The first hypothesis aimed to determine whether the predation rates of cryptic and aposematic caterpillars were significantly different or not. The results showed that the null hypothesis (i.e., the predation rates are the same) was rejected in favor of the alternative hypothesis (i.e., the predation rates are significantly different). However, further analysis revealed that the green caterpillars, which were assumed to be cryptic, were not actually cryptic based on the color analysis.

- The second hypothesis investigated whether the color types of the plants where the dummy caterpillars were installed had any effect on predation rates. The initial analysis using model 1, which included yellow and green background colors, failed to reject the null hypothesis (i.e., no significant effect). However, a subsequent color analysis and model 2 showed that the contrast between the colors of the caterpillars and the background had a significant effect on predation rates.

- From the color analysis we can see that the higher the contrast between the caterpillars and the background, the higher the predation risk The high contrast group here in the study were the green caterpillars.

### Drawbacks
--------

- Easier to spot predation on green caterpillars suggests that the observer may be biased towards detecting predation on green caterpillars compared to other caterpillar colors. This could be due to the material for making the green caterpillar was with a high contrast.

- Possible confounding factors that need to be controlled for include: seasonality, field site properties, human influence, weather conditions, and distribution of samples per field site.

### Further Fesearch
--------

- To minimize the impact of confounding factors, appropriate sampling methods and statistical analyses should be used.


### Requirements
--------

To run the code and reproduce the analysis, the following software and packages are required:

- [Python 3.x](https://www.python.org/)
- [Pandas](http://pandas.pydata.org/) > 1.4.2
- [NumPy](http://www.numpy.org/)
- [Matplotlib](http://matplotlib.org/)



## Author
This project was created by Senayit Berhane. For questions or feedback, please contact senayita.hac@gmail.com
</div>



