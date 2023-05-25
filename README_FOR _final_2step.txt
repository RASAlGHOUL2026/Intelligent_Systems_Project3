instruction to run final_2step.ipynb
============================================================

LINK YOUR GOOGLE DRIVE AND SAVE THE DATA SET IN THE DRIVE 
TO RUN THE NOTEBOOK ON GOOGLE COLLAB

============================================================

==>In Classification of human and non human images

# Define the path to the directory containing the images
original_dir = 'PATH TO THE DIRECTORY OF THE IAMGES TO TEST'

P.S can be any images you want to test
=============================================================


==>In Training new model

# Re-size all the images
IMAGE_SIZE = [224, 224]

train_path = 'PATH TO train IMAGES'
valid_path = 'PATH TO Val IMAGES'

------------------------------------------------------------
# useful for getting number of output classes
folders = glob('PATH TO train IMAGES/*')
                                     ^
DONT FORGET TO PUT ABOVE ============*
      
------------------------------------------------------------                               

# Generate training and validation data
training_set = train_datagen.flow_from_directory('PATH TO train IMAGES',
                                                 target_size = (224, 224),
                                                 batch_size = 16,
                                                 class_mode = 'categorical')
test_set = test_datagen.flow_from_directory('PATH TO val IMAGES',
                                            target_size = (224, 224),
                                            batch_size = 16,
                                            class_mode = 'categorical')


==============================================================

DATA SET LINK FROM MY DRIVE
==============================================================

 PATH TO train IMAGES = https://drive.google.com/drive/folders/1qjW3HPvBXiHHCiv4eRucWK-z8ewQMlkd?usp=share_link

 PATH TO val IMAGES = https://drive.google.com/drive/folders/1j6lqPGfwIHeXWQgGiOTV7mowzZUGHvjk?usp=share_link
 
 original_dir = https://drive.google.com/drive/folders/1Shpd1Gt9VzL5Eh8RJFOdLS-ntYFzCsNT?usp=share_link








