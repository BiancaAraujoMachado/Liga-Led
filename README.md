# Liga-Led
Código C- Liga Led

#include "io430.h"

void main( void )
{
  // Stop watchdog timer to prevent time out reset
  WDTCTL = WDTPW + WDTHOLD;

  P1DIR|=0x01;
  P1OUT=0;
  while(1) {
  P1OUT=0x01;
  }
}
