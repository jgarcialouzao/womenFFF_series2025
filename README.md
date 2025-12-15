# This README provides replication details for "Women's voice at work and family-friendly firms" 

# Data access


# Replication files
The full set of results can be obtained by running the `0_Master_File.do` program. This program includes the following sub-programs:

## Data preparation
  * `1_read_MCVL.do`          - opens raw MCVL files and transforms them in Stata format 
  * `2_code_panels.do`        - runs a sequence of do.files that create different panels [firms, workers, jobs, wages] that will be merged together 
  * `3_data_prep.do`          - prepares the data for the analysis; requires associated ado files: `sectorhom.do` `provtoreg.do` `censoredtobit_CHK.ado`

## Main text 
  * `Reg_Baseline.do` 				            - produces benchmark wage results as well as IV estimates and Oster bound exercise
  * `Reg_Mobility.do`      				        - produces mobility models
  * `Reg_WageMobility_CoopIncidence.do`   - estimates the wage gap and mobility by the incidence of cooperative time
  * `Reg_Returns2Exp.do`                  - produces wage returns to experience [including figure for catch-up rate]
  * `Reg_Promotions2Exp.do`               - produces promotion returns to experience

## Regular appendix
  * `Desc_FirstJob.do` + `Desc_PooledSample.do`    - generate results in the descriptive statistics table
  * `Reg_Baseline_Heterogeneity.do`                - wage effects by sub-groups 
  * `Reg_JobLadder.do`                             - persistence of cooperative employer
  * `Reg_Mobility_Unemployment.do`                 - incidence of unemployment over the career


## Online appendix
* additional figures and tables
    * `B1.FigureEntrants.do`
    * `B2.Graphs_Duration_first_job.do`
    * `B3.WorkerFE.do`
    * `B4.Distribution_CoopEntry_Observables.do`
    * `B5.Reg_ExitRate_1stJob.do`

* robustness test
    * `Reg_Baseline_Robust_WorkerOwned.do`
    * `Reg_Baseline_Robust_FirstJobDef.do`
    * `Reg_Baseline_Robust_LMRelationships.do`
    * `Reg_Baseline_Robust_Censoring.do`
    * `Reg_Baseline_Robust_FirmSizeEntry.do`

