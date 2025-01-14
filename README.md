'Main_code_R1.mlx' contains the code to run the main steps allowing to quantify the motor space of variability.

If you use the code please cite 
Manuello J. et al. "Mapping the complexity of motor variability: From individual space of variability to motor fingerprints". Behav Res (under review)


'Example_data.mat' contains all the stuff necessary to allow a straightforward run on the gait dataset described in Rengifo_Rodas et al. 2020, called Dataset 1 in our manuscript. 
The original data can be downloaded from https://data.mendeley.com/datasets/xzv6bjm9x2/1
Here, data come in a preprocessed and ready-to-use form, following the steps described in our manuscript.

'Matrix_BRS.m' is a 10x3x1051 where each page (i.e. 3rd dimension) is a step, described through 3 kinematics variable (i.e. 2nd dimension) over 10 time bins (i.e. 1st dimension). This structure allows a direct application of the 'procrustes' MATLAB function comparing each possible couple of steps (i.e. each possible couple of pages).

'StepNumber_Base.m' is a 1x84 vector specifying the number of steps walked in each instance. This information is necessary for the code to know how to attribute the single steps to the correct subject. Since 2 instances were analyzed for each of the 42 subjects, these are stored in consecutive cells of the vector. Note that each cell of the vector counts the increment of total number of steps walked. Therefore, the first cell is 15, meaning that subject 1 walked 15 steps in its first instance. The second cell is 29, meaning that subject 1 walked 14 steps (29-15) in its second instance. The third cell is 39, meaning that subject 2 walked 10 steps (39-29) in its first instance, and so on.

'SubjectNumber.m' is set to 42, corresponding to the sample size used for the analyses described in pur manuscript. Note that the 2nd dimension of 'StepNumber_Base.m' is 84 since 2 instances were analyzed for each of the 42 subjects.


If you need help or want to discuss specific issues please send emails to jordi.manuello@unito.it
