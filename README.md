# Contoh-By-Value
    #include<stdio.h>
    #include<conio.h>

    void secara_nilai(float a, float b, char c)
    {
        float *alamat_A;
        alamat_A=&a;
        a=7;
        printf("lokal A= %f, alamat A= %p\n",a,alamat_A);
        printf("lokal B= %f\n",b);
        printf("lokal C= %c\n",c);
    }
    int main(){
    float a=25,*alamat_A;
    char c='a';
    alamat_A=&a;
    secara_nilai(a,a/3,c);
    printf("main A= %f,alamat A= %p\n",a,alamat_A);
    printf("main A/3= %f\n",(a/3));
    printf("main C= %c\n",c);
    getch();
    }
   # Hasil
   ![img}(https://raw.githubusercontent.com/AminPriadi/Contoh-By-Value-4/master/6.png)
