package com.Sample.prg;
import java.util.Random;
import java.util.Scanner;
public class RPS {
public static void main(String[] args) {
	Scanner s=new Scanner(System.in);
	System.out.println("*******************************************");
	System.out.println("*   Rock Paper Scissor   *");
	System.out.println("*******************************************");
	int a=10;
	int h=0;
	int A=0;
	int n=0;
	int d=0;
	int t=0;
	int p=0;
	
	while(a>0){
		if(n<5) {
		display();
		System.out.println("Enter your option");
		String c=s.next();
		
		if(c.equals("R")) {
			Random r=new Random();
			int comp=10+r.nextInt(3)+1;
			if(comp==11) {
				System.out.println("You: Rock");
				System.out.println("AI: Rock");
				System.out.println("Game is draw\n");
				System.out.println("total number of games You Win="+h);
				System.out.println("total number of games AI Win="+A);
				System.out.println("total number of games You lost="+p);
				System.out.println("total number of games AI lost="+t);
				d++;
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
				
			}
			if(comp==12) {
				System.out.println("You: Rock");
				System.out.println("AI: Scissor");
				System.out.println("YOU is win\n");
				h++;
				System.out.println("total number of games You Win="+h);
				System.out.println("total number of games AI Win="+A);
				System.out.println("total number of gamesYou lost="+p);
				t++;
				System.out.println("total number of games AI lost="+t);
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
			
			}
			if(comp==13) {
				System.out.println("You: Rock");
				System.out.println("AI: Paper");
				System.out.println("AI is Win\n");
				System.out.println("total number of games You Win="+h);
				A++;
				System.out.println("total number of games AI Win="+A);
				p++;
				System.out.println("total number of games You lost="+p);
				System.out.println("total number of games AI lost="+t);
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
				
			}
			
		}
		if(c.equals("P")) {
			Random r=new Random();
			int comp=20+r.nextInt(3)+1;
			if(comp==21) {
				System.out.println("You: Paper");
				System.out.println("AI: Rock");
				System.out.println("You is Win\n");
				h++;
				System.out.println("total number of games You Win="+h);
				System.out.println("total number of games AI Win="+A);
				System.out.println("total number of games You lost="+p);
				t++;
				System.out.println("total number of games AI lost="+t);
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
				
			}
			if(comp==22) {
				System.out.println("You: Paper");
				System.out.println("AI: Paper");
				System.out.println("Game is draw\n");
				System.out.println("total number of games You Win="+h);
				System.out.println("total number of games AI Win="+A);
				System.out.println("total number of games You lost="+p);
				System.out.println("total number of games AI lost="+t);
				d++;
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
			}
			if(comp==23) {
				System.out.println("You: Paper");
				System.out.println("AI: Scissor");
				System.out.println("AI is Win\n");
				System.out.println("total number of games You Win="+h);
				A++;
				System.out.println("total number of games AI Win="+A);
				p++;
				System.out.println("total number of games You lost="+p);
				System.out.println("total number of games AI lost="+t);
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
			}
			
		}
		if(c.equals("S")) {
			Random r=new Random();
			int comp=30+r.nextInt(3)+1;
			if(comp==31) {
				System.out.println("You: Scissor");
				System.out.println("AI: Paper");
				System.out.println("You is Win\n");
				h++;
				System.out.println("total number of games You Win="+h);
				System.out.println("total number of games AI Win="+A);
				System.out.println("total number of games You lost="+p);
				t++;
				System.out.println("total number of games AI lost="+t);
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
				
			}
			if(comp==32) {
				System.out.println("You: Scissor");
				System.out.println("AI: Rock");
				System.out.println("AI is win\n");
				System.out.println("total number of gamesYou Win="+h);
				A++;
				System.out.println("total number of gamesAI Win="+A);
				p++;
				System.out.println("total number of gamesYou lost="+p);
				System.out.println("total number of games AI lost="+t);
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
				
			}
			if(comp==33) {
				System.out.println("You: Scissor");
				System.out.println("AI: Scissor");
				System.out.println("Game is draw\n");
				System.out.println("total number of games You Win="+h);
				System.out.println("total number of games AI Win="+A);
				System.out.println("total number of games You lost="+p);
				System.out.println("total number of games AI lost="+t);
				d++;
				System.out.println("Number of games draw="+d);
				n++;
				System.out.println("number of games="+n+"\n\n");
			}
			
		}
		}
		
		}
	}
	

public static void display() {
	System.out.println("1. Rock:R");
	System.out.println("2. Paper:P");
	System.out.println("3. Scissor:S");
	System.out.println("________________________________________________________");
}
}
