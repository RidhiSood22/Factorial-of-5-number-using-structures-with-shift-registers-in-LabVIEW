# Factorial-of-5-number-using-structures-with-shift-registers-in-LabVIEW

# FOR loop
Executes its subdiagram n times, where n is the value wired to the count (N) terminal. The iteration (i) terminal provides the current loop iteration count, which ranges from 0 to n-1.

<img width="208" height="98" alt="image" src="https://github.com/user-attachments/assets/082ab49c-fe9c-4c98-a460-51c7e98005d8" />


# Terminal Inputs
<img width="16" height="16" alt="image" src="https://github.com/user-attachments/assets/f18799dc-223a-4889-a75d-6cd37e94560d" /> —The count terminal specifies the number of times to execute the code inside the For Loop. If you wire 0 or a negative number to the count terminal, the loop does not execute.
This terminal is displayed by default.

<img width="16" height="16" alt="image" src="https://github.com/user-attachments/assets/f3deb766-a848-401e-acc2-d245d30395f9" /> —(Optional) The parallel instances terminal specifies the number of loop instances LabVIEW uses to run parallel loop iterations. If you leave the input of the parallel instances terminal unwired, LabVIEW automatically detects the number of logical processors in the machine and uses it as the default parallel instances terminal value.
You can use the input of the parallel instances terminal and the Number of generated parallel loop instances in the For Loop Iteration Parallelism dialog box to improve For Loop performance by oversubscribing or undersubscribing.

# To display this terminal, enable parallel For Loop iterations.

<img width="16" height="16" alt="image" src="https://github.com/user-attachments/assets/d43d5355-b778-47c1-9fd1-883c9d50fe1e" /> —(Optional) The chunk size terminal specifies the custom iteration schedule used to execute chunks of loop iterations in parallel when you enable parallel For Loop iterations. You should specify a custom schedule only if the For Loop would benefit from a schedule different from the default.
To display this terminal, programmatically configure the loop iteration schedule.

<img width="16" height="16" alt="image" src="https://github.com/user-attachments/assets/4ec29ba6-31f4-4461-8986-4d301be6d56b" /> —(Optional) The conditional terminal allows you to specify additional conditions for stopping the For Loop. The For Loop normally stops after executing the number of iterations you specify using the count terminal. However, you can use the conditional terminal to stop the For Loop when other conditions occur, such as an error.
By default, the conditional terminal is set to Stop if True. You can change the behavior of the conditional terminal to Continue if True.

To display this terminal, set the For Loop to stop when a condition occurs.

 # For Loop Tunnel Inputs
Loop tunnels allow you to pass data through the For Loop. You can change the tunnel mode to handle data that passes through the For Loop in different ways, as listed in the following table.

<img width="25" height="9" alt="image" src="https://github.com/user-attachments/assets/114deca6-7e7d-4af3-bc1a-4fc688196b0e" /> —The tunnel passes data into and out of the For Loop without additional manipulation.
<img width="41" height="12" alt="image" src="https://github.com/user-attachments/assets/9809580a-c36a-4c3d-b39b-7d330b2f78f3" /> —Shift registers access data from the previous loop iteration and pass data to the next loop iteration.
<img width="25" height="9" alt="image" src="https://github.com/user-attachments/assets/a82facdb-e242-41d7-8b16-48ac30a27a6d" /> —When you wire an array or a collection data type to the input tunnel of the For Loop, the auto-index tunnels read and process one element in the array or collection per loop iteration.

# WHILE loop
Repeats the code within its subdiagram until a specific condition occurs. A While Loop always executes at least one time.

<img width="199" height="88" alt="image" src="https://github.com/user-attachments/assets/efb1f7f2-79aa-44de-a3b3-d7b33e1659e7" />

Components of a While Loop

<img width="253" height="208" alt="image" src="https://github.com/user-attachments/assets/a61be3be-985b-4f95-8ad9-f759b9b35811" />

1 —Subdiagram—Contains code that the While Loop executes once per iteration.

2 —Iteration Terminal (i)—Provides the current loop iteration count. The loop count always starts at zero for the first iteration. If the iteration count exceeds 2,147,483,647, or 231-1, the iteration terminal remains at 2,147,483,647 for all further iterations. If you need to keep count of more than 2,147,483,647 iterations, you can use shift registers with a greater integer range.

3 —Conditional Terminal—Evaluates a Boolean input value to determine whether to continue executing the While Loop. To specify whether the loop stops for a TRUE or FALSE Boolean value, configure the continuation behavior of the loop. You also can determine when the loop stops by wiring an error cluster to the conditional terminal.

# Output in this Repo

<img width="286" height="149" alt="image" src="https://github.com/user-attachments/assets/57222cc5-cc6e-4e6d-9835-0b673741ef8b" />



<img width="286" height="149" alt="image" src="https://github.com/user-attachments/assets/d0c5b71a-4739-4065-b08a-9420a4e58908" />
