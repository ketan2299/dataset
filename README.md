model = Sequential()
model.add(Dense(12, input_dim=9, init='normal', activation='relu'))
model.add(Dense(9, init='normal', activation='relu'))
model.add(Dense(6, init='normal', activation='relu'))
model.add(Dense(3, init='normal', activation='relu'))
model.add(Dense(1, init='normal', activation='sigmoid'))

# 3. Compile Model.
model.compile(loss='binary_crossentropy', optimizer='adam', metrics=['accuracy'])
