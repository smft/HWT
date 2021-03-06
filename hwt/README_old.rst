
Information on the various files and how they were used during HWT 2019
=======================================================================


Directories:
============


additional_programs:
--------------------

 create_met_poly.py:

 run_met_surrogate_severe_perc.py:

 run_pcp_obs.py:


cron_jobs:
----------

  contains the two crontab files that were run during HWT 2019 on buxton2 and bigbang2
examples: contains the METplus configuration files for different runs of HWT variables and models
met_config: contains MET configuration files for the different MET executables

viewer_config:
--------------

  Automated scorecard images were created using METviewer running continuously inside a container and having cron entries send command line requests to the container.
- container_config
   docker-compose.yml is the yml file used to set up the HWT docker instance

   docker.sh is the shell script calling docker compose and giving an example of the metviewer commands to create the scorecards
- db_load
   a series of xml files used to load individual databases
- scorecards
   xml files to create different HWT scorecards


examples
--------

- bigbang.conf: 
   contains the full path to ncap2, since the executable is in different places on buxton2 and bigbang2.  This .conf file is only needed when running METplus on bigbang2
- base_paths.conf:
- ens_mean_apcp24.conf:
- ens_mean_apcp3.conf:
- ens_stat.conf:
- ens_stat_apcp24.conf:
- ens_stat_apcp3.conf:
- grid_stat_pcp.conf:
- grid_stat_refc.conf:
- HREFv2.conf:
- HREFv2_ens.conf:
- HREFv2_ens_apcp24.conf:
- HREFv2_ens_apcp3.conf:
- HRRRe.conf:
- HRRRe_ens.conf:
- HRRRv3.conf:
- HRRRv4.conf:
- hrrre_regrid.conf:
- NSSLfv3.conf:
- pb2nc.conf:
- pcp_24.conf:
- pcp_3.conf:
- pcprg_24.conf:
- pcprg_3.conf:
- point_stat.conf:
- point_stat_ens.conf:
- time_ens_apcp24_00.conf:
- time_ens_apcp24_12.conf:
- time_ens_apcp3.conf:
- time_valid.conf:

met_config
