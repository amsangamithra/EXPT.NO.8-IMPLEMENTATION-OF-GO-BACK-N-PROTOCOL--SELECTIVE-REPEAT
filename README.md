# EXPT.NO.9-IMPLEMENTATION-OF-GO-BACK-N-PROTOCOL-SELECTIVE-REPEAT.
# AIM:
To write and execute a program for Go-Back-N protocol-Selective Repeat.

# EQUIPMENTS REQUIRED:
Personal Computer Turbo C Compiler

# PROCEDURE:
	Connect two computers in Wired/Wireless LAN.
  
	Make sure that two computers are in one network and could able to ping each other.
   
In the codeblocker open new c file and type the program.

In the menu choose->Project->Properties->Project Build options->Linker settings->Add netproto and pthread.

Execute the program in both server and client.

Enter the IP address of the remote machine, port address of both local & remote machine and error rate.

Choose the file and verify the go back protocol operation.

# PROGRAM:

          #include<stdio.h> void main()
          {
          
          int i,j,n;
          printf("GO BACK N ARQ\n");
          //printf("Entermessage in format\n"); printf("Enter number of frame : "); scanf("%d",&n);
          char frame[n][10];
          
          for(i=1;i<=n;i++)
          {
          printf("Content for frame %d :",i); scanf("%s",&frame[i]);
          }
          int s=1;
          //while(j<=n){
          printf("Enter frame number with no ACK :"); scanf("%d",&j);
          for(i=1;i<=n;i++)
          {
          if(i!=j)
          printf("\n Sending frame %d \n FRAME ACKNOWLEDGED.	\n",i);
          //else
          //printf("\n Frame not Acknowledeged.	\n");
           
          }
          if(j<=n)
          {
          printf("No Acknowlegement for frame %d... \n",j); printf("Resending... Content from frame %d        :%s\n\n",j,frame[j]);
          
          }
          printf("\n Sending frame %d \n FRAME ACKNOWLEDGED.	\n",j);
          //}
          
          printf("\n\nALL FRAME RECIEVED SUCCESSFULLY\n\n");
          }

# OUTPUT:

 
<img width="451" height="475" alt="Screenshot 2026-03-19 at 5 26 41 PM" src="https://github.com/user-attachments/assets/d9fab10c-5993-448a-bdf5-c65bb233f594" />



# RESULT:
Thus the Go-Back-N protocol- Selective Repeat was implemented and the output is verified successfully.
