# deep-learning-challenge

Our goal is create a neural network that can determine whether or not a charity is successful or not from these variables

APPLICATION_TYPE 	AFFILIATION 	CLASSIFICATION 	USE_CASE 	ORGANIZATION 	STATUS 	INCOME_AMT 	SPECIAL_CONSIDERATIONS 	ASK_AMT 	IS_SUCCESSFUL.

After performing the necessary data cleaning we perform the following task
number_input_features = len(X_train[0])
hidden_nodes_layer1 = 10
hidden_nodes_layer2 = 5

nn = tf.keras.models.Sequential()

# First hidden layer
nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer1, input_dim=number_input_features, activation="relu"))

# Second hidden layer
nn.add(tf.keras.layers.Dense(units=hidden_nodes_layer2, activation="relu"))

# Output layer
nn.add(tf.keras.layers.Dense(units=1, activation="sigmoid"))

# Check the structure of the model
nn.summary()

The given output goes as followed 

268/268 - 0s - loss: 0.5533 - accuracy: 0.7292 - 427ms/epoch - 2ms/step
Loss: 0.553272008895874, Accuracy: 0.7292128205299377
