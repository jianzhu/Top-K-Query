
A simple Java implementation of the WAND top-k retrieval algorithm. Here are information regarding 
the WAND top-k retrieval algorithm. An in-depth PowerPoint presentation: https://www.slideshare.net/AndrewZhang44/wand-topk-retrieval 
and Original paper: "Efficient Query Evaluation Using a Two-Level Retrieval Process" by Andrei Z. Broder

Inside the TopKQuery folder issue the following command:  

    java -jar dist/TopKQuery.jar <file name> -k <K> -s<No. of Skips> -c <UB Constant>

Alternativley you can run: 

    java -classpath "dist/TopKQuery.jar:dist/lib/*:" topkquery.TopKQuery <file name> -k <K> -s<No. of Skips> -c <UB Constant>

You have to atleast mention the file name that is the first argument to run the program. 
If you want to use 6th argument you must ensure to provide all preciding arguments too.

Example:  java -jar dist/TopKQuery.jar data.txt -k 5, will return topk documents 
and their scores. Then provide the terms as: t1 t2 t3 t4 etc and press enter for output.
