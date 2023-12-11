## Write to a file
Using the fs library again, try to write to the contents of a file.
You can use the fs library to as a black box, the goal is to understand async tasks.



let fs=require('fs');

let toWriteData="Pankaj singh , full-stack developer";

fs.writeFile(`{__dirname}/out.txt`,toWriteData,(err,data)=>{
  if(err){
    console.log("There is some error in writing data to file");
  }else{
    console.log("data is written successfully in out.txt");
  }
});