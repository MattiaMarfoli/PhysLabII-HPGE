Sorgenti nelle cartelle:
	
NAI: prese con voltaggio a 1kV 



*************************************************

GE: 
	 
Refill post compass:

	1) 19/05  circa alle 12	 
2) 7/06   circa 11 

*** per i dati dell’ultima settimana di misure sono quelli con ultima modifica del 8 giugno ***	


sistemato = girato il programma col nuovo algoritmo (dovrebbe inficiare solo per gain a 30)


Ba133 

	      nomefile         ggmm_gain

           		   
		            *Ba133_THR_10 	1305_30	sistemato  
			*Ba133_THR_10_1    1305_30
			
			Ba133_THR_11       1905_30 sistemato (inutilizzabile)
			
			*Ba133_THR_12      1905_30
			*Ba133_THR_12_1    1905_30 sistemato
			*Ba133_THR_12_2    1905_30
			
			 Ba133_THR_5       2005_10
			 Ba133_THR_5_1     2005_10  sistemato
			 Ba133_THR_5_2     1905_10


 Ba133_THR_9        0806_30 sistemato
			 Ba133_THR_2        0806_10
			 Ba133_THR_3         0806_10
			 Ba133_THR_3_1     0806_10

thresholds del bario compatibili tra loro: 
9,10,12 per gain a 30
5,2,3 per gain a 10 (picchi fino ad 80 keV non visibili)
		fatto	
    ----------------------------------------
         
Co60 

	      nomefile         ggmm_gain
 
		   *Co60_THR_20       2005_10
		   *Co60_THR_20_1     2005_10 sistemato
			
		    Co60_THR_10       1905_10
		    Co60_THR_10_1     1905_10  sistemato


		Co60_THR_9       0806_10   non hanno picchi :(
Co60_THR_15    0806_10   
	
tutti compatibili tra loro	: fatto	
	 ----------------------------------------

Cs137

	      nomefile         ggmm_gain

			 *Cs137_THR_12     1905_30
			 *Cs137_THR_12_1   1905_30    sistemato

			Cs137_THR_9     0806_30
			Cs137_THR_9_1   0806_30
                                     Cs137_THR_9_2     0806_30
 Cs137_THR_9_3   0806_30    sistemato

  			Cs137_THR_3     0806_10   inutilizzabile
 Cs137_THR_3_1   0806_10	

Thresholds a 12 e 9 compatibili tra loro per gain a 30 : fatto

	 ----------------------------------------

Na22

	      nomefile        ggmm_gain

			 *Na22_THR_5      2005_10
			 *Na22_THR_5_1    2005_10 sistemato
			 *Na22_THR_5_2    2005_10

			  Na22_THR_20     2005_10
 
threshold compatibili : fatto

Calibration:

SPOILER SAD: i dati del 08/06 non sono utilizzabili ( evidenziati in azzurro)

PICCHI:

	Na22_THR_5     511keV
	Co60_THR_20    1173keV  
	Ba133_THR_5    30.9keV 34.9keV 53keV 80keV   276keV  302keV 356keV  383keV
	Cs137                  32.194,  ( viene ricostruito male: 661.657)


	“A G=10 i primi 3 picchi del bario non si vedono”				           


Fano:
tutti gain a 10:
Ba133_THR_10000 picchi > 80keV (quello a 383 da togliere)
Co60_THR_10000 2 picchi

[7.27929500e-03 4.27518957e-05 3.66465969e-05 3.13223999e-05
 3.01344588e-06 3.28007994e-06]
S:  0.0009238691979365463 sigma_S: 0.0003803851057854222
n_e:  1.7754998132508368 sigma_n_e: 0.06667790883269534
Fano:  0.31211797227586024 sigma_Fano: 0.12850848168426426

all with E>80keV

TENTATIVI DI CALIBRAZIONE:

Sorgenti  Ba, Cs             gain  30        giorno 19/05
Calibrazione   m: 7.18e+04  +/- 3.86e+02    relative:  0.54 %
q: -1.96e+06  +/- 7.53e+04    relative:  3.84 %
Chi squared reduced: 377815.680           

Sorgenti  Ba, Co, Na           gain  10        giorno 20/05
Calibrazione   m: 2.26e+04  +/- 4.08e+02    relative:  1.81 %
q: -2.02e+06  +/- 1.93e+05    relative:  9.55 %
Chi squared reduced: 2801886.600

Sorgenti  Ba, Co,           gain  10        giorno 19/05
Calibrazione m: 2.27e+04  +/- 4.41e+02    relative:  1.95 %
q: -2.01e+06  +/- 2.06e+05    relative:  10.26 %
Chi squared reduced: 2945639.975



CALIBRAZIONE OGNI SORGENTE PER SE’:

    1) Sorgente: Bario133     gain: 30     giorno:19/05      treshold:12 

picchi:    30.9keV 34.9keV 53keV 80keV   276keV  302keV 356keV  383keV

m: 7.20e+04  +/- 4.50e+02    relative:  0.63 %
q: -2.01e+06  +/- 1.01e+05    relative:  5.00 %
Chi squared reduced: 408751.308

    2) Sorgente: Bario133     gain: 10     giorno:20/05      treshold:5 

picchi:    80keV   276keV  302keV 356keV  383keV

m: 2.05e+04  +/- 3.13e+02    relative:  1.53 %
q: -1.53e+06  +/- 8.38e+04    relative:  5.47 %
Chi squared reduced: 182197.496

    3) Sorgente: Co60    gain: 10     giorno:20/05      treshold: 20 

picchi: 1173.237 keV 1332.501 keV

m: 2.36e+04  +/- inf    relative:  inf %
q: -2.78e+06  +/- inf    relative:  inf %
Chi squared reduced: 0.000

    4) Sorgente: Cs137    gain: 30     giorno:08/06     treshold: 9 

picchi: 32.194 keV , 661.657 keV

m: 6.22e+04  +/- inf    relative:  inf %
q: -1.61e+06  +/- inf    relative:  inf %
Chi squared reduced: 0.000

    5) per il sodio c’è poco da fare: solo un picco è fittabile (quello a 600) quindi un punto per un fit è pochino

