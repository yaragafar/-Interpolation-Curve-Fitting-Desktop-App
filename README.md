# Interpolation-and-Curve-Fitting-Desktop-App
A digital signal processing desktop app using python and PyQt5 where  Users can browse for a signal, interpolate, and visualize signals along with latex mathematical equations and an error map.

## Introduction
Curve fitting and interpolation are among the most usable tool in signal processing and data science. In 
curve fitting, the given points can be treated as one chunk that fits one polynomial, or small chunks, each to be fit into a 
different polynomial. The latter is often called spline interpolation. In any interpolation problem, a compromise is often 
needed between the order of the polynomial (usually, the higher order, the better accuracy) and the computational 
needs (usually, the higher order, the more exhaustive).

## Description
A python and PyQt5 desktop application that illustrates the efficacy of different curve fitting and interpolation models 
where:
- The user can open and display an arbitrary signal (of reasonable length of 1000 points).
- The user can choose if the fitting to be done as one chunk or multiple ones. If multiple, choose how many 
chunks the curve should be divided into. 
- The user can choose the order of the fitting polynomial (either for the big chunk or the multiple ones).
- Upon any change in the selections, the fitting result is displayed in dotted line on the same graph that 
displays the original signal.
- The fitted equation and percentage error is shown in its mathematical form above the main graph using 
Latex format. 
- The user can generate an error map for the fitting process via clicking a button. The user can choose the x- and y- axis of 
the error map among number of chunks, order of the fitting polynomial, and overlapping between 
consecutive chunks (0-25% of the chunk size). The error values in the map is normalized and shown 
up in percentage. 
- A progress bar shows the status of the map generation process, and the clicked button should turn into a “cancel” button where the user can click it to 
stop the process and return to the normal status.
- To illustrate the extrapolation efficacy, there is an option to clip the curve fitting process into only 
portion of the open signal. For example, apply the fitting process on only 50% or 60%,…or 90% of the signal. 
Then, the fitted curve is plotted for the whole signal. i.e., the last portion is practically extrapolated.

## Tools
- Python
- PyQt5
- QtDesigner

## Demo
- The user can open and display an arbitrary signal (of reasonable length of 1000 points).
![](https://github.com/yaragafar/Interpolation-and-Curve-Fitting-Desktop-App/blob/main/gifs/open_file.gif)



- The user can choose the order of the fitting polynomial (either for the big chunk or the multiple ones).
![](https://github.com/yaragafar/Interpolation-and-Curve-Fitting-Desktop-App/blob/main/gifs/linear_polynomial.gif)


- The user can choose if the fitting to be done as one chunk or multiple ones. If multiple, choose how many 
chunks the curve should be divided into
![](https://github.com/yaragafar/Interpolation-and-Curve-Fitting-Desktop-App/blob/main/gifs/chunks.gif)


- The user can generate an error map for the fitting process via clicking a button. The user can choose the x- and y- axis of 
the error map among number of chunks, order of the fitting polynomial, and overlapping between 
consecutive chunks (0-25% of the chunk size). The error values in the map is normalized and shown 
up in percentage. 
![](https://github.com/yaragafar/Interpolation-and-Curve-Fitting-Desktop-App/blob/main/gifs/error_map.gif)
