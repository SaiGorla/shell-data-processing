# Shell - Data - Processing

## GitBash Commands

* Transform each space into a return character 
  ```bash
  tr ' ' '\12' < data.txt
  ```
    
* Send the results of one command as input into another command
  ```bash
  tr ' ' '\12' < returnedfile | sort
  ```

* Redirect the output to result.txt 
  ```bash
  tr ' ' '\12' < returnedfile | sort | uniq -c | sort -nr > result.txt
  ```
  
* The Command used to fing the most common words, sorted:
  ```bash
     tr ' ' '\12' < data.txt | sort | uniq -c | sort -nr
     ```
    
## Links:

+ [Data.txt](https://github.com/SaiGorla/shell-data-processing/blob/master/data.txt)

+ [Result.txt](https://github.com/SaiGorla/shell-data-processing/blob/master/result.txt)
