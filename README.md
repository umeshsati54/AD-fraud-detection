# AD-fraud-detection

Objective is to predict whether a user will download an app after clicking a mobile app advertisement.

Download data from https://www.kaggle.com/c/talkingdata-adtracking-fraud-detection/data

# File descriptions
1. train.csv - the training set
2. train_sample.csv - 100,000 randomly-selected rows of training data, to inspect data before downloading full set
3. test.csv - the test set
4. sampleSubmission.csv - a sample submission file in the correct format
UPDATE: test_supplement.csv - This is a larger test set that was unintentionally released at the start of the competition. It is not necessary to use this data, but it is permitted to do so. The official test data is a subset of this data.

# Data fields
Each row of the training data contains a click record, with the following features.

1. ip: ip address of click.
2. app: app id for marketing.
3. device: device type id of user mobile phone (e.g., iphone 6 plus, iphone 7, huawei mate 7, etc.)
4. os: os version id of user mobile phone
5. channel: channel id of mobile ad publisher
6. click_time: timestamp of click (UTC)
7. attributed_time: if user download the app for after clicking an ad, this is the time of the app download
8. is_attributed: the target that is to be predicted, indicating the app was downloaded
Note that ip, app, device, os, and channel are encoded.

The test data is similar, with the following differences:

1. click_id: reference for making predictions
2. is_attributed: not included
