# tester
Scanner scanner=new Scanner(System.in);
        int num=Integer.parseInt(scanner.nextLine());
        int a=1;
        int b=1;
        int c=0;
        int d=0;
       int ctr=0;
        for(int i=1;i<=num;i++)
       for(int j=1;j<=num;j++)
           for(int k=1;k<=num;k++)
               for(int l=1;l<=num;l++){
        System.out.printf("%s%s%s%s ",i,j,k,l);
         System.out.println();
        ctr++;
        
        if(ctr==4){
        a=i;
        b=j;
        c=k;
        d=l;
        }
        }
        if(ctr>=4){
        System.out.printf("PASS IS %s%s%s%s ",a,b,c,d);
       
        }else{
        System.out.prin

