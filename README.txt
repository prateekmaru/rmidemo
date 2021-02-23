FOR LINUX USERS
RMI EXMPLE 
    1) compile all the java files  
      
    javac *.java  
      
    2)create stub and skeleton object by rmic tool  
      
    rmic AdderRemote  
    /*****
    
    p_x@ArcX:~/prateek/sem4/DAD/rmi$ rmic AdderRemote
Warning: generation and use of skeletons and static stubs for JRMP
is deprecated. Skeletons are unnecessary, and static stubs have
been superseded by dynamically generated stubs. Users are
encouraged to migrate away from using rmic to generate skeletons and static
stubs. See the documentation for java.rmi.server.UnicastRemoteObject.
p_x@ArcX:~/prateek/sem4/DAD/rmi$ 

    
    *******/
      
    3)start rmi registry in one command prompt  
      
    rmiregistry 2001 &  
    
    /*
  	p_x@ArcX:~/prateek/sem4/DAD/rmi$ rmiregistry 2001 &
	[1] 33866
	p_x@ArcX:~/prateek/sem4/DAD/rmi$ 

    */
      
    4)start the server in another command prompt  
      
    java MyServer  
      
    5)start the client application in another command prompt  
      
    java MyClient 
     
