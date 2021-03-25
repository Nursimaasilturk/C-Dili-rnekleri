# C-Dili-Örnekleri
 
 SWİTCH CASE DE ATM DE BANKA İŞLEMİ YAPMA 
   
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
