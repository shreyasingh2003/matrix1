import java.io.*;
class matrix1
{
	 int[][] mat1;
	 int row,col;
	 
	 matrix1(int i, int j)
	 {
		 row=i;
		 col=j;
		 mat1= new int[row][col];
		 
	 }
	 void input() throws IOException
	 {
		 BufferedReader br = new
					BufferedReader(new InputStreamReader(System.in));
		 System.out.println("ENTER THE ELEMENT OF MATRIX :");
		 for(int i=0 ; i<row ; i++) {
			 for(int j=0; j<col ; j++) {
				 mat1[i][j]=Integer.parseInt(br.readLine());
			 }
		 }
	 }
	//cpmstructor to initialize another object
	matrix1 add(matrix1 o1)
	{
		matrix1 temp;
		temp= new matrix1(o1.row,o1.col);
		 for(int i=0; i<row ; i++) {
			 for(int j=0 ; j<col ; j++) {
				 temp.mat1[i][j]=mat1[i][j]+o1.mat1[i][j];
				 
		
		
		 }
		 }
		 return temp;
		
		
	}
	matrix1 multiply(matrix1 o1)
	{
		matrix1 temp= new matrix1(row,o1.col);
		for(int i=0; i<row ; i++) {
			 for(int j=0 ; j<o1.col ; j++) {
				 temp.mat1[i][j]=0;
				 for(int k=0;k<col;k++)
					 temp.mat1[i][j]+=mat1[i][k]*o1.mat1[k][j];
			 }
		
				
		
	}
		return temp;
	}
	void display()
	{
		 for(int i=0; i<row ; i++) {
			 for(int j=0 ; j<col ; j++) {
					 
				 System.out.print(mat1[i][j]+"\t");
			 }
			 System.out.println();
		 }
		
	}
}
 class matrixclass{

	public static void main(String[] args) 
	throws IOException{
		BufferedReader br = new
				BufferedReader(new InputStreamReader(System.in));
	System.out.println(" Enter  number of rows : ");
		int row = Integer.parseInt(br.readLine());
		 System.out.println("Enter number of columns : ");
		 int col= Integer.parseInt(br.readLine());
		
		matrix1 o1,o2,o3;
		o1= new matrix1(row,col);
		o2= new matrix1(row,col);
		 o1.input();
		 o2.input();
		 o3=o1.add(o2);
		 System.out.println("First matrix");
		 o1.display();
		 System.out.println("Second matrix");
		 o2.display();
		 System.out.println("Matrix addition ");
		 o3.display();
	matrix1 o4,o5,o6;
	o4 = new matrix1(row,col);
	o5= new matrix1(row,col);
	o4.input();
	o5.input();
	o6= o4.multiply(o5);
	System.out.println("First matrix");
	o4.display();
	System.out.println("Second matrix");
	o5.display();
	System.out.println("Matrix multiplication");
	o6.display();		 
}
}
