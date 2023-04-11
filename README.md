 A mobile device has an in-memory collection B of M external hosts which cannot be visited by
 user. There is a rule that if a host is forbidden, any child hosts are forbidden too.

 For example, if host adult.hb is forbidden, the following hosts are forbidden too:
 images.adult.hb, ringo.adult.hb, video.ringo.adult.hb

 Write an efficient algorithm (in C#):

 ```
 C# class Solution { public static int[] solution(string[] A, string[] B); }
 ```

 that, given a non-empty array A of N hosts, and B of M forbidden hosts, returns a sequence
 consisting of L integers where each integer represents an index of a host in input A array that can
 be visited by user.

 For example, given:
```

 	A[0] = unlock.microvirus.md 	B[0] = microvirus.md
 	A[1] = visitwar.com         	B[1] = visitwar.de
 	A[2] = visitwar.de          	B[2] = piratebay.co.uk
	A[3] = fruonline.co.uk      	B[3] = list.stolen.credit.card.us
 	A[4] = australia.open.com
 	A[5] = credit.card.us

```
 the function should return the array [1, 3, 4, 5], as explained above.

Assume that:

     + N and M are integers within the range [1..100000];
     + L is integer within the range [0..100000];
     + each element of array A is a string with length [2.. 256];
     + each element of collection B is a string with length [2..256].

Complexity:

     + expected worst-case time complexity is O(N + M);
