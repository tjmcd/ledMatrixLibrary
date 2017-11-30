// Change these numbers based on how your board is made
int numRows = 5;
int numCols = 5;

// Change these pin numbers depending on where you plug the wires onto your Arduino
int cols[] = {6, 7, 8, 9, 10};  // These represent the pins that are connected to the columns on your matrix
int rows[] = {1, 2, 3, 4, 5};   // same as above, but for the rows instead

void setup() {
  // set the column pins as outputs
  for(int c = 0; c < numCols; c++) {
    pinMode(cols[c], OUTPUT);
  }

  // set the row pins as outputs
  for(int r = 0; r < numRows; r++) {
    pinMode(rows[r], OUTPUT);
  }

  for (int i = 0; i < numOfLeads; i++)
    digitalWrite(i, LOW); 
}

void loop() {
  // Choose from the list of functions written below. Feel free to add your own functions and push them to Github!
  allOn();
  
}

void allOn() {
  // Maximizes brightness of LEDs by flashing through the columns really fast
  for(int i = 0; i < 5; i++) {
    digitalWrite(cols[i], HIGH);   
  }

  for(int i = 0; i < 5; i++) {
    digitalWrite(cols[i], LOW);
  }
  
}

/*
 * Currently unfinished, but feel free to play with it
 */
void lightThisLED(int row, int col) {
  digitalWrite(cols[col], HIGH);

  for(int r = 0; r < numRows; r++){
    digitalWrite(rows[r], HIGH);
  }
  digitalWrite(rows[row], LOW);
}
