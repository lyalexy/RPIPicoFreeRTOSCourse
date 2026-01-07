README.txt Alexy LY F14158806

OS-10 FINAL

AssignmentQueue Project
I make changes in the CounterAgent.cpp and CounterAgent.h files by adding more GPIO assignments to the class.

CounterAgent.cpp

/***
 * Contructor
 * @param gp1 GPIO PAD for 1st LED - units
 * @param gp2 GPIO PAD for 1st LED - 2
 * @param gp3 GPIO PAD for 1st LED - 4
 * @param gp4 GPIO PAD for 1st LED - 8
 * @param gp5 GPIO PAD for 1st LED - 16
 * @param gp6 GPIO PAD for 1st LED - 32
 * @param gp7 GPIO PAD for 1st LED - 64
 */

CounterAgent::CounterAgent(uint8_t gp1, uint8_t gp2, uint8_t gp3, uint8_t gp4, uint8_t gp5, uint8_t gp6, uint8_t gp7) {


	pLedPads[0] = gp1;
	pLedPads[1] = gp2;
	pLedPads[2] = gp3;
	pLedPads[3] = gp4;
	pLedPads[4] = gp5;
	pLedPads[5] = gp6;
	pLedPads[6] = gp7;



CounterAgent.h

	/***
	 * Contructor
	 * @param gp1 GPIO PAD for 1st LED - units
	 * @param gp2 GPIO PAD for 1st LED - 2
	 * @param gp3 GPIO PAD for 1st LED - 4
	 * @param gp4 GPIO PAD for 1st LED - 8
	 * @param gp5 GPIO PAD for 1st LED - 16
 	 * @param gp6 GPIO PAD for 1st LED - 32
 	 * @param gp7 GPIO PAD for 1st LED - 64
	 */
	CounterAgent(uint8_t gp1=0, uint8_t gp2=0, uint8_t gp3=0, uint8_t gp4=0,  uint8_t gp5=0, uint8_t gp6=0, uint8_t gp7=0);



main.cpp

//LED PAD to use
#define LED_PAD				25
#define LED1_PAD			2
#define LED2_PAD			3
#define LED3_PAD			4
#define LED4_PAD			5
#define LED5_PAD			6
#define LED6_PAD			7
#define LED7_PAD			8

void mainTask(void *params){ 
	BlinkAgent blink(LED_PAD);
	CounterAgent counter(LED1_PAD, LED2_PAD, LED3_PAD, LED4_PAD, LED5_PAD, LED6_PAD, LED7_PAD);






JsonCmds / FREERTOSSMP Project
I made the same changes as in AssignmentQueue so I changed the CounterAgent.cpp and CounterAgent.h files by adding more GPIO assignments to the class.

CounterAgent.cpp

/***
 * Contructor
 * @param gp1 GPIO PAD for 1st LED - units
 * @param gp2 GPIO PAD for 1st LED - 2
 * @param gp3 GPIO PAD for 1st LED - 4
 * @param gp4 GPIO PAD for 1st LED - 8
 * @param gp5 GPIO PAD for 1st LED - 16
 * @param gp6 GPIO PAD for 1st LED - 32
 * @param gp7 GPIO PAD for 1st LED - 64
 */

CounterAgent::CounterAgent(uint8_t gp1, uint8_t gp2, uint8_t gp3, uint8_t gp4, uint8_t gp5, uint8_t gp6, uint8_t gp7) {


	pLedPads[0] = gp1;
	pLedPads[1] = gp2;
	pLedPads[2] = gp3;
	pLedPads[3] = gp4;
	pLedPads[4] = gp5;
	pLedPads[5] = gp6;
	pLedPads[6] = gp7;



CounterAgent.h

	/***
	 * Contructor
	 * @param gp1 GPIO PAD for 1st LED - units
	 * @param gp2 GPIO PAD for 1st LED - 2
	 * @param gp3 GPIO PAD for 1st LED - 4
	 * @param gp4 GPIO PAD for 1st LED - 8
	 * @param gp5 GPIO PAD for 1st LED - 16
 	 * @param gp6 GPIO PAD for 1st LED - 32
 	 * @param gp7 GPIO PAD for 1st LED - 64
	 */
	CounterAgent(uint8_t gp1=0, uint8_t gp2=0, uint8_t gp3=0, uint8_t gp4=0,  uint8_t gp5=0, uint8_t gp6=0, uint8_t gp7=0);



main.cpp

//LED PAD to use
#define LED_PAD				0
#define LED1_PAD			2
#define LED2_PAD			3
#define LED3_PAD			4
#define LED4_PAD			5
#define LED5_PAD			6
#define LED6_PAD			7
#define LED7_PAD			8

void mainTask(void *params){ 
	BlinkAgent blink(LED_PAD);
	CounterAgent counter(LED1_PAD, LED2_PAD, LED3_PAD, LED4_PAD, LED5_PAD, LED6_PAD, LED7_PAD);


