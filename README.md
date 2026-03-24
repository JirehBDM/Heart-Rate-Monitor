# Heart-Rate-Monitor
A function to monitor heart rate and display a warning when it becomes too high or too low.

## Language
- Matlab
## Features
- Displays a message when heart rate is too high or low
- Displays an error if the script is ran without data
## The Input

The provided file *heart.txt* contains the heart rate of an individual measured at intervals from a smart watch.

## The Process

First, the function needs to be defined. The written code first defines the outputs, being *outx* and *outy* which are then initialized as empty variables. Next, it defines the function as ```HeartFunc```, and the input of this function is the variable *heart_data*.

Next, a loop is created to check whether or not the inputted data is empty or not. MATLAB will not run the code and will display its own error, but this error may not be easily understood by the user. To ensure that the user can effectively troubleshoot, an error message is coded to display if the error has occurred due to the file being empty

A loop is then created where the current *heart_data* value is compared to the average of its last 5 values, if the value is higher or lower than 20% of this value, its time (position index) and status (whether it had increased or decreased) are recorded and displayed to the user. If there is no abnormality in the heart rate, the index and status are recorded as *normal*.

With the function initialized, a script can be written to load the file *heart.txt* into MatLab and save its contents within a variable we will call *heart_data*. To call the function, simply write it as any function would be written.
Output = Function( Input ). 

## The Output
<img width="555" height="95" alt="image" src="https://github.com/user-attachments/assets/896e4958-a900-4408-ad5d-bfc766475180" />

The code displays to the User when their heartrate was abnormally high or low.

## What I learned
### Working with Functions:
-  I explored and learned how to write and use functions in Matlab. It's evident that will be extremely useful in summarizing bulky code, and making it easier to re-use useful code for other projects. It's clear to me that further understanding how to use functions will change the way I approach problems in MatLab.
  
### Conditional Statements:
-  This project, I utilized the conditional statements ```if``` ```ifelse``` and ```else``` while writing my loop to achieve my intended results. Practicing with these commonly used statements had enhanced my familiarity with them, and will allow me to use them more effeciently in the future.

### Overall Growth:
Each part of this project helped me understand more about coding in Matlab, writing and running functions, and improving patient experience. It was more than just making a tool, it was about solving problems, learning new things, and improving my skills for future projects and work.

## How It Can Be Improved
-  The magnitude of the increase/decrease of the heart rate can be displayed along with the warnings.
-  The ability to sort the data based on the magnitudes, by the time they occured, or by increase or decrease could be added to provide better clarity.
-  More statistics could be added to inform the patient on the condition of their health.

## License
-  This project was completed for academic purposes and is open for educational use.
