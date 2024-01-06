Working with IBM’s aihwkit tool in this assignment. The tool can be used to do 
hardware-aware neural networks training and inference. Currently, it offers crossbar array 
models for simulating the synapses (Linear layer in Pytorch) in hardware. The tool can be 
divided into two parts: 1. A backend c++ based simulator for crossbar arrays 2. A Pytorch 
frontend that offers function calls to the sim in the Pytorch native layer-like form.

1. Create a hardware-aware equivalent of neural net class
Replace Linear layers in your net with AnalogLinear layers from the tool. Use the constant 
step device config for the crossbar.

2. Fit the model and report the final validation accuracy
Remember to use the AnalogSGD optimizer provided by the tool. Also, apply the
regroup_param_groups function on your model parameters (required by the tool)

3. Repeat the experiment for the following preset device configs and tabulate
the final validation accuracies respectively.
ReRamSBPresetDevice, ReRamESPresetDevice, CapacitorPresetDevice,
IdealizedPresetDevice, PCMPresetDevice
