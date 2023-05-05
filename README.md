Download Link: https://assignmentchef.com/product/solved-csi121-lab6-lambda-stream-and-recursive
<br>
<ul>

 <li>Familiar with Lambda, Stream and Recursive.</li>

</ul>

<strong>Use Lambda and Stream to convert Q1 and Q2.  </strong>

<strong><u>Q1</u></strong>

int[] values={12,2,9,8,4,65,7,4,2,66,88,11,33,44,55};       double result = 0;      for(int e : values) {        result = result +e;

}

result=result/values.length;

<strong><u>Q2 </u></strong>

Integer[] values={12,2,9,8,4,65,7,4,2,66,88,11,33,44,55};      Set&lt;Integer&gt; a = new TreeSet&lt;&gt;(Arrays.asList(values));     for(int e : a) {

System.out.println(e);

}

<strong><u>Q3: Write the following code and use Lambda and Stream to process its instances</u></strong><strong> </strong>

Given the following CarEngine class

public class CarEngine {     private String engineName;

private int cylinderVolumn; // example 2.4L     private int numberOfCylinder;

private String fuelType;

public CarEngine(String engineName, int cylinderVolumn, int numberOfCylinder, String fuelType) {         this.engineName = engineName;         this.cylinderVolumn = cylinderVolumn;         this.numberOfCylinder = numberOfCylinder;         this.fuelType = fuelType;

}

public String getEngineName() {

return engineName;

}

public void setEngineName(String engineName) {         this.engineName = engineName;

}

public int getCylinderVolumn() {

return cylinderVolumn;

}




public void setCylinderVolumn(int cylinderVolumn) {         this.cylinderVolumn = cylinderVolumn;

}




public int getNumberOfCylinder() {         return numberOfCylinder;

}




public void setNumberOfCylinder(int numberOfCylinder) {         this.numberOfCylinder = numberOfCylinder;

}




public String getFuelType() {

return fuelType;

}




public void setFuelType(String fuelType) {

this.fuelType = fuelType;

}

}




Write the following code in the main method.

<ol>

 <li>Create 5 objects of the car and save them to the HashMap where the key is an engine name (the solution is provided underneath).</li>

</ol>




CarEngine a0 = new CarEngine(“Honda GT”,2500,6,”98″);

CarEngine a1 = new CarEngine(“Hyundai XTX”,2100,6,”98″);

CarEngine a2 = new CarEngine(“Holden TT”,1200,6,”98″);

CarEngine a3 = new CarEngine(“Toyota TX”,900,6,”98″);

CarEngine a4 = new CarEngine(“Tesla GX”,0,0,”Electricity”);




Map&lt;String,CarEngine&gt; ma = new HashMap&lt;&gt;();

ma.put(a0.getEngineName(),a0);          ma.put(a1.getEngineName(),a1);             ma.put(a2.getEngineName(),a2);             ma.put(a3.getEngineName(),a3);

ma.put(a4.getEngineName(),a4);




ma.values().stream() //convert a hashmap to a stream.




<ol start="2">

 <li>Write the code to search the object by the engine name (using Lambda and Stream)</li>

 <li>Write the code to search for the engine that the cylinder volume between 1000 cc. to 2400 cc. and display them to the console. (using Lambda and Stream)</li>

</ol>

<strong><u>Q4: Tower of Hanoi </u></strong>

Tower of Hanoi is a mathematical puzzle where we have three rods and n disks. The objective of the puzzle is to move the entire stack to another rod, obeying the following simple rules:

<ul>

 <li>Only one disk can be moved at a time.</li>

 <li>Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack i.e. a disk can only be moved if it is the uppermost disk on a stack.</li>

 <li>No disk may be placed on top of a smaller disk.</li>

</ul>

Approach :

Write a recursion program to solve the Tower of Hanoi. The program shall ask user to input the number of disks (n) and output the steps to solve the problem (You must use the recursion).




<a href="#_Toc4885">Examples: Input:                    2 </a>

<a href="#_Toc4886">Output: Disk 1 moved from A to     B </a>

<a href="#_Toc4887">        Disk 2 moved from A to     C </a>

<a href="#_Toc4888">        Disk 1 moved from B to     C </a>




Input: 3

<h1><a name="_Toc4886"></a>Output: Disk 1 moved from A to C</h1>

<h2><a name="_Toc4887"></a>        Disk 2 moved from A to B</h2>

Disk 1 moved from C to B         Disk 3 moved from A to C

<h2><a name="_Toc4888"></a>        Disk 1 moved from B to A</h2>

Disk 2 moved from B to C

Disk 1 moved from A to C





