# Data Model
### *Columns included in the stripped sample are marked with :star:*

|Column Name    |Description |
|    :---:    |---|
|***Identifiers***||
|`objname`    |Common galaxy name|
|`pgc`        |PGC number|
|`nsa_id`||
|`group_id`||
|`ra`|Right Ascension|
|`dec`|Declination|
|`d25`|Apparent Diameter|
|`t_type`|Numerical Hubble T-Type|
|`color_type`|Color-based Type|
|`best_type`|Combined galaxy type|
|`v_h`|Heliocentric Radial Velocity|
|`v_cmb`|Radial velocity with respect to CMB radiation|
|`v_source`|Original source for compiled velocity|
|`hl_obj`|True for objects from HyperLeda|
|`lvg_obj`|True for objects from Karachentsev|
|`nsa_obj`|True for objects from NASA-Sloan Atlas|
|`sga_obj`|True for objects from Sienna Galaxy Atlas|
|***Photometry***||
|`bv_color`   |(B-V) color from HyperLeda|
|`br_color`   |(B-R) color queried from NED|
|`gr_color`   |(g-r) color from Sienna Galaxy Atlas|
|`gi_color`   |(g-i) color from NASA-Sloan Atlas|
|`b_lum`      |B-band Luminosity|
|`v_lum`      |V-band Luminosity|
|`R_lum`      |R-band Luminosity|
|`r_lum`      |r-band Luminosity|
|`i_lum`      |i-Band Luminosity|
|***Distance***||
|`cf3_dist`|Distances from CosmicFlows3 Calculator|
|`cf3_dist_error`||
|`zind_dist`|Redshift independent distances|
|`zind_dist_error`||
|`bestdist`   |Our chosen best distance estimate|
|`bestdist_error` |error for best distance estimate|
|`bestdist_indicator` |Indicator used for best distance, when available|
|`bestdist_method` |General method used for best distances|
|***Mass***||
|`logmass_i`|log(Mstar) from (g-i)|
|`logmass_r`|log(Mstar) from (g-r)|
|`logmass_V`|log(Mstar) from (B-V)|
|`logmass_R`|log(Mstar) from (B-R)|
|`logmass`    |Compiled best Log(mass) estimate|
|`logmass_src`|Color used for best mass estimate|
