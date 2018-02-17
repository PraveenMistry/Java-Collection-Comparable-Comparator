# Java-Collection-Comparable-Comparator


Java provides two interfaces to sort objects using data members of the class:

1. Comparable
2. Comparator

1. Comparable Interface
	A comparable object is capable of comparing itself (this) with another object. 
	The class itself must implements the java.lang.Comparable interface to compare its instances
	
2. Comparator Interface

Now, suppose we want sort movies by their rating and names also. 
When we make a collection element comparable(by having it implement Comparable), 
we get only one chance to implement the compareTo() method. The solution is using Comparator.

Unlike Comparable, Comparator is external to the element type we are comparing. 
It’s a separate class. We create multiple separate classes (that implement Comparator) to compare by different members.

Collections class has a second sort() method and it takes Comparator. The sort() method invokes the compare() to sort objects.
