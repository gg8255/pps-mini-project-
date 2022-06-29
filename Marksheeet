#include <stdio.h>
#include <string.h>
#include <stdlib.h>
int main ()
{
  char name[30], fname[30];
  int rollNo, standard, math, hindi, english, physics, chemistry, obtained,percentage,grade, i, n = 1,a;
      struct marksheet_sheet
    {
  char name;
  char fname;
  char rollNo;
  char standard;
  char math;
  char hindi;
  char english;
  char physics;
  char chemistry;
  char obtained;
  char percentage;

}b;
    b.name;
    b.fname;
    b.rollNo;
    b.standard;
    b.math;
    b.hindi;
    b.english;
    b.physics;
    b.chemistry;
    b.obtained;
    b.percentage;

  while (1)
    {
      printf("Enter\n1-To make marksheet of a student\n2-To show the list and mark of student\n3-To exit the program:");
      scanf("%d",&a);
      if(a==1)
      {
      printf ("Enter Your name !! \n");
      scanf ("%s", name);
      printf ("Enter Your Father name !! \n");
      scanf ("%s", fname);
      printf ("Enter Your Roll no !! \n");
      scanf ("%d", &rollNo);
      printf ("Enter Your Class !! \n");
      scanf ("%d", &standard);
      printf ("Enter maths marks !! \n");
      scanf ("%d", &math);
      printf ("Enter hindi  marks !! \n");
      scanf ("%d", &hindi);
      printf ("Enter English marks !! \n");
      scanf ("%d", &english);
      printf ("Enter Physics marks !! \n");
      scanf ("%d", &physics);
      printf ("Enter Chemitry marks !! \n");
      scanf ("%d", &chemistry);

      // Calculating OBTAINED marks and percentage
      obtained = math + hindi + english + physics + chemistry;
      percentage = obtained * 100 / 500;
      FILE *fptr;
      fptr = (fopen ("student.txt", "a"));
      fprintf (fptr, "\nName:%s \nfname:%s \nrollNo=%d \nstandard=%d \nmath=%d \nhindi=%d \nenglish=%d \nphysics=%d  \nchemistry=%d \npercentage=%d ", name,fname,rollNo,standard,math,hindi,english,physics,chemistry,percentage);
      fclose (fptr);
      // printing marksheet
      printf ("--------MARKSHEET--------\n");

      printf ("Your name is %s \n", name);
      printf ("Your Father name is %s \n", fname);
      printf ("Your Roll number is %d \n", rollNo);
      printf ("Your Class is %d \n", standard);
      printf ("Your obtained marks are %d \n", obtained);
      printf ("Your percentage is %d \n", percentage);

      // if else if  for grades
      if (percentage >= 80)
	{
	  printf ("Grade : A-1 \n");
	}
      else if (percentage >= 70)
	{
	  printf ("Grade : A \n");
	}
      else if (percentage >= 60)
	{
	  printf ("Grade : B \n");
	}
      else if (percentage >= 50)
	{
	  printf ("Grade : C \n");
	}
      else if (percentage >= 40)
	{
	  printf ("Grade : D \n");
	}
      else if (percentage >= 33)
	{
	  printf ("Grade : E \n");
	}
      else
	{
	  printf ("Grade : F \n");
	}

      //obtained = math+ hindi + english + physics + chemitry;
      int supply = 0;

      if (math < 33)
	{
	  printf ("You have supply in maths\n");
	  supply++;
	}
      if (hindi < 33)
	{
	  printf ("You have supply in hindi\n");
	  supply++;
	}
      if (english < 33)
	{
	  printf ("You have supply in english\n");
	  supply++;
	}
      if (physics < 33)
	{
	  printf ("You have supply in physics\n");
	  supply++;
	}
      if (chemistry < 33)
	{
	  printf ("You have supply in chemistry\n");
	  supply++;
	}
    }
    else if(a==2)
    {
            char c;
    FILE *fr;
    fr=fopen("student.txt","r");
    while( c != EOF)
    {
        c = fgetc(fr);
        printf("%c",c); 
    }
        
    }
    else if(a==3)
    {
        exit(0);
    }
    }
  //printf("You have %d supply", supply);

  return 0;
}
