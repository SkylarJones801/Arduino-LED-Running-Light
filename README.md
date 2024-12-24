// Define the pins connected to the LEDs
const int ledPins[] = {3, 4, 5, 6, 7, 8, 9};
const int ledCount = sizeof(ledPins) / sizeof(ledPins[0]);

void setup() {
  // Initialize each pin as an output
  for (int i = 0; i < ledCount; i++) {
    pinMode(ledPins[i], OUTPUT);
  }
}

void loop() {
  // Loop through and light up each LED individually
  for (int i = 0; i < ledCount; i++) {
    digitalWrite(ledPins[i], HIGH); // Turn on the current LED
    delay(100);                     // Wait for 100 milliseconds
    digitalWrite(ledPins[i], LOW);  // Turn off the current LED
  }
  delay(100); // Wait for 100 milliseconds

  // Turn on all LEDs simultaneously
  for (int i = 0; i < ledCount; i++) {
    digitalWrite(ledPins[i], HIGH); // Turn on all LEDs
  }
  delay(1000); // Wait for 1 second

  // Turn off LEDs one by one
  for (int i = 0; i < ledCount; i++) {
    digitalWrite(ledPins[i], LOW); // Turn off the current LED
    delay(100);                    // Wait for 100 milliseconds
  }
  delay(1000); // Wait for 1 second

  // Each LED lights up individually 3 times, with a 500ms interval
  for (int i = 0; i < ledCount; i++) {
    for (int j = 0; j < 3; j++) { // Each LED lights up 3 times
      digitalWrite(ledPins[i], HIGH); // Turn on the current LED
      delay(300);                    // Wait for 300 milliseconds
      digitalWrite(ledPins[i], LOW);  // Turn off the current LED
      delay(300);                    // Wait for 300 milliseconds
    }
  }
  // Ensure there is a delay at the end of the loop to provide enough time before the next loop starts
  delay(1000); // Wait for 1 second
}# Arduino-LED-Running-Light
Learn how to use online simulation to create a dynamic Arduino LED running light.
