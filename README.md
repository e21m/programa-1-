# programa-1-// sueldos.cpp : Defines the entry point for the console application.
//

#include "stdafx.h"
#include <iostream>
#include "conio.h"
#define iva 0.13
#define afp 0.1271
using namespace std;




void main()

{
  int n,i;
  float sb,sn;
  cout<<"ingrese el numero de empleados";
  cin>>n;
  for (i=1;i<=n;i++)
  {
	  cout<<"ingrese el salario bruto";
	  cin>>sb;
	  if (sb>=7000)
		  sn=sb-(iva+afp)*sb;
	  else 
		  sn=sb-(afp*sb);
	  cout<<"el salario neto es:"<<sn <<endl;
	  getch();
  }
  getch();
}

