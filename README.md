# es05

#define button 12
#define led0 2
#define led1 3
#define led2 4

void setup()
{
  pinMode(button, INPUT);
  pinMode(led0, OUTPUT);
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
}

void loop()
{
 
 if(digitalRead(button)== HIGH)
  PORTD = PORTD ^ 0x1C; //MEMORIA CONTRALLA I PIN DA 0 A 7
  delay(100);
 
 
  /*
   if(digitalRead(button)== HIGH)
  PORTD = PORTD ^ 0x1C;*/
}
