# C-Dili-Örnekleri
 
 SWİTCH CASE 
 ATM DE BANKA İŞLEMİ YAPMA 
   
    #include<stdio.h>
     int main()
        {
    int islem;
    int bakiye =1000;
    int tutar;
    printf("İşlemeler\n1:Para çekme \n2:Para yatırma\n3:Havale yapma\n4:Bakiye sorgulama\n5:Kart iade\n\n\n");
    printf("İşlemi seçiniz");
    scanf("%d",&islem);
    switch(islem){
        case 1:
            printf("Bakiyeniz:%d\n",bakiye);
            printf("Çekilecek tutar:\n");
            scanf("%d",&tutar);
            if(tutar>bakiye){
                printf("bakiyeniz yetersiz\n");
            }
            bakiye-=tutar;
            printf("Bakiyeniz:%d\n",bakiye);
            break;
        case 2:
            printf("Bakiyeniz:%d\n",bakiye);
            printf("Yatırılacak tutar:\n");
            scanf("%d",&tutar);
           
            bakiye+=tutar;
            printf("Bakiyeniz:%d\n",bakiye);
            break;
            
        case 3:
            printf("Bakiyeniz:%d\n",bakiye);
            printf("Havale yapılacak tutar:\n");
            scanf("%d",&tutar);
            if(tutar>bakiye){
                printf("bakiyeniz yetersiz\n");
            }
            bakiye-=tutar;
            printf("Bakiyeniz:%d\n",bakiye);
            break;
        case 4:
            printf("Bakiyeniz:%d\n",bakiye);
          
            break;
        case 5:
            printf("Kart iade edildi.\n");
            
        default:
            printf("Bilinmeyen işlem\n");
    }
    return 0;
    
}

DÖRT İŞLEM


      #include<stdio.h>
       int main(){
        int islem;
        int sayi1;
        int sayi2;
        int sonuc;
    printf("Birinci ve ikinci sayıyı giriniz:\n");
    scanf("%d  %d",&sayi1,&sayi2);
    printf("İşlemler\n1:Toplama\n2:Çıkarma\n3:Çarpma\n4:Bölme\n");
    scanf("%d",&islem);
    
    switch(islem){
        case 1:
            printf("sayılarınız %d ve %d\n",sayi1,sayi2);
            sonuc = sayi1 + sayi2;
            printf("İşlemin sonucun %d'dir.\n",sonuc);
            break;
        case 2:
            printf("sayılarınız %d ve %d\n",sayi1,sayi2);
            sonuc = sayi1 - sayi2;
            printf("İşlemin sonucun %d'dir.\n",sonuc);
            break;
            
        case 3:
            printf("sayılarınız %d ve %d\n",sayi1,sayi2);
            sonuc = sayi1 * sayi2;
            printf("İşlemin sonucun %d'dir.\n",sonuc);
            break;
        case 4:
            printf("sayılarınız %d ve %d\n",sayi1,sayi2);
            sonuc = sayi1 % sayi2;
            printf("İşlemin sonucun %d'dir.\n",sonuc);
            break;
            
        default :
            printf("bilinmeyen işlem\n");
            
    }
    
    return 0;
    
}

