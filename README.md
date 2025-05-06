# ser321-assignment-3-sockets-tcp-and-udp-parts-solved
**TO GET THIS SOLUTION VISIT:** [SER321 Assignment 3 Sockets TCP and UDP Parts Solved](https://www.ankitcodinghub.com/product/ser321-assignment-3-sockets-tcp-and-udp-parts-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96396&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SER321 Assignment 3 Sockets TCP and UDP Parts Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
<h1>Prerequisites</h1>
<ol>
<li>The assigned readings in module 3 on Canvas</li>
<li>Lecture videos from Canvas</li>
<li>Running and understanding the examples listed on the Canvas 3 Sockets page</li>
<li>Setup of a second device (second computer, AWS EC2, Raspberry PI) – see Canvas for details (should already be done)</li>
<li>Understanding about UDP, TCP, protocols</li>
</ol>
<strong>Learning outcomes of this assignment are:</strong>

<ol>
<li>Understanding how to work with sockets</li>
<li>Understanding how to use TCP and UDP sockets</li>
<li>Comparing UDP and TCP traffic and being able to “simulate” TCP through UDP</li>
<li>Understanding how to create a custom protocol</li>
</ol>
<h1>1 Background</h1>
You are required to implement a server client game and implement both of these yourself. The client and server will need to communicate with each other through a TCP connection and a JSON custom protocol you design.

The game:

We want to implement a simple game that is similar to hangman but is slightly different. The player receives an image of a city or country which represents the word they are trying to guess. For example, they receive an image of Phoenix and need to guess the word ’phoenix’. Like in hangman, the player starts with blanks “_______” when starting a new game. The player can now either guess the word right away or guess a letter. If they guess a letter right, then it will be put into the ’blanks’ in the correct spot. If they guess a word and it’s incorrect, then they will loose points.

The player starts with 10 points and looses when the points are 0 or wins when a word was guessed correctly.

When the game is over the server will ask if the user wants to continue. The client can either continue or decide to quit. This will then end the connection and the server can accept a new client.

<h1>2 Preliminary things</h1>
I strongly advise you to work on Git and GitHub, to version control and also to practice with the given examples first. If you work on GitHub make sure your repository is private. When you submit you can either upload your code into the Assignment 3 folder on GitHub through the web browser or just push it if using Git.

<h2>What you definitely need (20 points)</h2>
<ol>
<li>Structure: you will have to create two programs; one for TCP and one for UDP (more information will follow later in the assignment). Each of these should be in a separate folder called tcp and udp (Assignment3/udp, Assignment3/tcp). You should create the correct folder structure inside these for your projects. Use the given starter code as a guideline. I strongly advise you to look at the following examples in the Sockets directory:
<ol>
<li>JavaSimpleSock</li>
<li>JavaSimpleSock2</li>
<li>SimpleCustomProtocol</li>
<li>AdvancedCustomProtocol</li>
</ol>
</li>
<li>(1.5 points) One Gradle file for the project.</li>
<li>(2 points) Server should run through <em>gradle runServer − Pport </em>= <em>port </em>and the client through <em>gradle runClient − Pport </em>= <em>port − Phost </em>= <em>hostIP</em>.</li>
<li>Default port of 8080 and host “localhost” should be set in Gradle so that we can also run <em>gradle runServer </em>and <em>gradle runClient</em>. Include a link to a short screen capture (4-7min) showing you running both your programs and showing off all your features.</li>
<li>Provide a README.md for each project which includes (most points go towards TCP):
<ol>
<li>(1 points) A description of your project and a detailed description of what it does.</li>
<li>(1.5 points) Include a checklist of the requirements marking if you think you fulfill this requirement or not.</li>
<li>(1 points) An explanation of how we can run the program (hopefully exactly as described in this document).</li>
<li>(3 points) A UML diagram showing the back and forth communication between client and server program. Which UML diagram you use is up to you (just for TCP).</li>
<li>(5 points) A description of your protocol similar to what you usually see when a protocol is described. You should describe each request and all possible responses (including errors). See the add-on video on Canvas on the Sockets page for more details.</li>
<li>(3 points) A link to a video in which you show your program running and all the features.</li>
<li>(2 points) Explain how you designed your program to be robust (see later under constraints).</li>
</ol>
</li>
</ol>
The video is important to help us see how to run your programs. If it is NOT included, we reserve the right to deduct from the next section if we cannot easily find the functionality. We will not hunt for things. Same goes for telling us which requirements you completed and explain your protocol in detail.

We will not debug your code or try to make it run; it either runs through Gradle or it does not. If it does not you will not receive points for the implementation at all. So rather have 50% working than try to get everything done but nothing works.

<h1>3 Activity: The Game (75 points)</h1>
Your game will have a single player acting as the client playing the game.

<ol>
<li><strong><sub>Problem 1: </sub></strong>Create a client-server version of this game over TCP sockets (TCP folder)</li>
<li><strong><sub>Problem 2: </sub></strong>Create a client-server version of this game over UDP sockets (UDP folder) – this will be a simplified version – see later</li>
</ol>
<strong>3.1 Constraints for Problem 1 (65 points) </strong>A couple of things before going over the constraints:

You can skip requirements and continue working on things. Yes, you might lose you points but 80% working is better than being stuck at requirement 2. So check if you can continue or simplify things in case you cannot get something to work.

You should work with the UI given in the starter code, there is a code walk-through video. You can also make a more fancy UI if like, but we tried to keep it very simple. If you cannot figure out the UI, you can just work with the command line but you will loose 10 points from the overall 65 if you do not work with the UI (this is not listed below). When working with the command line the image should still be displayed in a frame (see the AdvancedCustomProtocol for how this could be done). Sending an image is always mandatory!

You can use the UI and integrate the client into it. Choose a server from the given examples and start adapting it to your needs. If you do not use the UI then you can start off with one of the given Client/Server examples and adapt it.

If I say “type X” then X would either be in the command line or in the input field of the UI.

The main part here is to create a Client/Server application. Ensure neither side crashes and is robust even if you might not be able to implement all the functionality.

Important: If you decide to use the networking code from the AdvancedCustomProtocol you will need to add 2-4 minutes to your screencast explaining the networking part of the code and how messages are sent! You will need to show that you actually understand what is going on in these files.

Requirements (I know the points below add up to more than 65, so doing everything perfectly will give you extra credit):

<ol>
<li>(3 points) When the user starts up it should connect to the server. The server will reply by asking for the name of the player.</li>
<li>(3 points) The user should send their name and the server should receive it and greet the user by name.</li>
<li>(4 points) The user should be presented a choice between seeing a leader board or being allowed to guess a city or country (make the interface easy so a user will know what to do).</li>
<li>(4 points) The leader board will show all players that have played since the first start of the server with their name and points. The server will maintain the leader board and send it to the client when requested. You can assume that the same name is the same player.</li>
<li>(2 points) Add on: The leader board is persistent even when the server is restarted (we did not cover this in class yet though) – so this is extra credit.</li>
<li>(6 points) If the user chooses city or county the server will send over an image and the blanks for the word we are searching for.</li>
<li>(5 points) The image should be chosen randomly from the folder, it is ok if you show the same image a couple times, you do not have to keep track of which you already used – you need to print the intended answer in the server terminal to simplify grading for us (this will be worth some points)</li>
<li>(5 points) The user can then do one of three things; enter a letter guess (a one letter response), enter a word (guessing the word), type “quit” to end the game.</li>
<li>(2 points) The user enters a guess (word or letter) and the server must check the guess and respond accordingly.</li>
<li>(2 points) If it is a letter and it is correct +1 point and the letter needs to be displayed in the UI at the correct place.</li>
<li>(2 points) If it is a letter and it is wrong -1 point and the points need to be updated in the UI, the game continues if the user has still more than 0 points.</li>
<li>(2 points) If it is a word and it is correct +5 point and the user is informed and the game ends.</li>
<li>(2 points) If it is a word and it is wrong -5 point and the user needs to be informed, the game continues if the user has still more than 0 points.</li>
<li>(3 points) If the user types “quit” the client disconnects gracefully.</li>
<li>(4 points) The current points the user has have to be displayed in the UI. As soon as a user has 0 points, they lose. As long as they have more than 0 points they are still in the game.</li>
<li>(3 points) If the player won add their new points to their old points on the leader board (or choose the highest value either one). You can assume that their name always identifies them.</li>
<li>Evaluations of the input needs to happen on the server side; the client will not know the images, the corresponding answers, the points, or the leader board. The correct answers should not be sent to the client. No real points for this since if this is not done then you do not really use the client/server correctly. So this will lead to deductions above.</li>
<li>(4 points) Your protocol must be robust. If a command that is not understood is sent to the server or an incorrect parameterization of the command, then the protocol should define how these are indicated. Your protocol must have headers and optionally payloads. This means in the context of one logical message the receiver of the message has to be able to read a header, understand the metadata it provides, and use it to assist with processing a payload (if one is even present). This protocol needs to be described in detail in the README.md.</li>
<li>(7 points) Your programs must be robust. If errors occur on either the client or server or if there is a network problem, you have to consider how these should be handled in the most recoverable and informative way possible. Implement good general error handling and output. Your client/server should not crash even when invalid inputs are provided by the user.</li>
<li>(3 points) After the player wins/loses they can start a new game by entering their name again or they can quit by typing “quit”. After entering their name they can choose start or the leader board again.</li>
<li>(3 points) – advice: skip this until you have everything else then get back to this: If a game is in progress and a second user tries to connect, they should receive a message that a game is already in progress and they cannot connect. How exactly you handle this, whether you let the user wait or just do not let them do anything anymore, is up to you. DO NOT use threads, yes I know I am mean.</li>
</ol>
<h2>3.2 Constraints for Problem 2 (10 points)</h2>
Based on what you have for the TCP part create a second folder and project called UDP. In this version, change the protocol to UDP but you only need to include some parts of the game:

<ul>
<li>The asking and sending of the user’s name</li>
<li>Sending an image from the server to the client</li>
</ul>
You should consider what happens with large pictures in case they do not fit into one package.

In the README.md of this project, explain in detail how your protocol changed compared to TCP. What data do you need to include when you use UDP instead of TCP?

Important: If you decide to use the networking code from the AdvancedCustomProtocol you do need to add 2-4 minutes to your screencast explaining the networking part and how messages are sent! You will need to show that you actually understand what is going on in these files.

<strong>4 Hints:</strong>

These are some hints based on what I saw happening last session and what I do when I implement things. None of the below are requirements; they are tips/hints which you can take or leave.

<ul>
<li>Start slow and with the basics (e.g. setup client/server and send any message back and forth).</li>
<li>You can include the Client directly into the GUI.</li>
<li>For the server, look through the example repo and use a server you like as base.</li>
<li>Work incrementally. Get one message at a time working.</li>
<li>Ignore the images when you get started.</li>
<li>Have Wireshark open to check that messages get out correctly.</li>
<li>Include console outputs to know where you are in the code.</li>
<li>Think about the header and payload construct. You saw this in HTTP, but now you have to do it yourself. Watch the video I added for protocol design for this.</li>
<li>Remember everything explained in the lectures, especially about TCP and UDP.</li>
<li>Use a UML sequence diagram (or at least an informal one) to visualize the backand-forth between the client and server and the places where different outcomes may “branch”.</li>
<li>In your Client and Server, include a status which will tell you if the game has started, etc.</li>
<li>If you cannot get a requirement done, e.g. sending the image, then at least have an image on the client side to display and send over a message “IMAGE” to indicate that you know what is supposed to happen. You will at least get some partial points for this instead of being stuck on this part.</li>
<li>Always check how much each requirement is worth. Requirements do not necessarily depend on each other so you can skip requirements to continue.</li>
<li>To send an image you can look into converting the image into a String to then add to your JSON, or if you send over Bytes you can send it as a Byte stream. That is up to you.</li>
<li>Think of the design criteria: location – ok we will just use IP address, protocol semantics – are we (a)synchronous? Stateful or stateless? Do we need the connection to remain open? Do these change if you do the extra credit? message format</li>
<li>What kind of data is required in the payload? Some of these are truly binary (images) while some are textual data. How will you know what message has which kind of data (hint: how does HTTP do it?).</li>
<li>You should make sure that you also use large images so that one packet is not enough to sent it to the client.</li>
</ul>
<h1>5 Important</h1>
<ul>
<li>We will NOT debug or try to fix your code.</li>
<li>If we cannot find a certain requirement you will not receive points for it. It is in your best interest to have 80% working correctly rather than having everything implemented but not working at all.</li>
<li>Remember the video where you can show us your functionality!</li>
<li>If your code does not compile/run then you will not receive points for the coding part of the assignment.</li>
<li>If your code does not run through Gradle we will not run it and thus not grade it.</li>
</ul>
<h1>6 Coding</h1>
You are in your junior year so good coding practices and appropriate error handling are expected along with a solution that compiles and runs. If your code is unreadable for us, you can lose up to 10% of the assignment points on top of everything else.

<h1>7 Server on a second system (5 points)</h1>
You should run your server on your second system (e.g. AWS) and connect to that server with your client from your main computer. This setup should be demonstrated in your screencast.

<h1>8 Submission</h1>
On Canvas add the link to your Assignment 3 folder on GitHub, this folder should have the tcp and the udp program in separate directories.

<ul>
<li>tcp</li>
<li>udp</li>
</ul>
ALSO: zip your whole Assignment 3 folder and upload it on Canvas for your assignmnet 3 submission.

Yes, the overall points in this assignment add up to more than 100 points; everything over 100 points will be extra credit.
