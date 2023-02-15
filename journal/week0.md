# Week 0 — Billing and Architecture

<h1>What we watched this week:</h1><br/>
<ul>
  <li>The Saturday Livestream</li>
  <li>Chirag's Spend Consideration Video</li>
  <li>Ashish's Security Video (Loved it so much! Connected and messaged him on LinkedIn. Also, his repo is 🔥https://github.com/hashishrajan)</li>
  <li>The after stream video where Andrew explains A LOT in detail!</li>
</ul>

<h2>What I took notes on this week </h2>
<ul>
  <li>The user needs for the Cruddur app, and an overview of the services we will use. Margaret did an awesome job with the technical roleplay!</li>
  <li>What "dumb questions" to ask from Chris - "Why am I here?" "What goals can I help you reach?"</li>
  <li>The C4 Model-Never heard of it! That link is now bookmarked for future use. </li>
  <li>The importance of a napkin architectural diagram and the fact that we can refine and improve it. We don't have to start with a perfect one.</li>
  <li>The iron triangle that consists of scope (features, functionality), time (the schedule), and the cost (budget resources). And the saying that "good work isn't cheap, cheap work isn't good."</li>
  <li>Added the auto prompt to my AWS CLI, used the command aws sts get-caller-identity to access my AWS info as a settings check. Also, we can look at lists of the shortcuts to learn to use them better.</li>
  <li>If stuck in VIM in the CLI, q to quit!</li>
  <li>Make sure SVG's have an XML tag</li>
  <li>The Well Architected Tool helps us walk through the solutions we have created to make sure that they fit with AWS standards and best practices. https://docs.aws.amazon.com/wellarchitected/latest/userguide/intro.html</li>
</ul>

<h2>What I learned</h2>
<ul>
  <li>Linux commands! Once we began using Gitpod, we got into exploring various Linux commands. Also, echo $path was very informative to see </li>
  <li>Top 5 Security Best Practices from Asish</li>
  <li>grep helps you search for things in Gitpod</li>
  <li>Our env datas persist in Gitpod.io/user/variables , check there for info after you have run gp env AWS_ACCESS_KEY_ID="" in the terminal</li>
  <li>How to get the account id: aws sts get-caller-identity --query Account </li>
</ul><br/>
<p>Also, I'm sure the below lines of code will be useful!</p><br/>
<p>gitpod /workspace $ export AWS_ACCESS_KEY_ID=""<br/>
gitpod /workspace $ export AWS_SECRET_ACCESS_KEY=""<br/>
gitpod /workspace $ export AWS_DEFAULT_REGION=""<br/>
  The below line checks to see if the above lines were successful! <br/>
gitpod /workspace $ env | grep AWS_<br/>
AWS_DEFAULT_REGION=<br/>
AWS_SECRET_ACCESS_KEY=<br/>
AWS_ACCESS_KEY_ID=<br/>
  </p>


<h2>My Cruddur first draft architecture. Make with a combo of Lucid and my "napkin" art with a stylus.</h2>
<img width="625" alt="cruddur" src="https://user-images.githubusercontent.com/98853049/218921009-ec082388-0b0e-43de-889d-25f328dc0ee6.png">
<h2>And here is my "napkin" diagram that I made while in the yard on this beautiful February day! </h2>
<img width="625" src='https://user-images.githubusercontent.com/98853049/219192172-fe0cd055-036d-419c-8d7e-9adcf4ac780c.jpg'
 >
<h3>Thanks so much Cloud Camp for a great Week 0! I am going to go check off my to do list in the student portal and see if I can help anyone on Discord. Others, Andrew Brown included, helped me this week on Discord. It's a fabulous group of people!</h3>
