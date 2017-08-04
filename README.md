
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

<html lang="en">

<head>

<link rel="apple-touch-icon" href="http://algs4.cs.princeton.edu/apple-touch-icon.png"></link>
<link rel="shortcut icon"    href="http://algs4.cs.princeton.edu/favicon.ico"></link>

<link rel="stylesheet"       href="http://algs4.cs.princeton.edu/algs4.css" type="text/css" media="screen"></link>

<meta name="google-site-verification" content="nYspbl5bNBQrNZKguiAAFTMVM7sq2P1WQYc8Oi6Okl0" />
<meta name="msvalidate.01" content="D4B7F6DF793EFF34DE96F611C2A367A5" />

<!-- IE HACKS -->
<!--[if IE]>
<style type="text/css" media="screen">
 #menu ul li {float: left; width: 100%;}
</style>
<![endif]-->
<!--[if lt IE 7]>
<style type="text/css" media="screen">
body {
behavior: url(/csshover.htc);
} 
#menu ul li {float: left; width: 100%;}
#menu ul li a {height: 1%;} 

#menu a, #menu h2 {
font: bold 0.9em/1.5em arial, helvetica, sans-serif;
} 

</style>
<![endif]-->



<title>
Data Abstraction</title>

<META HTTP-EQUIV="Content-Type" content="text/html; charset=iso-8859-1">
<META NAME="AUTHOR" CONTENT="Robert Sedgewick and Kevin Wayne">
<META NAME="KEYWORDS" CONTENT="Data Abstraction,Algorithms,4th edition,data structures,Java,intro,introduction,Sedgewick,Wayne">
<META NAME="DESCRIPTION" CONTENT="The textbook Algorithms, 4th Edition by Robert Sedgewick and Kevin Wayne surveys the most important algorithms and data structures in use today. The broad perspective taken makes it an appropriate introduction to the field.">
<META NAME="TITLE" CONTENT="Data Abstraction. Algorithms, 4th Edition by Robert Sedgewick and Kevin Wayne.">
<META NAME="ROBOTS" CONTENT="INDEX,FOLLOW">

<script type='text/javascript' src='/media/swfobject.js'></script>
<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'UA-10811519-2', 'auto');
  ga('send', 'pageview');

</script>

</head>


<body>

<div id = "menu">
<div align="center">
<a class = picture href = "http://algs4.cs.princeton.edu">
<img src="http://algs4.cs.princeton.edu/cover.png" width=189 height=236 border=0 alt = "Algorithms, 4th Edition by Robert Sedgewick and Kevin Wayne">
</a>  
</div>





<ul>
  <li><a class = title href = "http://algs4.cs.princeton.edu">Algorithms, 4th edition</a>

<ul>


      <li> <a href = "/10fundamentals">1.&nbsp;&nbsp;Fundamentals</a>
        <ul>
          <li> <a href = "/11model">1.1&nbsp;&nbsp;Programming Model</a>
          <li> <a href = "/12oop">1.2&nbsp;&nbsp;Data Abstraction</a>
          <li> <a href = "/13stacks">1.3&nbsp;&nbsp;Stacks and Queues</a>
          <li> <a href = "/14analysis">1.4&nbsp;&nbsp;Analysis of Algorithms</a>
          <li> <a href = "/15uf">1.5&nbsp;&nbsp;Case Study: Union-Find</a>
        </ul>

      <li> <a href = "/20sorting">2.&nbsp;&nbsp;Sorting</a>
        <ul>
          <li> <a href = "/21elementary">2.1&nbsp;&nbsp;Elementary Sorts</a>
          <li> <a href = "/22mergesort">2.2&nbsp;&nbsp;Mergesort</a>
          <li> <a href = "/23quicksort">2.3&nbsp;&nbsp;Quicksort</a>
          <li> <a href = "/24pq">2.4&nbsp;&nbsp;Priority Queues</a>
          <li> <a href = "/25applications">2.5&nbsp;&nbsp;Sorting Applications</a>
        </ul>

      <li> <a href = "/30searching">3.&nbsp;&nbsp;Searching</a>
        <ul>
          <li> <a href = "/31elementary">3.1&nbsp;&nbsp;Symbol Tables</a>
          <li> <a href = "/32bst">3.2&nbsp;&nbsp;Binary Search Trees</a>
          <li> <a href = "/33balanced">3.3&nbsp;&nbsp;Balanced Search Trees</a>
          <li> <a href = "/34hash">3.4&nbsp;&nbsp;Hash Tables</a>
          <li> <a href = "/35applications">3.5&nbsp;&nbsp;Searching Applications</a>
        </ul>

      <li> <a href = "/40graphs">4.&nbsp;&nbsp;Graphs</a>
        <ul>
          <li> <a href = "/41graph">4.1&nbsp;&nbsp;Undirected Graphs</a>
          <li> <a href = "/42digraph">4.2&nbsp;&nbsp;Directed Graphs</a>
          <li> <a href = "/43mst">4.3&nbsp;&nbsp;Minimum Spanning Trees</a>
          <li> <a href = "/44sp">4.4&nbsp;&nbsp;Shortest Paths</a>
        </ul>

      <li> <a href = "/50strings">5.&nbsp;&nbsp;Strings</a>
        <ul>
          <li> <a href = "/51radix">5.1&nbsp;&nbsp;String Sorts</a>
          <li> <a href = "/52trie">5.2&nbsp;&nbsp;Tries</a>
          <li> <a href = "/53substring">5.3&nbsp;&nbsp;Substring Search</a>
          <li> <a href = "/54regexp">5.4&nbsp;&nbsp;Regular Expressions</a>
          <li> <a href = "/55compression">5.5&nbsp;&nbsp;Data Compression</a>
        </ul>

      <li> <a href = "/60context">6.&nbsp;&nbsp;Context</a>
        <ul>
          <li> <a href = "/61event">6.1&nbsp;&nbsp;Event-Driven Simulation</a>
          <li> <a href = "/62btree">6.2&nbsp;&nbsp;B-trees</a>
          <li> <a href = "/63suffix">6.3&nbsp;&nbsp;Suffix Arrays</a>
          <li> <a href = "/64maxflow">6.4&nbsp;&nbsp;Maxflow</a>
          <li> <a href = "/65reductions">6.5&nbsp;&nbsp;Reductions</a>
          <li> <a href = "/66intractability">6.6&nbsp;&nbsp;Intractability</a>
        </ul>
    </ul>




<li><a class = title> Related Booksites</a>
<table width = 100% border = 0 cellspacing = 0 cellpadding = 0>
<tr>
<td align = center>
<a class = booksite href = "http://introcs.cs.princeton.edu">
   <img src = "http://introcs.cs.princeton.edu/java/cover.png"
        width = 80 height = 108 border=0
        alt = "Introduction to Programming in Java
               by Robert Sedgewick and Kevin Wayne">
</a>
<td align = center>
<a class = booksite href = "http://aofa.cs.princeton.edu">
   <img src = "http://algs4.cs.princeton.edu/cover-analysis-of-algorithms.png"
        width = 81 height = 108 border=0
        alt = "An Introduction to the Analysis of Algorithms by Robert Sedgewick and Philippe Flajolet">
</a>
</tr>
</table>

<li><a class = title>Web Resources</a>


      <li> <a href = "/faq">FAQ</a>
      <li> <a href = "http://introcs.cs.princeton.edu/java/data">Data</a>
      <li> <a href = "/code">Code</a>
      <li> <a href = "/errata">Errata</a>
      <li> <a href = "/cheatsheet">Cheatsheet</a>
      <li> <a href = "/references">References</a>
      <li> <a href = "https://www.coursera.org/course/algs4partI">Online Course</a>
      <li> <a href = "/lectures">Lecture Slides</a>
      <li> <a href = "http://introcs.cs.princeton.edu/java/assignments">Programming Assignments</a>
   </ul>

</ul>

<p><br>

<script>
  (function() {
    var cx = '005649317310637734940:s7fqljvxwfs';
    var gcse = document.createElement('script');
    gcse.type = 'text/javascript';
    gcse.async = true;
    gcse.src = (document.location.protocol == 'https:' ? 'https:' : 'http:') +
        '//www.google.com/cse/cse.js?cx=' + cx;
    var s = document.getElementsByTagName('script')[0];
    s.parentNode.insertBefore(gcse, s);
  })();
</script>
<gcse:searchbox-only></gcse:searchbox-only>

<p><br>




</div>


<div id = "content">
<h1>1.2 &nbsp; Data Abstraction</h1>

<p><br>
<h2>Object-oriented programming.</h2>

Programming in Java is largely based on building data types.
This style of programming is known as <em>object-oriented programming</em>,
as it revolves around the concept of an <em>object</em>,
an entity that holds a data type value. With Java's 
primitive types we are largely confined to programs that operate on numbers,
but with reference types we can write programs that operate on strings, pictures,
sounds, or any of hundreds of other abstractions that are available
in Java's standard libraries or on our booksite.
Even more significant than libraries of predefined data types is that the range of 
data types available in Java programming is open-ended, because you can
define your own data types.

<ul>

<p><li><em>Data types.</em>
A <em>data type</em> is a set of values and a set of
operations on those values.

<p><li><em>Abstract data types.</em>
An <em>abstract data type</em> is a data type whose internal
representation is hidden from the client.

<p><li><em>Objects.</em>
An <em>object</em> is an entity that can take on a data-type value.
Objects are characterized by three essential properties:
The <em>state</em> of an object is a value from its data type;
the <em>identity</em> of an object distinguishes one object from another;
the <em>behavior</em> of an object is the effect of data-type operations.
In Java, a <em>reference</em> is a mechanism for accessing an object.


<p><li><em>Applications programming interface (API).</em>
To specify the behavior of an abstract data type,
we use an <em>application programming interface</em> (API), 
which is a list of <em>constructors</em> and <em>instance methods</em>
(operations), with an informal description of the effect of each,
as in this API for <tt>Counter</tt>:

<p><center>
<IMG SRC="images/counter-api.png" alt = "api for counter">
</center>

<p><li><em>Client.</em>
A client is a program that uses a data type.

<p><li><em>Implementation.</em>
An implementation is the code that implements the data type specified in an API.

</ul>



<p><h2>Using abstract data types.</h2>
A client does not need to know how a data type is implemented
in order to be able to use it.

<ul>


<p><li><em>Creating objects.</em>
 Each data-type value is stored in an object.
To create (or <em>instantiate</em>) an individual object,
we invoke a <em>constructor</em> by using the keyword <tt>new</tt>.
Each time that a client uses <tt>new</tt>, the system
allocates memory space for the object, initializes its value,
and returns a reference to the object.

<p><center>
<IMG SRC="images/constructor.png" alt = "constructor">
</center>

<p><li><em>Invoking instance methods.</em>
The purpose of an instance method is to operate on data-type values.
Instance methods have all of 
the properties of static methods: arguments are passed by value, 
method names can be overloaded, they may have a return value, and they may cause side 
effects. They have an additional property that characterizes them:
<em>each invocation is associated with an object</em>. 

<p><center>
<IMG SRC="images/instance-method.png" alt = "instance method">
</center>

<p><li><em>Using objects.</em>
Declarations give us variable names for objects that we can use in code.
To use a given data type, we:
<ul>
<p><li> Declare variables of the type, for use in referring to objects
<p><li> Use the keyword <tt>new</tt> to invoke a constructor that
creates objects of the type
<p><li> Use the object name to invoke instance methods,
either as statements or within expressions
</ul>

<p>
For example,
<a href = "Flips.java.html">Flips.java</a> is a 
<a href = "Counter.java.html">Counter.java</a> client that 
takes a command-line argument <tt>T</tt> and simulate <tt>T</tt> coin flips.


<p><li><em>Assignment statements.</em>
An assignment statement with a reference type creates a copy of the reference
(and does not create a new object).
This situation is known as <em>aliasing</em>:
both variables refer to the same object.
Aliasing is a common source of bugs in Java programs,
as illustrated by the following example:

<blockquote>
<table>
<TR><TD><pre>
Counter c1 = new Counter("ones");
c1.increment();
Counter c2 = c1;
c2.increment(); 
StdOut.println(c1);
</pre></td></tr>
</table>
</blockquote>

The code prints the string <tt>"2 ones"</tt>.


<p><li><em>Objects as arguments.</em>
You can pass objects as arguments to methods.
Java passes a <em>copy</em> of the argument value from the calling program to the method.
This arrangement is known as <em>pass by value</em>.
If you pass a reference to an object of type <tt>Counter</tt>, Java
passes a copy of that reference. Thus, the method cannot change the original reference
(make it point to a different <tt>Counter</tt>), but it can change the 
value of the object, for example by using the reference to call <tt>increment()</tt>.

<p><li><em>Objects as return values.</em>
You can also use an object as a return value from a method. The method 
might return an object passed to it as an argument, as in 
<a href = "FlipsMax.java.html">FlipsMax.java</a>, or it might 
create an object and return a reference to it.
This capability is important because Java 
methods allow only one return value&mdash;using objects
enables us to write code that, in effect, returns multiple values.

<p><li><em>Arrays are objects.</em>
In Java, every value of any nonprimitive type is an object. In particular,
arrays are objects. As with strings, there is special language support
for certain operations on arrays: declarations, initialization, and indexing. 
As with any other object, when we pass an array 
to a method or use an array variable on the right hand side of an assignment statement, we are 
making a copy of the array reference, not a copy of the array.

<p><li><em>Arrays of objects.</em>
Array entries can be of any type.
When we create an array of objects, we do so in two steps:
create the array, using the bracket syntax for array constructors;
create each object in the array, using a standard 
constructor for each.
<a href = "Rolls.java.html">Rolls.java</a> simulates rolling a die, using an array of 
<tt>Counter</tt> objects to keep track of the number of occurrences
of each possible value. 

</ul>



<p><h2>Examples of abstract data types.</h2>

<ul>

<li><em>Geometric objects.</em>
A natural example of object-oriented programming is designing
data types for geometric objects.
<ul>
<p><li> <a href = "Point2D.java.html">Point2D.java</a> is a data type for points in the plane.
<p><li> <a href = "Interval1D.java.html">Interval1D.java</a> is a data type for 
one-dimensional intervals.
<p><li><a href = "Interval2D.java.html">Interval2D.java</a> is a data type for 
two-dimensional intervals.
</ul>


<li><em>Information processing.</em>
Abstract data types provide a natural mechanism for organizing and
processing information.
the information
<ul>
<p><li> <a href = "Date.java.html">Date.java</a> is a data type
that represents the day, month, and year.

<p><li> <a href = "Transaction.java.html">Transaction.java</a> is a data type 
that represents a customer, a date, and an amount.
</ul>

<li><em>Accumulator.</em>
<a href = "Accumulator.java.html">Accumulator.java</a>
defines an ADT that provides to clients the ability to
maintain a running average of data values.
For example, we use this data type frequently in this book to process
experimental results.
<a href = "VisualAccumulator.java.html">VisualAccumulator.java</a>
in an enhanced version that also plots the data (in gray) and 
the running average (in red).


<p><li><em>Strings.</em>
Java's <tt>String</tt> data type in an important and useful ADT.
A <tt>String</tt> is an indexed sequence of <tt>char</tt> values.
<tt>String</tt> has dozens of instance methods, including the 
following:

<p><center>
<IMG SRC="images/string-api.png" alt = "string api">
</center>

<tt>String</tt> has special language support for initialization
and concatenation: instead of creating and initializing a
string with a constructor, we can use a string literal; 
instead of invoking the method <tt>concat()</tt> we can use the <tt>+</tt>
operator.

<p><li><em>Input and output revisited.</em>
A disadvantage of the <tt>StdIn</tt>, <tt>StdOut</tt>, and <tt>StdDraw</tt>
libraries of Section 1.1 is that they restrict us to working with just
one input file, one output file, and one drawing for any 
given program. With object-oriented programming, we can define
similar mechanisms that allow us to work with <em>multiple</em>
input streams, output streams, and drawings within one program. 
Specifically, our standard library includes the data types
<a href = "In.java.html">In.java</a>,
<a href = "Out.java.html">Out.java</a>, and
<a href = "Draw.java.html">Draw.java</a> that
support multiple input and output streams.
</ul>



<p><h2>Implementing abstract data types.</h2>
We implement ADTs with a Java class, putting the code in 
a file with the same name as the class, followed by the .java extension.
The first statements in the file declare <em>instance variables</em>
that define the data-type values. Following the 
instance variables are the <em>constructor</em> and the
<em>instance methods</em> that implement operations on data-type values.

<ul>
<p><li><em>Instance variables.</em>
To define data-type values (the state of each object), we declare 
instance variables in much the same way as we declare local variables.
There are numerous values corresponding to each instance variable (one 
for each object that is an instance of the data type).
Each declaration is qualified 
by a <em>visibility modifier</em>. In ADT implementations, we use <tt>private</tt>,
using a Java language mechanism to enforce the idea that the representation
of an ADT is to be hidden from the 
client, and also <tt>final</tt>, if the value is not to be changed once
it is initialized.

<p><li><em>Constructors.</em>
The constructor establishes an object's identity and
initializes the instance variables.
Constructors always share the same name as the class. We can overload the name 
and have multiple constructors with different signatures, just as with methods. If no other 
constructor is defined, a default no-argument constructor is
implicit, has no arguments, and initializes instance values to default values. The default 
values of instance variables are 0 for primitive numeric types, <tt>false</tt>
for <tt>boolean</tt>, and <tt>null</tt>.


<p><li><em>Instance methods.</em>
Instance methods specify the data-type operations.
Each instance method has a return type, a <em>signature</em>
(which specifies its name and the types and names of its parameter variables),
and a <em>body</em> (which consists of a sequence of statements,
including a <em>return</em> statement that provides a value of the return
type back to the client). 
When a client invokes a method, the parameter values (if any) are initialized with client 
values, the statements are executed until a return value is computed, and the value is 
returned to the client.
Instance methods may be <em>public</em> (specified in the API)
or <em>private</em> (used to organize the computation and not available to clients).

<p><center>
<IMG SRC="images/counter-anatomy.png" alt = "anatomy of a class">
</center>


<p><li><em>Scope.</em>
Instance methods use three kinds of 
variables: parameter variables, local variables, and instance variables.
The first two of these are the same as for static methods:
parameter variables are specified in the method 
signature and initialized with client values when the method is called, and local variables 
are declared and initialized within the method body. The scope of parameter variables is the 
entire method; the scope of local variables is the following statements in the block where 
they are defined. Instance variables hold data-type values 
for objects in a class, and their scope is the entire class (whenever there is an ambiguity, 
you can use the <tt>this</tt> prefix to identify instance variables).

<p><center>
<IMG SRC="images/scope.png" alt = "scope">
</center>


</ul>




<p>

<p><h2>Designing abstract data types.</h2>
We put important information related to designing data types in one place
for reference and to set the stage for implementations 
throughout this book.


<ul>
<p><li><em>Encapsulation.</em>
A hallmark of object-oriented programming is that it enables us to
<em>encapsulate</em> data types within their implementations, to facilitate
separate development of clients and data type implementations.
Encapsulation enables modular programming.

<p><li><em>Designing APIs.</em>
One of the most important and most challenging steps in building modern
software is designing APIs.
Ideally, an API would clearly articulate behavior for all possible 
inputs, including side effects, and then we would have software to check 
that implementations meet the specification. Unfortunately, a 
fundamental result from theoretical computer science known as the 
<em>specification problem</em> implies that this goal is actually 
impossible to achieve. There are numerous potential pitfalls
when designing an API:

<ul>
<p><li> Too hard to implement, making it difficult or impossible to develop.
<p><li> Too hard to use, leading to complicated client code.
<p><li> Too narrow, omitting methods that clients need.
<p><li> Too wide, including a large number of methods not needed
by any client.
<p><li> Too general, providing no useful abstractions.
<p><li> Too specific, providing an abstraction so diffuse as to be useless.
<p><li> Too dependent on a particular representation, therefore not
freeing client code from the details of the representation.
</ul>

<p>
In summary, provide to clients the methods they need and no others.



<p><li><em>Algorithms and ADTs.</em>
Data abstraction is naturally suited to the study of algorithms, because it helps us provide a 
framework within which we can precisely specify both what an algorithm needs to accomplish and 
how a client can make use of an algorithm.
For example, our whitelisting example at the beginning of
the chapter is naturally cast as an ADT client,
based on the following operations:
<ul>
<p><li> Construct a SET from an array of given values.
<p><li> Determine whether a given value is in the set.
</ul>

<p>
These operations are encapsulated in
<a href = "StaticSETofInts.java.html">StaticSETofInts.java</a>
and <a href = "Whitelist.java.html">Whitelist.java</a>.


<p><li><em>Interface inheritance.</em>
Java provides language support for defining relationships among objects, 
known as <em>inheritance</em>.
The first inheritance mechanism that we consider is known as <em>subtyping</em>,
which allows us to specify a relationship between otherwise unrelated
classes by specifying in an <em>interface</em> a set of common methods that 
each implementing class must contain.
We use interface inheritance for 
<em>comparison</em> and for <em>iteration</em>.

<p><center>
<IMG SRC="images/interfaces.png" alt = "Java interfaces used in this book">
</center>




<p><li><em>Implementation inheritance.</em>
Java also supports another inheritance mechanism known as <em>subclassing</em>,
which is a powerful technique that enables a programmer to change behavior
and add functionality without rewriting an entire class from scratch.
The idea is to define a new class (<em>subclass</em>) 
that inherits instance methods and instance variables from another class
(<em>superclass</em>).
We avoid subclassing in this book because it generally works against encapsulation. 
Certain vestiges of the approach are built in to Java and therefore unavoidable: 
specifically, every class is a subclass of
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Object.html">Object</a>.


<p><center>
<IMG SRC="images/inherited.png" alt = "Inherited methods from Object used in this book">
</center>


<p><li><em>String conversion.</em>
Every Java type inherits <tt>toString()</tt> from 
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Object.html">Object</a>.
This convention is the basis for Java's automatic conversion of one operand of the
concatenation operator <tt>+</tt> to a <tt>String</tt> whenever the 
other operand is a <tt>String</tt>.
We generally include implementations of <tt>toString()</tt> that override the 
default, as in <a href = "Date.java.html">Date.java</a> and
<a href = "Transaction.java.html">Transaction.java</a>.

<p><li><em> Wrapper types.</em> Java supplies built-in 
reference types known as <em>wrapper types</em>,
one for each of the primitive types: 

<p>

<center>
<table cellspacing="1" cellpadding="4" border="0" bgcolor="#ffffff">

<tr align=center>
<th align=center width = 150><b>primitive type</b></th>
<th align=center width = 150><b>wrapper type</B></th>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>boolean</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Boolean.html">Boolean</a>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>byte</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Byte.html">Byte</a>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>char</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Character.html">Character</a>
</tr>



<tr align=center bgcolor="#ebebeb">
<td><tt>double</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Double.html">Double</a>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>float</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Float.html">Float</a>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>int</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Integer.html">Integer</a>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>long</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Long.html">Long</a>
</tr>

<tr align=center bgcolor="#ebebeb">
<td><tt>short</tt>
<td><a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Short.html">Short</a>
</tr>

</table>
</center>

<p>
Java automatically converts from primitive types to 
wrapper types (<em>autoboxing</em>) and back (<em>auto-unboxing</em>) when warranted.

<p><li><em>Equality.</em>
What does it mean for two objects to be equal?
If we test equality with <tt>(a == b)</tt>
where <tt>a</tt> and <tt>b</tt> are reference variables of the same type,
we are testing whether they have the same identity: whether the <em>references</em>
are equal.
Typical clients would rather be able to test 
whether the <em>data-type values</em> (object state) are the same.
Every Java type inherits the method <tt>equals()</tt> from 
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/Object.html">Object</a>.
Java provides natural implementations both for
standard types such as <tt>Integer</tt>,
<tt>Double</tt>, and <tt>String</tt>
and for more complicated types such as
<a href = "http://download.oracle.com/javase/6/docs/api/java/io/File.html">java.io.File</a>
and 
<a href = "http://download.oracle.com/javase/6/docs/api/java/net/URL.html">java.net.URL</a>.
When we define our own data types
we need to override <tt>equals()</tt>.
Java's convention is that <tt>equals()</tt> must be an <em>equivalence relation</em>:

<ul>
<p><li> <em>Reflexive</em>: <tt>x.equals(x)</tt> is true.
<p><li> <em>Symmetric</em>: <tt>x.equals(y)</tt> is true if and only if <tt>y.equals(x)</tt>
is true.
<p><li> <em>Transitive</em>: if <tt>x.equals(y)</tt> and <tt>y.equals(z)</tt>
are true, then so is <tt>x.equals(z)</tt>.
</ul>
<p>
In addition, it must take an <tt>Object</tt> as argument and satisfy 
the following properties.
<ul>
<p><li><em>Consistent</em>: multiple invocations of <tt>x.equals(y)</tt> consistently 
return the same value, provided neither object is modified.
<p><li><em>Not null</em>: <tt>x.equals(null)</tt> returns false.
</ul>

<p>
Adhering to these Java conventions can be tricky, as illustrated 
for <a href = "Date.java.html">Date.java</a> and
<a href = "Transaction.java.html">Transaction.java</a>.


<p><li><em>Memory management.</em>
One of Java's most significant features is its ability to <em>automatically</em>
manage memory. When an object can no longer be referenced, it is said to be
<em>orphaned</em>.
Java keeps track of orphaned objects and returning
the memory they use to a pool of free memory.
Reclaiming memory in this way is known as <em>garbage collection</em>.


<p><li><em>Immutability.</em>
An <em>immutable</em> data type has the property that
the value of an object never changes once constructed.
By contrast, a <em>mutable</em> data type
manipulates object values that are intended to change. 
Java's language support for helping to enforce immutability is 
the <tt>final</tt> modifier. When you declare a variable to be <tt>final</tt>,
you are promising to assign it a value only once, either in an initializer
or in the constructor. Code that could modify the 
value of a <tt>final</tt> variable leads to a compile-time error.


<p><a href = "Vector.java.html">Vector.java</a> is an immutable
data type for vectors. In order to guarantee immutability, it
<em>defensively copies</em> the mutable constructor argument.


<p><li><em>Exceptions and errors</em> are disruptive events 
that handle unforeseen errors <em>outside</em> our control.
We have already encountered the following exceptions and errors:
<ul>
<p><li>
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/ArithmeticException.html">ArithmeticException</a>.
Thrown when an exceptional arithmetic condition (such as integer division by zero) occurs.
<p><li>
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/ArrayIndexOutOfBoundsException.html">ArrayIndexOutOfBoundsException</a>.
Thrown when an array is accessed with an illegal index.

<p><li>
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/NullPointerException.html">NullPointerException</a>.
Thrown when <tt>null</tt> is used where an object is required.

<p><li>
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/OutOfMemoryError.html">OutOfMemoryError</a>.
Thrown when the Java Virtual Machine cannot allocate an object because it is out of memory.

<p><li>
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/StackOverflowError.html">StackOverflowError</a>.
Thrown when a recursive method recurs too deeply.
</ul>

<p>
You can also create your own exceptions. The simplest kind is a 
<a href = "http://download.oracle.com/javase/6/docs/api/java/lang/RuntimeException.html">RuntimeException</a>
that terminates execution of the program and prints an error message.

<blockquote>
<table>
<TR><TD><pre>
throw new RuntimeException("Error message here.");
</pre></td></tr>
</table>
</blockquote>


<p><li><em>Assertions</em> are boolean expressions which verify assumptions
that we make <em>within</em> code we develop.
If the expression is false, the program will terminate and report 
an error message.
For example, suppose that you have a computed value that you might use to 
index into an array. If this value were negative, it would cause an 
<tt>ArrayIndexOutOfBoundsException</tt> sometime later.
But if you write the code 

<blockquote>
<table>
<TR><TD><pre>
assert index >= 0; 
</pre></td></tr>
</table>
</blockquote>

you can pinpoint the place where the error occurred.
By default, assertions are disabled.You can enable them from the command line by 
using the <tt>-enableassertions</tt> flag (<tt>-ea</tt> for short).
Assertions are for debugging: your program 
should not rely on assertions for normal operation since they may be disabled.


</ul>





<p>
<h4>Q + A.</h4>
<p>Q. Are there any truly immutable classes in Java?
<p>A. If you use reflection, you can access the <tt>private</tt>
fields of any class and change them.
Program <a href = "MutableString.java.html">MutableString.java</a>
demonstrates how to mutate a <tt>String</tt>.
Program <a href = "MutableInteger.java.html">MutableInteger.java</a>
demonstrates that this is true even if the instance variable is
final.

<h4>Exercises</h4>
<ol>

<a name = "Ex1.2.1"></a>
<p><li value = 1>
Write a <a href = "Point2D.java.html">Point2D.java</a>
client that takes an integer value N from the command line,
generates N random points in the unit square,
and computes the distance separating the closest pair of points.

<a name = "Ex1.2.4"></a>
<p><li value = 4>
What does the following code fragment print?

<blockquote>
<table>
<TR><TD><pre>
String string1 = "hello";
String string2 = string1;
string1 = "world";
StdOut.println(string1);
StdOut.println(string2);
</pre></td></tr>
</table>
</blockquote>

<p><em>Solution:</em> 

<blockquote>
<table>
<TR><TD><pre>
world
hello
</pre></td></tr>
</table>
</blockquote>


<a name = "Ex1.2.6"></a>
<p><li value = 6>
A string s is a <em>circular rotation</em> of a string t if
it matches when the characters are circularly shifted by
any number of positions; e.g., ACTGACG is a circular shift of TGACGAC,
and vice versa.
Detecting this condition is important in the study of genomic sequences.
Write a program that 
checks whether two given strings s and t are circular shifts of one another.

<p><em>Solution:</em> <tt>(s.length() == t.length()) && (s.concat(s).indexOf(t) >= 0)</tt>


<a name = "Ex1.2.7"></a>
<p><li value = 7>
What does the following recursive function return?

<blockquote>
<table>
<TR><TD><pre>
public static String mystery(String s) {
    int N = s.length();
    if (N <= 1) return s;
    String a = s.substring(0, N/2);
    String b = s.substring(N/2, N);
    return mystery(b) + mystery(a);
}
</pre></td></tr>
</table>
</blockquote>

<p><em>Solution:</em> Reverse of the string.

<a name = "Ex1.2.13"></a>
<p><li value = 13>
Using our implementation of <a href = "Date.java.html">Date.java</a> as a model,
develop an implementation of <a href = "Transaction.java.html">Transaction.java</a>.

<a name = "Ex1.2.14"></a>
<p><li value = 14>
Using our implementation of <tt>equals()</tt> in
<a href = "Date.java.html">Date.java</a> as a model,
develop an implementation of <tt>equals()</tt> for
<a href = "Transaction.java.html">Transaction.java</a>.


</ol>

<h4>Creative Problems</h4>
<ol>

<a name = "Ex1.2.16"></a>
<p><li value = 16>
<b>Rational numbers.</b>
Implement an immutable data type 
<a href = "Rational.java.html">Rational.java</a> for rational
numbers that supports addition, subtraction, multiplication, and division.

<p><center>
<IMG SRC="images/rational-api.png" alt = "api for rational numbers">
</center>


You do not have to worry about testing for overflow,
but use as instance variables two <tt>long</tt> values that represent 
the numerator and denominator to limit the possibility of overflow.
Use Euclid's algorithm to ensure that the numerator and 
denominator never have any common factors. Include a test client
that exercises all of your methods.

<a name = "Ex1.2.18"></a>
<p><li value = 18> 
<b>Sample variance for accumulator.</b>
Validate that the following code, which adds the methods <tt>var()</tt>
and <tt>stddev()</tt> to <a href = "Accumulator.java.html">Accumulator.java</a>
to compute the mean, sample variance, and sample standard deviation of the
numbers presented as arguments to <tt>addDataValue()</tt>.

<p><em>Reference:</em> Here is a good
<a href = "http://www.johndcook.com/standard_deviation.html">explanation</a>
of this one-pass method, that was first discovered by Welford in 1962.
This approach can be applied to computing the skewness, kurtosis,
regression coefficients, and Pearson's correlation coefficient.


<a name = "Ex1.2.19"></a>
<p><li value = 19>
<b>Parsing.</b>
Develop the parse constructors for your <a href = "Date.java.html">Date.java</a>
and <a href = "Transaction.java.html">Transaction.java</a> implementations
that take a single <tt>String</tt> argument to specify the initialization values,
using the formats given in the table below.

<p><center>
<IMG SRC="images/parsing.png" alt = "parsing for Date and Transaction">
</center>

</ol>




<br><br>
<p class = footer>
<em>Last modified on August 26, 2016.</em><br><br>
Copyright &copy; 2000&ndash;2016
<a href = "http://www.cs.princeton.edu/~rs" class = footer>Robert Sedgewick</a>
and
<a href = "http://www.cs.princeton.edu/~wayne" class = footer>Kevin Wayne</a>.
All rights reserved.
</div>




<script type="text/javascript">
var gaJsHost = (("https:" == document.location.protocol) ? "https://ssl." : "http://www.");
document.write(unescape("%3Cscript src='" + gaJsHost + "google-analytics.com/ga.js' type='text/javascript'%3E%3C/script%3E"));
</script>
<script type="text/javascript">
try {
var pageTracker = _gat._getTracker("UA-10811519-2");
pageTracker._trackPageview();
} catch(err) {}</script>

</body>

</html>

 
