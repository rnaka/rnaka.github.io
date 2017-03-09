---
layout: essay
type: essay
title: Coding Standards
date: 2017-02-09
labels:
- Software Engineering
- ESLint
- IntelliJ
---

<b>Configuration Management</b>

In the lesson by Philip Johnson on coding standards, he brings up several good points on the importance of coding standards, which include the following: 

<ul>
<li>Improved readability</li>
<li>Detect and remove generic coding mistakes</li>
</ul>

I, myself, believe that coding standards is very important because of the ease in reading code. One of the most important coding standards I hold myself to is the spacing. For example, let's look at the followig code:

```ruby
function fibberoo (val1, val2) {
	let fib = [];
	let first = val1;
	let second = val2;
	fib.push(first, second);
	for (let i = 0, i < 100, i++){
		const temp = first + second;
		fib.push(temp);
		first = second;
		second = temp;
	}
	return fib;
}
```

This code is easy to read because of the spacing and alignment of the code. The spacing also allow us to find any mistakes easily. Without the spacing, the code would be very hard to read, thus hard for us to fix the code if there is a problem. The next example shows the above code, but without the correct spacing and with an error in it. 

function fibberoo (val1, val2) {<br/>
let fib = [];<br/>
let first = val1;<br/>
let second = val2;<br/>
fib.push(first, second);<br/>
for (let i = 0, i < 100, i++){<br/>
const temp = first + second;<br/>
fib.push(temp);<br/>
first = second;<br/>
second = temp;<br/>
return fib;<br/>
}<br/>

In the above example, the following code wouldn't have been able to compile due to a missing bracket. Was it hard to find the mistake in this code? This was just a minor problem, but if you have program that is 100+ lines, it would have been very difficult to find without the proper coding standards, which is more than just the spacing. 

For me, I was lucky to have had a great teacher when I started to learn how to program. My first computer science program was at the University of New Mexico and the teacher I had was very strict with how we organized our code and how we did it. For example, we were never allowed to use the tab button to put spaces. He was very specific and wanted us to have two spaces instead of the tab space. At first, I didn't understand the importance of doing things in that way. In fact, I hated it since I always managed to forget to do one thing or another. However, we eventually came to the point where we had to work with partners and read code from other people. During that time, I was greatful to see that my partner followed the coding standards of my teacher because when we came across a problem, it was easy to spot (although it wasn't always easy for us to fix). However, when we did the next project, my partner wasn't soo keen on following our teachers coding standard, which caused me a lot of headache when we had to trouble shoot a problem with our code. I ended up having to go over the entire program to input the proper coding standard and it turned out that we misspelled a couple words. 

This brings me to using ESLint with IntelliJ. Since my first class, I've experienced several different programs that will compile my program or tell me where a problem is and what the problem is. This past week however, I feel that using ESLint is quite helpful, although it is bothersome at times. For example, I had written a program that had gotten a green check without ESLint enabl2ed, however, when I enabled ESLint, I no longer had a green checkmark. In these instances, I get frustrated using ESLint. But for the majority of the time, I'm usually thankful for ESLint since it tells me the exact problem and where the problem is. 

Overall, using coding standards is something I appreciate and am thankful that others follow as well. If not to make the code easier to read, it also makes it helpful for people to troubleshoot, find items in their code, and keep everyone on the same page when working on a big problem. If, at some point, a group of students are working on a large project, it would be much easier for everyone if they had the same coding standard rather than allowing everyone to write their code any way they want. 