<h1> Arduino </h1>

For a project in our Research and Development class in school we got to use the arduino.
At first i was struggeling with how to get it to read the code in unity but it works.

So here is a simple to tutorial to make a cube rotate in unity using codebender and arduino.

As i said i use codebender so here is the link: [Codebender.cc](https://codebender.cc/).

This is the code for codebender:
int UD = 0;
int LR = 0;
int GG = 0;
void setup() 

{
Serial.begin(9600);
} 

void loop()
{ 
UD = analogRead(A0);
LR = analogRead(A1);
GG = analogRead(A2);
Serial.print(UD, DEC);
Serial.print(",");
Serial.print(LR, DEC);
Serial.print(","); 
Serial.println(GG, DEC);
delay(200); 
}

After you put this in codebender you have to check which port you put the arduino in you can see that at the top of the screen in codebender.

Then get the [Unity Code](https://github.com/JeffrinDumas/Arduino/blob/master/Assets/Arduino.cs)

put this in a unity projects script.

Check the COM.
If the Number behind COM is different than yours, then you have to change it to yours.

Makes sure the script names match.

Put the script on an 3d object and start the scene.

Controll with the joystick and enjoy.

