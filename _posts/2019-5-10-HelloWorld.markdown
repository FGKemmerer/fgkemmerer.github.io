---
layout: post
title: 1.1 Hello World
---

1.1 Hello World

Buried in these two words I find a nearly irresistible hope for the future. For me, I’ve just taken my “first steps into a larger world”. But even more exciting, that one little program, is saying something too. You might even imagine that the person saying hello was the code, and not the programmer. I know that it is me anthropomorphizing the program, but I remain convinced that from early on the greatest achievement we have hoped for is to create some-thing, some-one like us, who could look out at everything we see and say Hello World.

The gcc likes most of what K&R have to say here. The only difference is that our a.out program wants to be phrased as, 

./a.out

The notes on the use of \n are helpful and as K&R suggest, there are errors if it is neglected. 
Likewise, even if you include the \n but break the line like:

  	printf("hello, world \n
  		   ");

You will still get these sorts of errors from gcc:
  
    1.c:8:9: error: missing terminating " character
    	  printf("hello, world \n
          	   ^~~~~~~~~~~~~~~~
    1.c:9:6: warning: missing terminating " character
    	     ");
     	     ^
    1.c:9:6: error: missing terminating " character
    	      ");
     	      ^~~
   1.c:13:1: error: expected expression before ‘}’ token
       }
       ^
    1.c:13:1: error: expected ‘;’ before ‘}’ token
  
I wonder if this is true of every compiler. In any case I was delighted the first time I saw how the gcc identified erros with the caret symbol ^ follwed by tidles ~~~

So neat!
