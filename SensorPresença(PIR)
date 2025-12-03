#define PIR_PIN 14   // Pino conectado ao sinal do PIR
#define LED_PIN 2    // LED indicador (LED interno do ESP32)

void setup() {
  Serial.begin(115200);

  pinMode(PIR_PIN, INPUT);
  pinMode(LED_PIN, OUTPUT);

  Serial.println("Sensor PIR iniciado...");
}

void loop() {
  int estado = digitalRead(PIR_PIN);

  if (estado == HIGH) {
    Serial.println("💥 Movimento detectado!");
    digitalWrite(LED_PIN, HIGH);
  } else {
    Serial.println("Nenhum movimento...");
    digitalWrite(LED_PIN, LOW);
  }

  delay(300); // Evita poluir o monitor serial
}
