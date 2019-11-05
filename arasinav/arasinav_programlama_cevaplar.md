Soru 1:

```c++
int  p[]={7,8,9,10,11};
void setup() {
  for(int i=0;i<=4;i++)
    pinMode(p[i], OUTPUT);
}

void loop() {

    for(int i=0; i<=4;i++){
    digitalWrite(p[i], HIGH);
    digitalWrite(p[4-i], HIGH);
    delay(500);
    digitalWrite(p[i], LOW);
    digitalWrite(p[4-i], LOW); }
}
```

---------------------
Soru 3:

```c++
int say=0, artis=1;
void loop(){
for(int i=0;i<4;i++){
 digitalWrite(i,bitRead(say%10,i));
 digitalWrite(i+4,bitRead(say/10,i));}
  say=say + artis;
   
  if(say>=99 || say<=0)
    artis= -artis;  delay(400); 
```

---------------------
Soru 5:

```c++
for(int i=9;i<=11;i++){
rnd = random(0,256);
analogWrite(i,rnd);
}
delay(1000);
```

---------------------
Soru7:

```c++
analog_deger=analogRead(A0);
derece=map(analog_deger, 102, 204, 0, 50);
aci=map(derece, 30,0,0,90);
myservo.write(aci);

delay(100);
```

