Determine-the-Min-and-Max-Numbers
=================================
public class ArrayMarkLoisRazon {
    public static void main(String[] args) {
        int numbers = /*inserting new int[]*/new int[]{20, 25, 13, 82, 45, 73, 23, 55, 95, 33}
        LVCCArrayLoisRazon arr = new LVCCArrayLoisRazon(numbers);
        
        /*assigning element of numbers into max and min value*/
        int min = numbers[0];
        int max = numbers[0];
 
        System.out.println("Smallest Number: " /*calling the determineMin*/ + this.determineMin);
        System.out.println("Largest Number: " /*calling the determineMax*/ + this.determineMax);
    }
}

---------------------------------------------------------------------------------------------------------------------------------
 LVCCArrayLoisRazon.java

public class LVCCArrayLoisRazon {
private int max;
private int min;
private int[] numbers;
 
public LVCCArrayLoisRazon(int[] numbers) {
this.numbers = numbers;
this.determineMin();
this.determineMax();
}
 
private void determineMin() {
int i;
this.min = this.numbers[0];
for (int i = 1; i < this.numbers.length; i++) {
/* adding if else statement*/
/* getting numbers and max/small numbers*/
        if(this.numbers[i] > this.determineMax) 
                this.determineMax = this.numbers[i];
         else if (this.numbers[i] < this.determineMin) 
                this.determineMin = this.numbers[i];
	
	}
}
 
private void determineMax() {
int i;
this.max = this.numbers[0];
for (int i = 1; i < this.numbers.length; i++) {
/* adding if else statement*/
/* getting numbers and max/small numbers*/
		if(numbers[i] > this.determineMax) 
                this.determineMax = numbers[i];
         else if (numbers[i] < this.determineMin) 
                this.determineMin = numbers[i];
	}
}
 
public int getMin() {
return this.min;
}
 
public int getMax() {
return this.max;
	}
}
