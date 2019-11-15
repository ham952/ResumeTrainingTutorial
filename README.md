# ResumeTrainingTutorial
 Starting Stopping and Resuming Training
 
 https://www.pyimagesearch.com/2019/09/23/keras-starting-stopping-and-resuming-training/
 
--checkpoints : The path to our output checkpoints directory.

--model : The optional path to a specific model checkpoint to load when resuming training.

--start-epoch : The optional start epoch can be provided if you are resuming training. By default, training starts at epoch 0 



EpochCheckpoint : This callback is responsible for saving our model as it currently stands at the conclusion of every epoch. That way, if we stop training via ctrl + c  (or an unforeseeable power failure), we don’t lose our machine’s work — for training complex models on huge datasets, this could quite literally save you days of time.

TrainingMonitor : A callback that saves our training accuracy/loss information as a PNG image plot and JSON dictionary. We’ll be able to open our training plot at any time to see our training progress — valuable information to you as the practitioner, especially for multi-day training processes.
