# All-prime-nos.-upto-n
// SIEVE OF ERATOSTHENES

ll p[100001];
    
    for(i=0; i<=100000; i++){
        p[i]=1;
    }
    
    for(i=2; i<=100000; i++)
    {
        if(p[i]==1){
            for(j=i*i; j<=100000; j+=i){
                p[j]=0;
            }
        }
    }
    
