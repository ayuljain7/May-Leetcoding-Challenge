<h3> First Bad Version</h3>
<p>You are a product manager and currently leading a team to develop a new product. Unfortunately, the latest version of your product fails the quality check. Since each version is developed based on the previous version, all the versions after a bad version are also bad.</p>

<p>Suppose you have n versions [1, 2, ..., n] and you want to find out the first bad one, which causes all the following ones to be bad.</p>

<p>You are given an API bool isBadVersion(version) which will return whether version is bad. Implement a function to find the first bad version. You should minimize the number of calls to the API.</p>

<p><b>Example:</b></p>
<pre>Given n = 5, and version = 4 is the first bad version.

<code>call isBadVersion(3) -&gt; false
call isBadVersion(5)&nbsp;-&gt; true
call isBadVersion(4)&nbsp;-&gt; true

Then 4 is the first bad version.&nbsp;</code>
</pre>

<h2> Here's my code </h2>
