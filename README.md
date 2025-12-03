<h1>Braintree Production Keys: The Undocumented Maze</h1>

<h2>Project Description</h2>
My bad experience getting live braintree api keys. Evidence suggests PayPal is quietly        
  sunsetting Braintree for new merchants

<h2>Motivation</h2>
  Implement payment processing for Post2Video (my SaaS) using Braintree.

<h2>My Experience</h2>
  <ul>
      <li>Spent weeks learning Braintree SDK and documentation</li>
      <li>Integrated Braintree into Post2Video (my SaaS)</li>
      <li>Built working POC in sandbox environment (see reference: paypal-poc)</li>
      <li>Ready to go live - tried to get production keys</li>
      <li>Submitted contact form Nov 10, 2025 (form error) and Nov 13, 2025 (success)</li>
      <li>Waited weeks - no response from Braintree sales team</li>
      <li>Had to throw away all Braintree integration code</li>
      <li>Implemented manual PayPal process instead</li>
      <li>Result: Weeks of development time lost</li>
  </ul>

<h2>Key Takeaways</h2>
<ul>
    <li>getting braintree sandbox keys and merchant id is easy , but getting them for live (production) is nightmare</li>
   <li>don't use braintree as newcomer</li>
</ul>

<h2>What Others Are Saying About Braintree Support</h2>
  
 <p>To verify my experience wasn't isolated, I researched community sentiment on December 3, 2025 using Perplexity AI. The findings confirm     
  a widespread pattern of support issues with Braintree:</p>

  <p>Recent comments from users in the last months are mostly negative about Braintree support, especially around response speed, phone
  access, and handling of problems.</p>

  <h3>Main Complaints</h3>
  <ul>
      <li>Many reviewers say support is "practically nonexistent," with no easy way to reach a human and heavy reliance on slow contact forms    
   or email tickets</li>
      <li>Merchants report long waits or no replies on urgent issues like fraud attacks, chargebacks, login problems, or 3DS changes</li>        
      <li>Several reviews mention there is no working incoming phone support anymore, or that only sales numbers exist and calls either loop     
  in menus or get cut off</li>
  </ul>

  <h3>Overall Sentiment</h3>
  <ul>
      <li>Ratings on major review platforms in 2024–2025 are very low (around 1–1.5 out of 5), driven mainly by frustration with slow or
  unreachable customer service</li>
      <li>In e-commerce communities, multiple merchants say they are considering or already switching to alternatives such as Stripe because     
  of poor recent support experiences</li>
  </ul>

This is the image of the reply i got from perplexity
  <img src='./figs/perplexity-3-dec-2025.png'/>

<h2>Installation</h2>
go live \ get production account

<img src='./figs/get-production-account.png'/>

click <a href='https://www.paypal.com/us/business/contact-sales?utm_campaign=Braintree_Migration&utm_medium=Website&utm_source=Braintree'>get in touch with our sales team</a> and you will need to fill the form <img src='./figs/get-in-touch.png'/> and submit which i did 10-nov-25 at about 10AM and i wait for answer =>did not get any and page had error

try again in 13-11-25 , filled the contact form and now it was success but still got no answer as of today 3-dec-25

<img src='./figs/success-contact-sails.png'/>

<h2>Usage</h2>
navigate to the page of <a href='https://apply.braintreegateway.com/signup/sandbox?utm_campaign=Braintree_Migration&utm_medium=Website&utm_source=Braintree'>Create a Braintree Sandbox Account</a> scroll down and click on Go Live <img src='./figs/go-live.png'/>

Click on it i am navigatedwhy to pure paypal page - nothing about braintree here !

<img src='./figs/go-live-clicked.png'/>

but there are some links below in the first image

click on 'sandbox vs production' and you will be navigated to <img src='./figs/switch-from-sandbox-to-production.png'/> here click on <a href='https://developer.paypal.com/braintree/docs/start/go-live/ruby/'> begin your production integration</a>



<h2>References</h2>
<ul>
    <li><a href='https://developer.paypal.com/braintree/articles/'>https://developer.paypal.com/braintree/articles/</a></li>
    <li><a href='https://youtu.be/6u0aroHdIpM'>One-Click Payment Guide with PayPal and Braintree</a> - this is my own experience</li>
</ul>
