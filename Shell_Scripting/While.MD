```
#!/bin/bash

while true; do
    read -p "Enter a number (or 'q' to quit): " input

    if [[ $input == "q" ]]; then
        echo "Exiting the loop."
        break
    elif ! [[ $input =~ ^[0-9]+$ ]]; then
        echo "Invalid input. Please enter a valid number."
        continue
    fi

    echo "You entered: $input"
done

```





```
narendra@pop-os:~/Documents/DevOps/Shell_Scripting$ ./while_loop.sh 
Enter a number (or 'q' to quit): q
Exiting the loop.
narendra@pop-os:~/Documents/DevOps/Shell_Scripting$ ./while_loop.sh 
Enter a number (or 'q' to quit): 1
You entered: 1
Enter a number (or 'q' to quit): s
Invalid input. Please enter a valid number.
Enter a number (or 'q' to quit): 7
You entered: 7
Enter a number (or 'q' to quit): 8
You entered: 8
Enter a number (or 'q' to quit): 6
You entered: 6
Enter a number (or 'q' to quit): 

```

Explaination :

It is a simple while loop program which takes input and give input based on it.

case 1
when you press q : it break the program

case 2
when you press other character :
show Invalid input

case 3
For Number
it show the entered number

