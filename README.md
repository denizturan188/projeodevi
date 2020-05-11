# projeodevi
Banka Otomasyonu

#include <stdio.h>
#include <stdlib.h>

struct musteri{
	
	char adSoyad[50];
	int id;
	int type;
	int dg;
	
};

int main(int argc, char *argv[]) {

	
	int a, i, n=0;
	
	printf("Yeni musteri girmek ister misiniz?");
	scanf("%d", &a);
	
	
	do{
		
	n+=1;
	
	for(i=0;i<=n;i++){
		
		struct musteri musteri[i];
		
		printf("Yeni musteri giriniz:");
		scanf("%s", &musteri[i].adSoyad);
		scanf("%d", &musteri[i].id);
		scanf("%d", &musteri[i].type);
		scanf("%d", &musteri[i].dg);
		
		printf("%s\n%d\n%d\n%d\n", musteri[i].adSoyad, musteri[i].id, musteri[i].type, musteri[i].dg);
		
		}
		
	printf("Devam mi?");
	scanf("%d", &a);
	
	}while(a==1);
	
	return 0;
}
