Scripts for 2018 paired eDNA/Beach Seine data
Note: all scripts must be run independantly (i.e., restart to clear environment and packages loaded)

10_species_detections_compared:
	Format data to compare read abundance and biomass and biomass densities
		
	IN:		bs_long.rds
			eDNA_long.rds
			BS_taxonomy_reconciled.rds
			eDNA_taxonomy_reconciled.rds
	OUT: 	data:	shared_long.rds
			plots:	
				biomass x reads for each species  
				biomassDensity x reads for each species
				biomass of each observation for each species
				rank biomass and eDNA detection errors
			tables:  
			LCT_table.csv - annotate this with higher/shared taxonomy, merge with error table
			
11_Trees:
	Build a dendrogram from higher taxonomy and colour code by method. 
	Plot frequency of positive detections by method.

12_richness_analyses:
	Plot differences in richnes. run models to predict differences in richness
	IN:		long_shared.rds
			environmental.rds
	OUT:	rich x rich.png; richdiff.png: richdiffdensity.png - combine in powerpoint
			
			sample schedule plot
	
	Thinking of taking a different approach here. As these data contain many repeat samples we need to account for this in the model. (Longitudinal data)
	We cannot use mixed models because of small sample size and few within group observations.
			"GEE extends the GLM likelihood analysis to incorporate a (within group) correlation structure. There are different (plausible) 
			correlation structures: independence, exchangeable, autoregressive, etc. for different scenarios. 
			The correlation structure is estimated by averaging on the Pearson's residuals. The estimation is done in an 
			iterative way - estimate the coefficients, then the correlations, rinse-repeat."
	Generalized Estimating Equations:
		- assume some correlation between grouped observations
		- quasi-liklihood
		- don't specify distribution of y
		- specify mean-variance structure and dispersion parameter
		- addition: add a correlation structure to likelihood equations
			- if we ignore we underestimate between-group SD and overestimate within-group SD   -  SE are not reliable
		- need to estimate correlation structure, but need the betas to do this
				- estimate betas using GLM, then estimate correlation structure (alphas)
				- estimate betas again using correlation structure and then new correlation structure again - repeat until parameters don't change

13_betadiver_analyses


16_patchiness 
	summarize spatial data of vegetation and exposure. Plot density-histogram showing difference in scales of patchiness.

Citations

# Hardin, J.W. and Hilbe, J.M. (2012). Generalized Estimating Equations, 2nd Edition, Chapman and Hall/CRC: New York.
# Liang KY, Zeger SL. Longitudinal data analysis using generalized linear models. Biometrika. 1986;73:13–22.



	