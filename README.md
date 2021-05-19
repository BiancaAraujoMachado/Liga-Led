# Liga-Led
Código C- Liga Led

#include "io430.h"

void main( void )
{
  // Stop watchdog timer to prevent time out reset
  WDTCTL = WDTPW + WDTHOLD;

  P1DIR|=0x01;      //Definir pino 0 da porta 1 como saída
  P1OUT=0;          //Zerar saídas
  while(1) {        //Loop infinito
  P1OUT=0x01;       //Ligar Led
  }
}
