This project contains the workload traces used in the simulations for
the paper entitled "Host Overload Detection for Dynamic Consolidation
of Virtual Machines in Clouds Based on a Markov Chain Model and
Multisize Sliding Window Workload Estimation", which has been
submitted to the Special Issue of TPDS on Cloud Computing.

The data have originally been provided as a part of the CoMon project,
a monitoring infrastructure for PlanetLab: [http://comon.cs.princeton.edu/](http://comon.cs.princeton.edu/).

The simulated host was assumed to be equipped with a quad-core
CPU. The clock frequency of a single core of the host was set to 3
GHz, which according to the model introduced in the paper transforms
into 12 GHz. These CPU characteristics correspond to a mid-range
Amazon EC2 physical server type. The amount of the host’s memory was
assumed to be enough for the Virtual Machines (VMs) allocated to the
host. The CPU frequency of a VM was randomly set to one of the values
approximately corresponding to [the Amazon EC2 instance types](http://aws.amazon.com/ec2/instance-types/): 
1.7 GHz, 2 GHz, 2.4 GHz, and 3 GHz.

The data are in the comma-delimited CSV format, where the columns are:

    Simulation ID - the index of a simulation, or a set of VMs assigned to the host
    VM ID         - the index of a VM within a simulation
    Time Frame    - the index of a time frame within a simulation
    CPU Frequency - the CPU frequency of a VM in MHz
    Utilization   - the VM's CPU utilization as a percentage of the VM's CPU frequency

## License

Copyright (C) 2012 Anton Beloglazov
