<div data-v-5e9078c0=""><h1 data-v-5e9078c0="">
      Top 21 Concurrency interview
      questions and answers in 2021.
    </h1> <p data-v-5e9078c0="" align="center"><a data-v-5e9078c0="" href="https://devinterview.io/"><img data-v-5e9078c0="" src="https://source.unsplash.com/collection/52661698/700x350"></a></p> <p data-v-5e9078c0="">
      You can check all
      21
      Concurrency interview questions here 👉
      https://devinterview.io/design/concurrency-interview-questions
    </p> <br data-v-5e9078c0=""> <div data-v-5e9078c0="" class="unit"><div><h2>🔹 1. What is a Deadlock?</h2></div> <div><h3>Answer:</h3> <div class="answer"><div><div><div class="AnswerBody"><ul><li><p>A <strong>lock</strong> occurs when multiple processes try to access the same resource at the same time. One process loses out and must wait for the other to finish.</p></li><li><p>A <strong>deadlock</strong> occurs when the waiting process is still holding on to another resource that the first needs before it can finish.</p></li></ul><p></p><div><div><div><div></div></div></div></div><p></p><p>So, an example:</p><p>Resource A and resource B are used by process X and process Y</p><ul><li>X starts to use A.</li><li>X and Y try to start using B</li><li>Y 'wins' and gets B first</li><li>now Y needs to use A</li><li>A is locked by X, which is waiting for Y</li></ul><pre><code>Thread 1               Thread 2

Lock1-&gt;Lock();         Lock2-&gt;Lock();
WaitForLock2();        WaitForLock1();   &lt;-- Oops!</code></pre><p>The best way to avoid deadlocks is to avoid having processes cross over in this way. Reduce the need to lock anything as much as you can. In databases avoid making lots of changes to different tables in a single transaction, avoid triggers and switch to optimistic/dirty/nolock reads as much as possible.</p></div></div><div class="row my-2"><div><span><i>Source:</i>&nbsp;<span><a href="https://stackoverflow.com/questions/34512/what-is-a-deadlock" rel="noreferrer" target="_blank" title="What is a Deadlock? Interview Questions Source To Answer">stackoverflow.com</a></span></span>&nbsp; &nbsp;</div></div></div></div></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 2. Explain the difference between Asynchronous and Parallel programming?</h2></div> <div><h3>Answer:</h3> <div class="answer"><div><div><div class="AnswerBody"><p>When you run something <strong>asynchronously</strong> it means it is non-blocking, you execute it without waiting for it to complete and carry on with other things. 
<strong>Parallelism</strong> means to run multiple things at the same time, in parallel. Parallelism works well when you can separate tasks into independent pieces of work. Async and Callbacks are generally a way (tool or mechanism) to express concurrency i.e. a set of entities possibly talking to each other and sharing resources. </p><p>Take for example rendering frames of a 3D animation. To render the animation takes a long time so if you were to launch that render from within your animation editing software you would make sure it was running <em>asynchronously</em> so it didn't lock up your UI and you could continue doing other things. Now, each frame of that animation can also be considered as an individual task. If we have multiple CPUs/Cores or multiple machines available, we can render multiple frames in <em>parallel</em> to speed up the overall workload.</p></div></div><div class="row my-2"><div><span><i>Source:</i>&nbsp;<span><a href="https://stackoverflow.com/questions/6133574/how-to-articulate-the-difference-between-asynchronous-and-parallel-programming#:~:text=13%20Answers&amp;text=When%20you%20run%20something%20asynchronously,into%20independent%20pieces%20of%20work." rel="noreferrer" target="_blank" title="Explain the difference between Asynchronous and Parallel programming? Interview Questions Source To Answer">stackoverflow.com</a></span></span>&nbsp; &nbsp;</div></div></div></div></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 3. What is a Mutex?</h2></div> <div><h3>Answer:</h3> <div class="answer"><div><div><div class="AnswerBody"><p>A <strong>Mutex</strong> is a mutually exclusive object. It acts as a gate keeper to synchronise two threads. When you have two threads attempting to access a single resource, the general pattern is to have the first block of code attempting access, to set the <em>mutex</em> before entering the code. When the second code block attempts access, it sees that the <em>mutex</em> is set and waits until the first block of code is complete (and un-sets the mutex), then continues.</p><p>Specific details of how this is accomplished obviously varies greatly by programming language.</p><p></p><div><div><div><div></div></div></div></div><p></p></div></div><div class="row my-2"><div><span><i>Source:</i>&nbsp;<span><a href="https://stackoverflow.com/questions/34524/what-is-a-mutex" rel="noreferrer" target="_blank" title="What is a Mutex? Interview Questions Source To Answer">Stackoverflow.com</a></span></span>&nbsp; &nbsp;</div></div></div></div></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 4. Is there any difference between a Binary Semaphore and Mutex?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 5. What is a Race Condition?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 6. Write a function that guarantees to never return the same value twice</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 7. Explain Deadlock to 5 years old</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 8. What is the meaning of the term “Thread-Safe”?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 9. How much work should I place inside a lock statement?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 10. What is the difference between Concurrency and Parallelism?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 11. What's the difference between Deadlock and Livelock?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 12. What are some advantages of Lockless Concurrency?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 13. What is Green Thread?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 14. What is a Data Race?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div><div data-v-5e9078c0="" class="unit"><div><h2>🔹 15. What is Starvation?</h2></div> <div>
    👉🏼 Check
    <a href="https://devinterview.io/design/concurrency-interview-questions">all 21 answers</a></div> <br><br></div> <div data-v-5e9078c0="" class="end"></div> <br data-v-5e9078c0="">
    Thanks 🙌 for reading and good luck on your next tech interview!
    <br data-v-5e9078c0="">
    Explore 3800+ dev interview question here 👉
    <a data-v-5e9078c0="" href="https://devinterview.io/">Devinterview.io</a></div>
