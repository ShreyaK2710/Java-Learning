package guessinggame;
import javax.swing.*;
public class numberGuesser{
    public static void main(String[] args) {
        int computerNumber=(int)(Math.random()*100+1);
        int userAnswer=0;
        System.out.println("The correct guess is"+computerNumber);
        int count=1;
        while(userAnswer!=computerNumber)
        {
            String response= JOptionPane.showInputDialog(null, "Guess a number between 1 to 100", "Guessing Game", 3);
            userAnswer=Integer.parseInt(response);
            JOptionPane.showMessageDialog(null, ""+determineGuess(userAnswer,computerNumber,count));
            count++;
        }
    }
    public static String determineGuess(int userAnswer,int computerNumber,int count){
        if(userAnswer<=0||userAnswer>100){
            return "Your guess is invalid";
        }
        else if(userAnswer==computerNumber){
            return "Correct!\nTotal Guesses: "+count;
        }
        else if(userAnswer>computerNumber){
            return "Your guess is a bit higher, try again!\nTry Number: "+count;
        }
        else if(userAnswer<computerNumber){
            return "Your guess is a bit lower, try again!\nTry Number: "+count;
        }
        else{
            return "Your guess is incorrect\nTry Number: "+count;
        }
    }
}
