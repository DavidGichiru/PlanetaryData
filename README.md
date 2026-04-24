

# EXOPLANET HABITABILITY ANALYSIS:

This is an exploratory analysis of 4575 exoplanets from the NASA Exoplanet Archive (2021)
The dataset has 4575 rows and 23 columns, plus a header meaning it roughly has aboout 4575 exoplanets.

QUESTIONS:

- Do heavier stars produce heavier planets?
  
- Investigating this question, I wanted to understand whether stellar mass is a determinant in the mass of planets orbiting a particular star.
- After cleaning and visualization, I discovered the following;
  
  * The correlation between stellar mass and planet mass is 0.3, a moderate correlation which implies   that stellar mass is not the sole determinant of a planet mass. However the correlation proves that massive stars tend to host massive planets. The correlation itself does not show strong         
relationship between stellar and planet mass but its enough to prove the nebular formation theory        (Planets form from the same materials making up their parent star.)

-Does star metallicity determine the number of planets a particular star will host?

Metallicity (how rich a star composition is) is likely to affect the number of planets formed in that; high metallicity means a particular planet was formed from rich nebula clouds, meaning more heavy elements are available, more rocky materials to clump hence more planets.
I wanted to verify this hypothesis using the theory. The following is what i found out:
  * The correlation between the two variables was negative (-0.108) which means the relationship is basically flat. This comes down to what Kepler could see, meaning it was a discovery bias, and not atrributed to actual astrophysical relationship.

- Can I confirm Kepler's Third law using the dataset?

The law states that the square of a planet's Orbital period is proportional to the cube of  it's distance from the parent star.
Upon analysis, I found out the foloowimg:
  * The correlation between semi major axis and period days is 0.995, which implies a very strong relationship. I expected the slope to be 1.5 or approximately close, but it turned out to be o.677. Why? This is due to the plotting, whereby i interchanged the variables for x-axis and y-axis, but confirmed the inverse of the law, which is 2/3 thus giving a slope of 0.677.

- What is the effect of multi-planet systems on their individual planets' orbital paths?

  Hypothesis is that in multi-planet systems,planets stabilize their companions orbits over long periods of time, and therefore their orbits tend to be less eccentric.
  
-Can I confirm this hypothesis?

Upon analysis here is what I found out:
 *Generally, as planet systems grow larger, the average eccentricity of their orbits decrease. This is consistent with the gravitational stabilization thoery. However, 2 planet system planets, had higher eccentricity than single planet system. This is because if the two planets are not in resonance, it will result into them destabilizing eacg other, thus higher eccentricity in their orbits.

 -Which Planets shows signs of hosting life?
 Using various factors ( stellar temperature, semi major axis, eccentricity, stellar mass), I could filter out planets that could host life using Earth's values as the reference. 
 After analysis the results from my custom Habitability index, I found out the following:
   * HDD 28185 b ranks first, followed by Kepler 22 b, which was announced by NASA as a candidate that could possibly host life.

Generally these variables mattered the most: Stellar mass, Stellar effective temperature, Planet mass, Eccentricity, Semi-Major axis, Orbital Periods.

##TOOLS USED:
PYTHON, MATPLOTLIB, NUMPY, PANDAS, SCIPY, JUPYTER NOTEBOOK











  
