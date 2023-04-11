Instruction for adding graphics file

1) Copy "graphics.h" and "winbgim.h" files to "include" folder of Dev C++ directory.
   Default location is C:\Program Files\Dev-Cpp\MinGW64\include\

2) Copy "libbgi.a" to file to "lib" folder of Dev C++ directory.
   Default location is C:\Program Files\Dev-Cpp\MinGW64\lib

3) Open Dev C++ , New Project => Console Application

4) Goto Project => Project Options ( or CTRL + H ) => Parameters. In Linker , Add These Codes (Remove Any Code If Exist )
-lbgi
-lgdi32
-lcomdlg32
-luuid
-loleaut32
-lole32

Click OK

5) Make sure to select TDM-GCC x.x.x 32-bit Release From Drop Down (x.x.x is Version) . Done
6) Demo Program To Check All Is Working Or Not

#include<graphics.h>
int main()
{
    int gd=DETECT,gm;
    initgraph(&gd,&gm,"");
    circle(200,200,100);
    getch();
}


www.NarendraDwivedi.Org