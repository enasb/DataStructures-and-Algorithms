// LowArray.java 
// page44

class LowArray {

  private long[] a ;
  
  // constructor
  public LowArray (int size) {
    a= new long[size] ;
  }
  
  //set value
   public void setElem(int index , long val) {
      a[index] = val ;
   }
   
   // get value
   public long getElem(int index){
    return a[index] ; 
   }
   
} // end of class LowArray

class LowArrayApp {
    
      public static void main() {
      
        LowArray arr = new LowArray(20) ;
        int nelems = 0 ; // number of items in array
        int j;            // loop variable 
        
        // ------------------------------------------------------------------
        // insert 10 items
        
        arr.setElem(0,10);
        arr.setElem(1,5);
        arr.setElem(2,88);
        arr.setElem(3,45);
        arr.setElem(4,77);
        arr.setElem(5,21);
        arr.setElem(6,0);
        arr.setElem(7,34);
        arr.setElem(8,66);
        arr.setElem(9,453);
     
        nelems = 10
        
        //---------------------------------------------------------------------
        // display items
        
        for( j=0 ; j<nelems ; j++){
          System.out.println(arr.getElem(j) + " ") ;
        }
      } // end of main
} // end of LowArrayApp class
