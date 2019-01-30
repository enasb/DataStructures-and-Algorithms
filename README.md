//DataStructures-and-Algorithms
//chapter2 page41
//Array.java 

class ArrayApp {

public static void main(String[] args) {
Long[] arr = new Long[100] ;
int nelems = 0 ;

//-------------------------------------
arr[0] = 22 ;
arr[1] = 33 ;
arr[2] = 44 ;
arr[3] = 11 ;
arr[4] = 77 ;
arr[5] = 10 ;
arr[6] = 500 ;
arr[7] = 88 ;
arr[8] = 90 ;
arr[9] = 0 ;
nelems = 10 ;
// ------------------------------------------
// display items

for ( int i=0 ; i<nelems ; i++) {
  System.out.println(arr[i] + " ") ;
}

//---------------------------------------------
// find item with key 66
int key=66;
int i ;
for ( i=0 ; i<nelems ; i++) {
  if(arr[i] == key) 
    break;
  }
  
  if(i == nelems) 
          System.out.println("cannot find the item with key = " + key) ; 
  else 
         System.out.println("item found at index = " + i ) ; 

// -------------------------------------------------
// delete item with key 55
key = 55 ;

for(i=0 ; i<nelems ; i++) {
    if(arr[i] == key) 
        break ;
}

int j ;
 for ( j=i ; j<nelems ; j++) {
    arr[j] = arr[j+1] ;
 }
 
 nelems -- ;
 
 // ---------------------------------------------------
 // display items
 for ( i=0 ; i<nelems ; i++) {
  System.out.println(arr[i] + " ") ;
}
} // end main
} // end class 



