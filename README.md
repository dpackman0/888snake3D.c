//888snake3D.c
//8x8x8 3-dimensional snake game driven by an MCU using C
//Interface undecided. Could use joy stick, push buttons, RS232 keyboard input via teraterminal
//Think about writing some of it either in assembly or with pointers, bytewise shifts to simplify the tail code

//Variable Declaration
bit LEDbus[8][8][8]; //LED grid. One bit representing each LED.
unsigned char PlyrCMD; // use %hhu for printf. 0 = no input, 1-6 for direction, 7 = menu

char rxchar;
char txchar;
int length;
int head

//Funciton Declaration


void main(void)
{
  
}
int numbergen (int food) //uses a "random" number to decide where the next foodpiece will go highest possible value is 0x8E
{
  int food_z;
  int food_y;
  int food_x;
  bit pass;

  
              /*The while loop ensures that the
              food is far enough away from the
              snake head that the player has
              sufficient reaction time. */
  while (pass==0)
  {
    food = t % 01000;
    t=0;
    food_z = food % 010 /*base8*/; //031:base-8::0x19:base-16::25:base-10
    food y = food % 0100 /*base8*/ - food_z;
    food_x = food - food_z - food_y;
    
    if (LEDbus[food_x][food_y][food_z] = 0)
    {
      pass = 1;
    }
    
    else;
  }
food = food_x + food_y + food_z
}
void rxserial (void)
{

}

void /*Timer interrupt name*/ (void)
{
  t++; //time in microseconds or some other arbitrary value
/*the folllowing is a timer-interrupt driven input read*/  
  if (in1+in2+in3+in4+in5+in6+in7>0)
  {
    if (in7 = 1)
    {
      menu();
    }
    else
    {
      while (in1+in2+in3+in4+in5+in6>1)
      {
        if (in1) {PlyrCMD=1}
        if (in2) {PlyrCMD=2}
        if (in3) {PlyrCMD=3}
        if (in4) {PlyrCMD=4}
        if (in5) {PlyrCMD=5}
        if (in6) {PlyrCMD=6}
      }
    }
  }
}
