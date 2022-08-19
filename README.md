# Data Model
### *Columns included in the stripped sample are marked with :star:*

|Name    |Type |Units |Description |
|    :---:    |--- |--- |---|
|***Identifiers***| | | |
|`objname`:star:| | | Common galaxy name|
|`pgc`        | | |PGC number (from HyperLeda)|
|`nsa_id`| | |NASA-Sloan Atlas NSAID number|
|`group_id`| | |Galaxy is member of group, number based on Lambert et al. 2020 group catalog|
|`ra`:star:| | |Right Ascension|
|`dec`:star:| | |Declination|
|`d25`| | |Apparent Diameter from Karachentsev and HyperLeda|
|`v_h`:star:| | |Heliocentric Radial, see Section 4.1|
|`v_cmb`| | |Radial velocity with respect to CMB radiation|
|`v_source`| | |Original source for compiled velocity, list options|
|`hl_obj`| | |True for objects in HyperLeda|
|`chandra_limit`| | |"True" if CSCView crossmatch returned a limiting sensitivity|
|`chandra_detection`| | |"True" if CSCView crossmatch returned flux information as described in Section 7|
|`lvg_obj`| | |True for objects in Karachentsev's Catalog of Local Volume Galaxies|
|`nsa_obj`| | |True for objects in NASA-Sloan Atlas|
|`sga_obj`| | |True for objects in Sienna Galaxy Atlas|
|***Morphology***|- |- |***Section 6***|
|`t_type`:star:| | |Numerical Hubble T-Type|
|`color_type`| | |Color-based Type|
|`best_type`:star:| | |Combined galaxy type|
|***Photometry***|- |- |***Section 3**|
|`a_B_leda`| | |B-band extinction from Hyperleda multiplied by 0.86 to translate to Schlafly, A_V=0.769*a_B_leda and A_R=0.629*a_B_leda|
|`a_g_nsa`| | |g-band extinction from NASA-Sloan Atlas, the i-band extinction used is = 0.550 a_g_nsa|
|`EBV_irsa`| | |E(B-V) value from IRSA dust website Schlafly values for all galaxies.  Used only for the Siena Galaxy Atlas sources, A_g/EBV_sga=3.303, A_r/EBV_sga=2.285.|
|`Bt0_leda`| | |Extinction corrected total B band magnitude from HyperLeda|
|`BV_color_leda`| | |(B-V) color from HyperLeda — maybe make this one the final Hyperleda value|
|`B_lum`| | |B-band Luminosity — derived for non-Hyperleda sources as described in Section 3.2|
|`gi_color_nsa`| | |Extinction corrected (g-i) color from NASA-Sloan Atlas|
|`i_lum_nsa`| | |i-Band Luminosity, calculated using M_i_sun=XXX|
|`gr_color_sga`| | |Extinction corrected (g-r) color from Sienna Galaxy Atlas|
|`r_lum_sga`| | |r-band Luminosity, calculated using M_r_sun=XXX|
|`BR_color_ned`| | |Extinction corrected (B-R) color from NED|
|`R_lum_ned`| | |R-band Luminosity from NED, calculated using M_R_sun=XXX|
|`BMag`| | |Estimated absolute B-Band Magnitude for all galaxies|
|`gi_color`| | |Estimated g-i color for all galaxies with color measurements.|
|***Distance***|- |- |***Section 4***|
|`cf3_dist`| | |Distances from CosmicFlows3 Calculator|
|`cf3_dist_error`| | |Error on cf3_dist|
|`zind_dist`| | |Redshift independent distances|
|`zind_dist_error`| | |Error on zind_dist|
|`zind_indicator`| | |Use name as in NEDD, NEDD methods|
|`bestdist`:star:   | | |Our chosen best distance estimate|
|`bestdist_error`:star: | | |error for best distance estimate|
|`bestdist_method` | | |General method used for best distances, list|
|`bestdist_source` | | |Source/Reference for bestdist, see Section 4|
|***Mass***|- |- |***Section 5***|
|`logmass_gi`| | |log(Mstar) from (g-i)|
|`logmass_gr`| | |log(Mstar) from (g-r)|
|`logmass_BV`| | |log(Mstar) from (B-V)|
|`logmass_BR`| | |log(Mstar) from (B-R)|
|`logmass`:star:    | | |Compiled best Log(mass) estimate|
|`logmass_error`:star:| | |Error on logmass|
|`logmass_src`:star:| | |Color used for best mass estimate, list options|
