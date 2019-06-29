# studentmarks
checking student marks
package programkey;
import java.util.*; 
public class ExProgram {
		
	    public static void main(String[] args) {
	        Scanner s = new Scanner(System.in);
	        int sum = 0;
	        int count = 0;
	        int numStudents;
	        int score = 0;
	        int average;
	        char letter,A,B,C,D,F;
	        
	        System.out.print("What grade would you like to count? ");
	        letter = (s.nextLine()).charAt(0);
	        
	        System.out.print("How many students are in the class? ");
	        numStudents = Integer.parseInt(s.nextLine());
	        System.out.println();      
	       
	        for(int i = 1; i<=numStudents; i++) {
	           System.out.print("Exam score for student " + i + ": "); 
	           score += s.nextInt();
	        }
	        System.out.println();          
	        System.out.println("Average exam score is " + (score/numStudents)); 
	       
	             if (score <=90) {
	                letter = 'A';
	                count = count + 1;
	                System.out.println(count + " students got a= " + letter);
	                     }
	             else if (score <=80) {
	                letter = 'B';
	                count = count + 1;
	                System.out.println(count + " students got b= " + letter);
	            }else if (score <=50) {
	                letter = 'C';
	                count = count + 1; 
	                System.out.println(count + " students got c =" + letter);
	            }else if (score<= 30) {
	               letter = 'D';
	               count = count + 1; 
	               System.out.println(count + " students got d= " + letter);
	            }else  {
	               letter = 'F';
	               count = count + 1;
	               System.out.println(count + " students got f= " + letter);
	            }    
	    }
	}
	


