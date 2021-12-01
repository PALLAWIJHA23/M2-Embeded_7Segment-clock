#Features:

This is a 7 Segments Clock project, developed from zero, using authoral hardware and software. The clock marks hours, minutes and seconds, using an ATMEGA328P microcontroller, from ATMEL. The 7 Segments Clock was developed as a personal project and it was built on an universal soldering breadboard, according with Proteus folder schematics inside this project. During this README I'll explain how to develop your own 7 Segments Clock. :)

#Utility

The code was developed specifically to ATMEGA328P microcontroller using ATMEL Studio IDE. However, if some changes were made, mainly in initialization, configuration and some registers, the project can be adapted to other microcontroller families, from other manufacturers and IDEs. The idea to build a 7 Segments Clock is the same, but some things will change, like timer registers, I/O and ADC configurations.

##4W 1H:

###WHAT:

A seven-segment display is a form of electronic display device for displaying decimal numerals that is an alternative to the more complex dot matrix displays. Seven-segment displays are widely used in digital clocks, electronic meters, basic calculators, and other electronic devices that display numerical information.

###WHY:

Since the seven-segment circuit is so simple, there is a decreased risk of circuit malfunction due to component failure. Seven-segment LED displays are used in a wide range of environments from very hot to well below freezing that's why we use 7 segment clock.

###WHERE:

7 Segment clock is mainly used in hotels, banks, commercial centers, · stations and airports, · large industrial sites, · control and command centers, · and wherever there is a need to get accurate .

###WHEN:

We use 7 segment clock where we have to displaying numerals that is alternative to the more complex matrix displays.

###HOW:

The clock starts marking time from 00:00, in the moment that it's powered. To adjust time until desired hour and minute you have to use the circuit push buttons (in the right side of microcontroller). We have two push buttons, one to increment hours and another one to increment minutes.

This project algorithm marks hours, minutes and seconds, but it was built only with 4 displays, marking hours and minutes. However, if you want to build a full clock (using seconds markers too) it is only necessary to add two 7 Segments displays and connect it on 2 non used microcontroller ports.

The code was developed with the full clock logic, but when I burn it to microcontroller I comment one of markers (seconds, for example - "CalculateSeconds" function) and it marks Hours + Minutes. In the other hand, if I want to see Minutes + Seconds you need to comment "CalculateHours" function and it will display Minutes + Seconds.

In the moment that the circuit is de-energized, the clock loses its reference and the current time because it does not have a memory hardware implemented in circuit.

However, if you need to store the last marked time, even with the circuit de-energized, you can use a RTC hardware and only read its time variables, than display it in the 7 Segments array. In other way, according to what I said during Binary Clock project (here in github.com/hollwe/binary-clock), I think that this kind of "upgrade" is not interesting to this kind of project because it makes you miss the essence of build a real clock, since thinking in clock logic, counters, timers, until software otimization and implementation. 

##SWOT Analysis:

###Strenghts:

1.It avilable in various colors ,so it looks attractive.
2.It has long life.
3.It provide suoerior readablity during tense.
4.It can help people track the time with the help of a countdown timer.

###Weakness:
1.Some of the 7 segment displays are limited to displaying the 16 hexadecimal characters.
2. The display's internal structure is highly complex.

###Opportunities:
1.It mainly used in digital clocks, electronics meter, and other electronic devices that display numerical imformation.
2.Convenience
3.Anonymity
4.Spreading awareness

###Threats:
1.Lack of evidence-based effectiveness.
2.Acceptance & usablity issues.
3.  Privacy/data secruity

##High Level Requirement:
1.Atmega328p
2.Board
3.Display
4.LED
5.Aurdino

##Low Level Requirement:
1.CAPACITOR
2.RESISTOR
3.BATTERY
4.SOLDERING WIRE
5.JUMPER WIRE









