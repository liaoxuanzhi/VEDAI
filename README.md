# VEDAI

this is vehicle detection repository of Vehicle Detection on Aerial Imagery(VEDAI) based on Tensorflow object detection API.

annotations512 and annotations1024 files contain annotations descriptions of each images labelled separately in 512 X 512 pixels and 1024 X 1024 pixels.

data file contains the object_detection.pbtxt which indicates the class of item to be detected.

image_512 files contains VEDAI images in 512 * 512 pixels downloaded from https://downloads.greyc.fr/vedai/.

image_1024 files contains VEDAI images in 1024 * 1024 pixels downloaded from https://downloads.greyc.fr/vedai/.

main_vedai_512.py and main_vedai_1024.py use to generate XML files by extracting txt files from annotations512 and annotations1024. the XML files will be stored separately in image_512 and image_1024.

xml_to_csv_vedai.py converts the XML files to CSV files. please modify the codes to generate the different pixels image.

generate_tfrecord_vedai.py creates the train.record and test.record.

Note: once XML files are generated, then take parts into two set (training set and testing set ) and place them to directory: images/train and images/test separately.
