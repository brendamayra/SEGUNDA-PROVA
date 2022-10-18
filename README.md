# SEGUNDA-PROVA

#define BUTTON01 2
#define LED 12

int buttonState = 0;
int state = 0;

void setup()
{
  pinMode(2, INPUT);
  pinMode(LED, OUTPUT);
}

void loop()
{
  buttonState = digitalRead(BUTTON01); // fala que nesse variavel entra o button01 = 2
  
  if (buttonState == HIGH) // buttonstate começa com alta
  {
     for (int i = 0; i < 5; i++)
  {
    digitalWrite(LED, HIGH);
    delay(1000);
    
    digitalWrite(LED, LOW);
    delay(1000);
    
  }
  }
  
}





segundo
#define BUTTON01 2
#define BUTTON02 7
#define LED 12

int buttonState01 = 0;
int buttonState02 = 0;
int state = 0;

void setup()
{
  pinMode(2, INPUT);
  pinMode(7, INPUT);
  pinMode(LED, OUTPUT);
}

void loop()
{
  buttonState01 = digitalRead(BUTTON01);
  buttonState02 = digitalRead(BUTTON02);
  
  if (buttonState01 == HIGH) // se o button01 for em alto ele fica em alta
  {
    digitalWrite(LED, HIGH);
    delay(200);
  }
  else if(buttonState02 == HIGH) // s eo button02 for high ele muda para baixa
  {
    digitalWrite(LED, LOW);
    delay(200);
  }

}
