# comet-cooling
This repository contains codes for cooling methods 

first of all run the command "make" inside the hotspot_tool and hotspot_tool3 folders.

Go to the CoMeT-main/config/hotspot/2_5D and copy all the content into the hotspot_tool folder.

run the notebook oldarch file generator to generate sample trace files within  designated folders. After creating the traces, got to the folder containing the traces named "mycsv2_5.trace" and run the following command.


"../../../hotspot -c ../../../stack_hotspot.config -p mycsv2_5.trace -o temperature_mem.trace -model_secondary 1 -model_type grid -steady_file steady_temperature_mem.log -all_transient_file all_transient_mem.init -grid_steady_file grid_steady_mem.log -steady_state_print_disable 1 -l 1,1,1,1,1,1,1,1,1,1,1,1,1,1,1,1, -type 2.5D -sampling_intvl 0.001 -grid_layer_file ../../../stack.lcf -detailed_3D on -init_file ../../../stack.init"
