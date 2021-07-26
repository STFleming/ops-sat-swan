# Setting up the OPS-SAT development environment

The FPGA onboard OPS-SAT is an intel FPGA which means that a tool Quartus is required to generate bitstreams for it. I have created a common tools folder avaialbe to all OPS-SAT members where the FPGA tools will be installed. 

```
/tools/Intel
```

## Setup steps

1. Run the following command in an OPS-SAT-Server terminal
```
	echo "export PATH=\$PATH:\"/tools/Intel/20.01/quartus/bin\"" >> ~/.bashrc
	echo "export PATH=\$PATH:\"/tools/Intel/20.01/quartus/sopc_builder/bin\"" >> ~/.bashrc
	echo "export QSYS_ROOTDIR=\"/tools/Intel/20.01/quartus/sopc_builder/bin\"" >> ~/.bashrc
	echo "export LM_LICENCE_FILE=\"/tools/lics/jl_temp_quartus_lic.dat\"" >> ~/.bashrc
```

2. Logout and Log back in

3. Open Quartus 
```
quartus
```

## Base FPGA project

A base Quartus/Qsys project for implementing a custom circuit in the FPGA fabric and configuring the processing system can be found [here](https://github.com/STFleming/oss_fpga_base).


### Rough notes

Critical Links SoM board ID: 5CSE-L2-3Y8-RC

Intel FPGA part: 5CSEBA2U23C8SN

Critical Links setup guides: https://support.criticallink.com/redmine/projects/mityarm-5cs/wiki
