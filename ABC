#INCLUDE <16F887.H>
#FUSES NOWDT, PUT, HS, NOPROTECT, NOLVP
#USE DELAY(CLOCK=20M)
UNSIGNED INT8 i, Y, j;
VOID MAIN()
{
SET_TRIS_D(0x00);
   WHILE(TRUE)
   {
   Y=0x00;
   OUTPUT_D(Y);
   DELAY_MS(500);
      FOR(j=2;j>0;j--)
      {
      Y=0x00;
      OUTPUT_D(Y);
      DELAY_MS(500);
         FOR(i=0;i<4;i++)
         {
         Y=((Y<<2)|0x03) & 0x7F;
         OUTPUT_D(Y);
         DELAY_MS(500);
         }
         
      }
      FOR(j=2;j>0;j--)
      {
      Y=0x00;
      OUTPUT_D(Y);
      DELAY_MS(500);
         FOR(i=0;i<4;i++)
         {
         Y=(Y>>1)|0x20;
         OUTPUT_D(Y);
         DELAY_MS(500);
         }
      }
      FOR(j=2;j>0;j--)
      {
      Y=0x7F;
      OUTPUT_D(Y);
      DELAY_MS(500);
         FOR(i=0;i<6;i++)
         {
         Y=(Y>>1);
         OUTPUT_D(Y);
         DELAY_MS(500);
         }
      }
   }
}
