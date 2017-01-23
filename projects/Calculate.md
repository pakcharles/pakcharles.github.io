---
layout: project
type: project
image: images/change.jpg
title: Calculate
permalink: projects/calculate
date: 2016
labels:
  - Java
summary: The assignment that made me become an ICS major.
---

This project is a Java assignment I did in my ICS 111 class. It is a really simple project, but it has a lot of meaning to me. This homework has a lot of meaning to me because it was when I decided that this is the major I wanted to be in. Without going into too much detail, prior to taking ICS 111 I had absolutely no clue what coding was. I had no prior experiences in coding, so this class was truly all brand new to me. Getting back to the point, this was the first assignment I did on my own, and it made me feel really good about the class.

Here is the code:
```
/**
 * @author Charles
 *
 */
public class Homework02 {
  /**
   * @param args
   */
  public static void main(String[] args) {
    System.out.println("How much does the item cost?"); // system will ask how much item cost
    double a = TextIO.getlnDouble(); // user inputs the total of the item
    System.out.println("How much was paid?"); // system will ask how much tender was given
    double b = TextIO.getlnDouble(); // user inputs the amount tendered
    double Change = (b-a); // system will calculate the change
    int dollars = (int) (Change / 1); // system calculate the amount of dollars bills it owes
    System.out.print(dollars); // output the amount of dollars
    System.out.println(" dollars"); // to specify what the number is for
    double Change2 =(Change - dollars); // get the new total without the dollars 
    int quarters = (int)(Change2 / .25); // calculate the amount of quarters it owes
    System.out.print(quarters); // output the amount of quarters
    System.out.println(" quarters"); // specify what the number is for
    double Change3 = Change2 % .25; // get the new total without the quarters
    int dimes = (int)(Change3 / .1); // calculate the amount of dimes it owes
    System.out.print(dimes); //output the amount of dimes
    System.out.println(" dimes"); // specify what the number is for
    double Change4 = Change3 % .1; // get the new total without the dimes
    int nickels = (int)(Change4 / 0.05); // calculate the amount of nickels it owes
    System.out.print(nickels); // output the amount of nickels
    System.out.println(" nickels"); // specify what the number is for
    double Change5 = Change4 % 0.05; // get the new total without the nickels
    int Change6 = (int) Math.round(Change5 * 100); // times the total by 100 and round it to the nearest integer
    int Change7 = (int)(Change6 / 0.01); // calculate the amount of pennies it owes
    int pennies = (int)(Change7 / 100); // divide by 100 because we times it by a 100 earlier
    System.out.print(pennies); // output the amount of pennies
    System.out.println(" pennies"); // specify what the number is for
  }
}
```
My code looks very clunky, but I am proud of it! Of course I could go in there and revise it, but I want to keep it as it to remind myself, and show others that we all have to start somewhere.

