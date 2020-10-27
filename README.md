# Homework 3

## Goal
The main task is to predict average daily temperature of Budapest on one day, one week and one month in advance with a feed forward neural network.

## Approach

Data was collected from [http://idojarasbudapest.hu/archivalt-idojaras](http://idojarasbudapest.hu/archivalt-idojaras), from 2017-01-01 to 2020-10-24. Data was preprocessed, and day of year and other important parameters were generated for training. 
Because of the main task was to create a feed forward network, historical data attributes were not calculated to the daily data, like average temperature of the previous week. 

A simple neural network was designed with two dense layer each one with 512 neurons. Relu activation was used and l2 regularization was applied in the dense layers. The output layer had one neuron and linear activation because the problem is a regression. To prevent overfitting, early stopping was used during the training.