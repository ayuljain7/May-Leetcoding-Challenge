<head><script type="text/javascript" src="//api-public.addthis.com/url/shares.json?url=http%3A%2F%2Fleetcode.com%2Fexplore%2Fchallenge%2Fcard%2Fmay-leetcoding-challenge%2F536%2Fweek-3-may-15th-may-21st%2F3335%2F&amp;callback=_ate.cbs.rcb_5dt00"></script><script type="text/javascript" src="//graph.facebook.com/?id=http%3A%2F%2Fleetcode.com%2Fexplore%2Fchallenge%2Fcard%2Fmay-leetcoding-challenge%2F536%2Fweek-3-may-15th-may-21st%2F3335%2F&amp;fields=og_object%7Bengagement%7D&amp;callback=_ate.cbs.rcb_iu780"></script><script type="text/javascript" src="//api-public.addthis.com/url/shares.json?url=https%3A%2F%2Fleetcode.com%2Fexplore%2Fchallenge%2Fcard%2Fmay-leetcoding-challenge%2F536%2Fweek-3-may-15th-may-21st%2F3335%2F&amp;callback=_ate.cbs.rcb_dpx70"></script><script type="text/javascript" src="//graph.facebook.com/?id=https%3A%2F%2Fleetcode.com%2Fexplore%2Fchallenge%2Fcard%2Fmay-leetcoding-challenge%2F536%2Fweek-3-may-15th-may-21st%2F3335%2F&amp;fields=og_object%7Bengagement%7D&amp;callback=_ate.cbs.rcb_ezty0"></script><script type="text/javascript" src="https://m.addthis.com/live/red_lojson/300lo.json?si=5ec4ef5609d23b76&amp;bkl=0&amp;bl=1&amp;pdt=2484477&amp;sid=5ec4ef5609d23b76&amp;pub=ra-54828cb901e9e86a&amp;rev=v8.28.5-wp&amp;ln=en&amp;pc=men&amp;cb=0&amp;ab=-&amp;dp=leetcode.com&amp;fp=explore%2Fchallenge%2Fcard%2Fmay-leetcoding-challenge%2F536%2Fweek-3-may-15th-may-21st%2F3335%2F&amp;fr=&amp;of=4&amp;pd=0&amp;irt=1&amp;vcl=1&amp;md=0&amp;ct=1&amp;tct=0&amp;abt=0&amp;cdn=0&amp;pi=1&amp;rb=2&amp;gen=100&amp;chr=UTF-8&amp;colc=1589964630842&amp;jsl=1&amp;uvs=5ec4ef567cb50934000&amp;skipb=1&amp;callback=addthis.cbs.jsonp__7299601192420"></script><script type="text/javascript" src="https://v1.addthisedge.com/live/boost/ra-54828cb901e9e86a/_ate.track.config_resp"></script><script type="text/javascript" src="https://z.moatads.com/addthismoatframe568911941483/moatframe.js"></script></head>
<body>
<h3> Kth Smallest Element in a BST </h3>
<div class="question-description__3U1T"><div><p>Given a binary search tree, write a function <code>kthSmallest</code> to find the <b>k</b>th smallest element in it.</p>

<p><b>Note: </b><br>
You may assume k is always valid, 1 ≤ k ≤ BST's total elements.</p>

<p><strong>Example 1:</strong></p>

<pre><strong>Input:</strong> root = [3,1,4,null,2], k = 1
   3
  / \
 1   4
  \
&nbsp;  2
<strong>Output:</strong> 1</pre>

<p><strong>Example 2:</strong></p>

<pre><strong>Input:</strong> root = [5,3,6,2,4,null,null,1], k = 3
       5
      / \
     3   6
    / \
   2   4
  /
 1
<strong>Output:</strong> 3
</pre>

<p><b>Follow up:</b><br>
What if the BST is modified (insert/delete operations) often and you need to find the kth smallest frequently? How would you optimize the kthSmallest routine?</p>
</div></div>
<div class="hints-area"><div class="css-haw22i"><div class="expandable-panel__YLuE" style="background-color: white; margin-top: 0px;"><div class="center__3_51"><div class="expand-btn__2cag"><span class="text">&nbsp;</span><i class="fa fa-lightbulb-o" aria-hidden="true"></i><span class="text">&nbsp;&nbsp;</span>Hide Hint #1&nbsp;&nbsp;<i class="fa fa-caret-up" aria-hidden="true"></i></div></div><div class="expandable-wrapper__37QK" style="height: 44px;"><div><div class="line__2vww"></div><div class="content__1q_0"><div>Try to utilize the property of a BST.</div></div></div></div></div></div><div class="css-haw22i"><div class="expandable-panel__YLuE" style="background-color: white; margin-top: 0px;"><div class="center__3_51"><div class="expand-btn__2cag"><span class="text">&nbsp;</span><i class="fa fa-lightbulb-o" aria-hidden="true"></i><span class="text">&nbsp;&nbsp;</span>Hide Hint #2&nbsp;&nbsp;<i class="fa fa-caret-up" aria-hidden="true"></i></div></div><div class="expandable-wrapper__37QK" style="height: 44px;"><div><div class="line__2vww"></div><div class="content__1q_0"><div>Try in-order traversal. (Credits to @chan13)</div></div></div></div></div></div><div class="css-haw22i"><div class="expandable-panel__YLuE" style="background-color: white; margin-top: 0px;"><div class="center__3_51"><div class="expand-btn__2cag"><span class="text">&nbsp;</span><i class="fa fa-lightbulb-o" aria-hidden="true"></i><span class="text">&nbsp;&nbsp;</span>Hide Hint #3&nbsp;&nbsp;<i class="fa fa-caret-up" aria-hidden="true"></i></div></div><div class="expandable-wrapper__37QK" style="height: 44px;"><div><div class="line__2vww"></div><div class="content__1q_0"><div>What if you could modify the BST node's structure?</div></div></div></div></div></div><div class="css-haw22i"><div class="expandable-panel__YLuE" style="background-color: white; margin-top: 0px;"><div class="center__3_51"><div class="expand-btn__2cag"><span class="text">&nbsp;</span><i class="fa fa-lightbulb-o" aria-hidden="true"></i><span class="text">&nbsp;&nbsp;</span>Hide Hint #4&nbsp;&nbsp;<i class="fa fa-caret-up" aria-hidden="true"></i></div></div><div class="expandable-wrapper__37QK" style="height: 44px;"><div><div class="line__2vww"></div><div class="content__1q_0"><div>The optimal runtime complexity is O(height of BST).</div></div></div></div></div></div></div></body>