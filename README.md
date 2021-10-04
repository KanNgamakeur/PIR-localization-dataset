# PIR-localization-dataset
dataset for PIR localization

PIR Localization dataset

This data contains single person localization data collected from PIR sensors 

1.folder structure

     dataset
  	-training_data
            - training_data_LR.mat
	    - training_data_LRUD.mat
            - training_data_RLUD.mat
            - training_data_UD.mat
  	-testing_data
	    - sc1.mat
            - sc2.mat
            - sc3.mat
            - sc4.mat
2. mat file structure
	
	each training data is stored in the matlab cell structure. The each row represents profile data collected 
        from different walking path in the monitored area. The first column of the cell stores the collected sensor data and 
        the matrix of collected data is formatted as sensor_channel x timestep x sample.The second column of the cell holds 
        the groundtruth and the labels are defined using numbers such as 11 12 13. The number such as 11 can be interpreted as 
        the location is grid 1 and cell 1. The details of monitored area is discusses in the paper. 

        each testing data is stored in the matlab cell in the similar manner.
        the matrix of collected data is formatted as sensor_channel x timestep.   

  
