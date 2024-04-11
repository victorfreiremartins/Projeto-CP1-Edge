//Codigo para o sensor LDR Vinheria 

//Declarando as variáveis
const int buzzerPin = 7;
const int ledVermelho = 10;
const int ledAmarelo = 9;
const int ledVerde = 8;

int luminosidade = 0;

//Inicialização do arduino
void setup(){
	Serial.begin(9600); //iniciar a comunicação serial
  	pinMode(ledVermelho, OUTPUT); //indicar a saida de cada pino
    pinMode(ledAmarelo, OUTPUT); //indicar a saida de cada pino
  	pinMode(ledVerde, OUTPUT); //indicar a saida de cada pino 	
}

//Ciclo do Arduino
void loop() {
  int ldrValue = analogRead(A0); // Adicionando a variavel para ler o valor do LDR
  luminosidade = map(ldrValue, 435, 974, 0, 100); //
  Serial.println(luminosidade); //mostrar os valores no monitor serial

  //Luminosidade Alta 
  if (luminosidade > 95)
  {
    digitalWrite(ledVermelho,HIGH); //acender o led para luminosidade alta (ALERTA)
    digitalWrite(ledAmarelo,LOW); //apagar o led
    digitalWrite(ledVerde,LOW); //apagar o led
      
    //Alarme
    tone(buzzerPin,1000); //acionar em um tom de 1000hz
    delay(3000); //adiciona uma espera de 3000ms
    noTone(buzzerPin); //faz o som do buzzer parar
    delay(1000); //tempo de espera ate o buzzer tocar novamente
  }
  
  //Luminosidade média
  if (luminosidade >= 85 && luminosidade <= 95)
  {
    digitalWrite(ledVermelho,LOW); //apagar o led
    digitalWrite(ledVerde,LOW); //apagar o led
    digitalWrite(ledAmarelo,HIGH); //acender o led para luminosidade media (ATENÇÃO)
  }
    
    
  //Baixa luminosidade
  if (luminosidade < 85)
  {
    digitalWrite(ledVermelho,LOW); //apagar o led
    digitalWrite(ledAmarelo,LOW); //apagar o led
    digitalWrite(ledVerde,HIGH); //acender o led para baixa luminosidade (OK) 
  }
}
