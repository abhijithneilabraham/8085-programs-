
#include<reg51.h>
#define led P0
unsigned char i=0;
void delay (int);

void delay (int d)
{
	unsigned char i=0;
	for(;d>0;d--)
	{
		for(i=250;i>0;i--);
                for(i=248;i>0;i--);
	}
}

void main()
{
	while(1)//// led blink 
	{
	led=0xff;
	delay(1000);
	led=0x00;
	delay(1000);
	++i;
		if(i==7)
		{
			i=0;
			break;
		}
  }
	while(1)//// binary equivalent representation of 1byte data
	{
		led=i++;
		if(i==256)
		{
			i=0;
			break;
		}
		delay(500);
	}
		
	while(1);
}
