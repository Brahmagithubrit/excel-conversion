# excel-conversion
 this is the single conversion of the number in the column of xl into column letter like for A=1,b=2....z=26, AA=27..and so on .
 here is the sample code 
 String colName (long n)
    {
        
        StringBuilder s=new StringBuilder ();
        while(n>0){
            long remainder=(n-1)%26;
            char result=(char)('A'+remainder);
            s.insert(0,result );
            n=(n-1)/26;
        }
        return s.toString();
    }
