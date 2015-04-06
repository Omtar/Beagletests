/*
 * 
 *
 *      Reading the four analog values and then printing them out
 *      SYSFS method
 *      Author: Khurram
 */



#include <iostream>
#include <stdlib.h>
#include <stdio.h>
#include <string.h>
#include <fcntl.h> //define O_WRONLY and O_RDONLY
#include <unistd.h>

#define ADC_0 "/sys/devices/ocp.3/helper.15/AIN0"
#define ADC_1 "/sys/devices/ocp.3/helper.15/AIN1"
#define ADC_5 "/sys/devices/ocp.3/helper.15/AIN5"
#define ADC_6 "/sys/devices/ocp.3/helper.15/AIN6"
#define MAX_BUF 64


int main()
{
    int fd0,fd1,fd5,fd6, len;
    char buf[4],buf1[4],buf5[4],buf6[5];
    int ch=0,ch1=0, ch5=0, ch6=0;
    float X=0, Y=0,Sum=0;
    int inter1=0,inter2=0,inter3=0;
    int inter5=0,inter6=0,inter7=0;
    float inter4=0,inter8=0;
    int i;
    FILE *Handle0 = NULL; //Initialization
    FILE *Handle1 = NULL;
    FILE *Handle5 = NULL;
    FILE *Handle6 = NULL;

    	 //Handle0 = fopen("/sys/devices/ocp.3/helper.15/AIN0", "r");
    	 // Handle1 = fopen("/sys/devices/ocp.3/helper.15/AIN1", "r");
    	 //Handle5 = fopen("/sys/devices/ocp.3/helper.15/AIN5", "r");
    	// Handle6 = fopen("/sys/devices/ocp.3/helper.15/AIN6", "r");
         int a=0, a0=0, a1=0, a5=0, a6=0, b=0;
         
while(1)
{
         for ( int loop1=0;loop1<2;loop1++)

         {
        	 Handle0 = fopen("/sys/devices/ocp.2/helper.11/AIN0", "r"); //Getting values from First ADC port

        	 a=0;
    	    
    	    while(1)
    	      {
    	        ch = fgetc(Handle0);

    	       if(feof(Handle0 ))
    	         {
    	            break ;
    	         } //If end

           //printf("%c", ch);
             buf[a]=ch;
    	       a++;

    	      } //End of while(1)

    	      //puts(buf);
    	        a=0;
    	        a0=atoi(buf);
    	        printf("AN:0 %d\n",atoi(buf));
    	      //printf("%d",a);
              fclose(Handle0);

         }
                a=0;
                std::cout<<std::endl;
//////////////////////////////////////////////////////////////
/////////////

               for ( int loop2=0;loop2<2;loop2++)

                {
               	 Handle1 = fopen("/sys/devices/ocp.2/helper.11/AIN1", "r");

               	 a=0;
           	while(1)
           	     {
           	        ch = fgetc(Handle1);

           	       if(feof(Handle1))
           	        {
           	            break ;
           	        }

           //     printf("%c", ch);
                  buf1[a]=ch;
           	      a++;

           	     }

           	      //puts(buf);
           	        a=0;
           	        a1=atoi(buf1);
           	        printf("AN1: %d\n",atoi(buf1));
           	      //printf("%d",a);
                    fclose(Handle1);

                }
                       a=0;
                       std::cout<<std::endl;
////////////////////////////////////////////////////////////////////////////////////

                       for ( int loop5=0;loop5<2;loop5++)

                       {
                      	 Handle5 = fopen("/sys/devices/ocp.2/helper.11/AIN5", "r");

                      	 a=0;
                  	while(1)
                  	     {
                  	        ch5 = fgetc(Handle5);

                  	       if(feof(Handle5 ))
                  	        {
                  	            break ;
                  	        }

                            	 //     printf("%c", ch);

                  	      buf5[a]=ch5;
                  	      a++;

                  	     }

                  	      //puts(buf);
                  	        a=0;
                  	        a5=atoi(buf5);
                  	        printf("AN5: %d\n",atoi(buf5));
                  	      //printf("%d",a);
                            fclose(Handle5);

                       }
                              a=0;
                              std::cout<<std::endl;
/////////////////////////////////////////////////////////////////


                          for ( int loop6=0;loop6<2;loop6++)

                                      {
                                     	 Handle6 = fopen("/sys/devices/ocp.2/helper.11/AIN6", "r");

                                     	 a=0;
                                 	while(1)
                                 	     {
                                 	        ch6 = fgetc(Handle6);

                                 	       if(feof(Handle6 ))
                                 	        {
                                 	            break ;
                                 	        }

                                      //printf("%c", ch);
                                       buf6[a]=ch6;
                                 	      a++;

                                 	     }

                                 	      //puts(buf);
                                 	        a=0;
                                 	        a6=atoi(buf6);
                                 	        printf("AN:6 %d\n",atoi(buf6));
                                 	      //printf("Last one done");
                                 	      //printf("%d",a);
                                         fclose(Handle6);

                                      }
                                             a=0;
                                            std::cout<<std::endl;
/////////////////////////////////////////////////////////////////////////////////
         /*  	while(1)
            	     {
            	        ch1 = fgetc(Handle1);

            	       if(feof(Handle1 ))
            	        {
            	            break ;
            	        }

            	      printf("%c", ch1);
            	      buf1[a]=ch1;
            	      a++;

            	     }
                             	puts(buf1);
            	    	        a=0;
            	    	        a=atoi(buf1);
            	    	        printf("tttttttttttttt %d\n",atoi(buf1));
            	    	        printf("%d",a);


                        fclose(Handle1);

 ////////////////////////////////////////////////////////////
                        while(1)
                                    	     {
                                    	        ch5 = fgetc(Handle5);

                                    	       if(feof(Handle5 ))
                                    	        {
                                    	            break ;
                                    	        }

                                    	      printf("%c", ch5);
                                    	     }
                                                fclose(Handle5);

                                                ////////////////////



///////////////////////////////////////////////////////////////////////////
                                                while(1)
                                                            	     {
                                                            	        ch6 = fgetc(Handle6);

                                                            	       if(feof(Handle6 ))
                                                            	        {
                                                            	            break ;
                                                            	        }

                                                            	      printf("%c", ch6);
                                                            	     }
                                                                        fclose(Handle6);

        // while(1)
    //{
   /* for(i=0;i<50;i++)
    {
        snprintf(buf,sizeof(buf),ADC_0);
        fd0 = open(buf, O_RDONLY);
        read(fd0,ch0,4);
        printf("AIN0:%s\n",ch0);

        close(fd0);
        usleep(1000);//pause for 1 ms

   /*     /////////////////////////////////////////////////////
       snprintf(buf,sizeof(buf),ADC_1);
        fd1 = open(buf, O_RDONLY);
        read(fd1,ch1,4);
        printf("AIN1: %s\n",ch1);
        close(fd1);
        usleep(1000);//pause for 1 ms
        /////////////////////////////////////////////////////
        snprintf(buf,sizeof(buf),ADC_5);
        fd5 = open(buf, O_RDONLY);
        read(fd5,ch5,4);
        printf("AIN5 %s\n",ch5);
        close(fd5);
        usleep(1000);//pause for 1 ms
        //////////////////////////////////////////////////////
        snprintf(buf,sizeof(buf),ADC_6);
        fd6 = open(buf, O_RDONLY);
        read(fd6,ch6,4);
        printf("AIN6: %s\n",ch6);
        close(fd6);
        usleep(1000);//pause for 1 ms

       /////////////////////////////////////////////////////


    //}
        std::cout<<std::endl; */
        inter1 = a0 + a1 ;
        inter2 = a5 + a6 ;
        inter3 = inter1 - inter2;
        Sum    = a0 + a1 + a5 + a6;
        inter4 = inter3 / Sum;
        X      = inter4;
        //printf ( "  X = %d \n", X );

        ///////////////////////////////////////////////////////
        inter5 = a5 + a0;
        inter6 = a1 + a6;
        inter7 = inter5 - inter6;
        inter8 = inter7 / Sum;
        Y      = inter8;

        printf ( "X =%f  Y = %f  Sum = %f \n ", X, Y, Sum);
        sleep(3);
}

return 0;
}
