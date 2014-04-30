DICE-TEST--LAB--2--WEEK-11
==========================

DICE TEST LAB #2 - WEEK 11
//  BY REINA OLARTE

// LAB # 2 WEEK 11   "DICE TEST"

import java.util.Scanner;

public class DiceTest 
{
	public static void main( String[]args)	
	{
	Scanner input = new Scanner(System.in);
   //   VARIABLES
	
		int COMPNumber;
		
		int NUMBROLLS;
		
		String Answer;
		
		boolean SIGA = true;
		
			while(SIGA)
		{
		Dice myDice = new Dice();

		System.out.println("How many rolls would you like to play: ");
		NUMBROLLS = input.nextInt();

		myDice.Throw(NUMBROLLS);
		
		COMPNumber = myDice.Value();
		
		System.out.printf("The Number that was rolled from the dice was : %d\n", COMPNumber);
		
		System.out.println("Do you want to continue playing ? YES = Y or NO = N : ");
		
		Answer= input.next();
		
		
			if(Answer.toUpperCase().startsWith("N"))
			{
				SIGA = false;
			}
		}
	}
}
