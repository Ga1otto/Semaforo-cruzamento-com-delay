# Semáforo cruzamento com delay
 Primeiro repositório curso git e github

void setup() 
{
  pinMode(13, OUTPUT); //define o pino 13 como saída
  pinMode(5, OUTPUT); //define o pino 5 como saída
  pinMode(6, OUTPUT); //define o pino 6 como saída
  pinMode(7, OUTPUT); //define o pino 7 como saída
  pinMode(11, OUTPUT); //define o pino 11 como saída
  pinMode(12, OUTPUT); //define o pino 12 como saída
}

void loop()
{
  digitalWrite(13, HIGH);
  digitalWrite(5, HIGH);
  delay(3000); // Wait for 3000 millisecond(s)
  digitalWrite(5, LOW);
  digitalWrite(6, HIGH);
  delay(2000); // Wait for 2000 millisecond(s)
  digitalWrite(13, LOW);
  digitalWrite(6, LOW);
  digitalWrite(7, HIGH);
  digitalWrite(11, HIGH);
  delay(3000); // Wait for 3000 millisecond(s)
  digitalWrite(11, LOW);
  digitalWrite(12, HIGH);
  delay(2000); // Wait for 2000 millisecond(s)
  digitalWrite(12, LOW);
  digitalWrite(7, LOW);