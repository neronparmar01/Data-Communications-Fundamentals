/*  Name: Parmar Neron Nelson
    ID: 171690217
    Email: nparmar22@myseneca.ca  */
    
    var initial;                                      
    var array_2;                                     
    var arr;
    var sum;
    initial = [0,1,1,1,1,1,1,0,1,1,1,1,1,1,0];        
    array_2 = [0,1,1,1,1,1,1,0,1,1,1,1,1,1,0];
    arr = [0,1,1,1,1,1,1,0]; 
    
    for (var i=0; i<array_2.length; i++){                   
        if(array_2[i]==1){
            sum+=1;                                         
        }
        if (array_2[i]==0){
            sum=0;                                          
        }
        else if (sum%5==0){
            array_2.splice(i+1,0,0);                        
        }
    }
    console.log("Before Stuffing : ", initial.join(" "), "--", initial.length, "characters"); 
    console.log("After Stuffing  : ", array_2.join(" "), "--", array_2.length, "characters");               
    console.log("After Framing   : ", arr.concat(array_2.concat(arr)).join(" "));           
    
    
    