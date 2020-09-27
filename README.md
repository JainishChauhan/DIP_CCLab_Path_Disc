# DIP_CCLab_Path_Disc
Digital Image Processing Assignment 1

The outputs are already there in the colab.

If the preview doesn't appear in the colab please download the .ipynb file and upload it to your drive and then open it in the colab. 

If you want to reproduce them you can make a copy of this colab and save it. Then run according to below instructions.

Question-1:
Finding path between two pixels with coordinates (x1,y1) and (x2,y2).
Run all cells below Q1 one by one in the colab.

Here I=input image is predefine in first cell and it can be changes there
The function paths(x1,y1,x2,y2,path_type) is the main function
  where, 
         x1=x-coordinate of start pixel
         y1=y-coordinate of start pixel
         x2=x-coordinate of goal pixel
         y2=y-coordinate of goal pixel
         path_type=4 for 4 connected paths
                   8 for 8 connected paths
                   10 for m connected paths


Question-3:
To generate n non overlapping discs in the given input image
Run all cell below Q3 one by one in the colab.
The main function over here is create_discs(M,N,n,r1,r2,mul,border,Vf,Vb)
Run the cell containing this function to see the output image
Change all params below as per the requirement:
M=   #width of image 
N=   #length of image
n=    #number of discs to be added
r1=    #lower limit of radius of the discs
r2=  #upper limit of radius of the discs
mul=1   #initial multiplication factor=1
border= #width of border
Vf=[]    #list of possible intensity values of FG pixels of disc pixels
Vb=[]  #list of possible intensity values of BG pixels

This display output image with discs as required. 
For each run it will give different image in output depending on the initialization and randomly selected centers.


Question-2:
Finding connected components in the input image
Run all cell below Q2 one by one in the colab.
Here cc(I,connectivity,V) is the main function. 
where I=input image array
      connectivity=4 for connected components with 4 connectivity
                  =8 for connected components with 8 connectivity 
     V=list of FG pixel intensity values
     
This function outputs two things: 
1) The number of connected components present in the given image (including 0 set also which is connected component of BG pixels)
2) Dictionary containing key=label of connected component and value=list of pixel coordinates which are part of that connected component

from the above dictionary using "image_from_ccs()" function we can generate labeld image also as shown in the colab


