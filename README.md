# Pearl_Oyster_ChIP_Seq

### Installing pipeline :

First, open your terminal. Then, run these two command lines :

    cd -place_in_your_local_computer
    git clone https://github.com/PLStenger/Pearl_Oyster_ChIP_Seq.git

### Update the pipeline in local by :

    git pull
    
### If necessary, install softwares by :   

    cd 99_softwares/
    conda install -c bioconda fastqc
    conda install -c bioconda trimmomatic
    conda install -c bioconda multiqc


### Know the number of CPU (threads) of your computer (here for MacOs) :   

    sysctl hw.ncpu
    > hw.ncpu: 4

### Run scripts in local by :


    # Put you in your working directory
    cd /scratch_vol1/fungi/Pearl_Oyster_ChIP_Seq/00_scripts
    
    
    # For run all pipeline, lunch only this command line : 
    time nohup bash 000_run_all_pipeline_in_one_script.sh &> 000_run_all_pipeline_in_one_script.out
    
    # Script 1
    time nohup bash 01_fastqc_raw_data.sh &> 01_fastqc_raw_data.out
    
