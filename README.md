int c1 = 5;
int c2 = 4;
int c3 = 3;
int c4 = 2;
int c5 = 1;

int r1= 10;
int r2= 9;
int r3= 8;
int r4= 7;
int r5= 6;

int wait= 250;

// initialize pin mode
void setup() {
pinMode (c1, OUTPUT);
pinMode (c2, OUTPUT);
pinMode (c3, OUTPUT);
pinMode (c4, OUTPUT);
pinMode (c5, OUTPUT);

pinMode (r1, OUTPUT);
pinMode (r2, OUTPUT);
pinMode (r3, OUTPUT);
pinMode (r4, OUTPUT);
pinMode (r5, OUTPUT);


}
// define loop
void loop(){
  smile();

}
// smile function
void smile() {
//c1 + c5
digitalWrite(c1, HIGH);
digitalWrite(c2, LOW);
digitalWrite(c3, LOW);
digitalWrite(c4, LOW);
digitalWrite(c5, HIGH);


digitalWrite(r1, HIGH);
digitalWrite(r2, HIGH);
digitalWrite(r3, HIGH);
digitalWrite(r4, LOW);
digitalWrite(r5, HIGH);

delay (5);

//c2 + c4
digitalWrite(c1, LOW);
digitalWrite(c2, HIGH);
digitalWrite(c3, LOW);
digitalWrite(c4, HIGH);
digitalWrite(c5, LOW);



digitalWrite(r1, LOW);
digitalWrite(r2, LOW);
digitalWrite(r3, HIGH);
digitalWrite(r4, HIGH);
digitalWrite(r5, LOW);

delay (5);
//C3
digitalWrite(c1, LOW);
digitalWrite(c2, LOW);
digitalWrite(c3, HIGH);
digitalWrite(c4, LOW);
digitalWrite(c5, LOW);


digitalWrite(r1, HIGH);
digitalWrite(r2, HIGH);
digitalWrite(r3, LOW);
digitalWrite(r4, HIGH);
digitalWrite(r5, HIGH);
  delay (5);
}
