# Braintree Production Keys: The Undocumented Maze

## Project Description
This repository documents my experience attempting to obtain **Braintree production (live) API keys**.  
Despite a smooth sandbox integration, the process of going live was unexpectedly difficult.  
Based on the behavior I encountered, it appears that **new merchants may no longer be a priority in Braintree’s onboarding pipeline**.

## Motivation
I planned to use Braintree to implement payment processing for **Post2Video**, my SaaS product.

## My Experience
- Spent several weeks learning the Braintree SDK and reading official documentation  
- Successfully integrated Braintree into Post2Video  
- Built a fully working sandbox POC (`paypal-poc`)  
- Reached the final step: obtaining production keys  
- Submitted the “Contact Sales” form:
  - **10 Nov 2025** — submission ended with a page error  
  - **13 Nov 2025** — submission succeeded  
- As of **3 Dec 2025**, I have received **no reply at all**  
- Ultimately, I had to remove all Braintree-related code and switch to a manual PayPal integration  
- Result: several weeks of development time lost

## Key Takeaways
- Getting sandbox keys and a sandbox merchant ID is easy  
- Getting *production* access is **unclear, slow, and appears unsupported**  
- For new projects, I cannot recommend starting with Braintree unless you already have a direct sales contact

## Community Sentiment (External Research)
To confirm my experience was not isolated, I searched for recent user feedback on **3 Dec 2025**.  
Using Perplexity AI, I collected summaries of recent discussions and reviews.

The findings match my experience:

### Main Complaints
- Support described as “practically nonexistent” or extremely slow  
- No reliable way to reach a human—phone lines reportedly non-functional or looping  
- Long delays on urgent issues (fraud, 3DS, chargebacks, access problems)  
- Merchants expressing frustration that communication happens only via slow email tickets

### Overall Sentiment
- Review platforms in **2024–2025** show very low ratings (≈ 1–1.5 / 5), mostly due to support  
- Many merchants publicly state they are migrating to alternatives such as Stripe

Here is the screenshot of the Perplexity AI summary that supports these findings:

<img src="./figs/perplexity-3-dec-2025.png" alt="Screenshot of Perplexity AI summary showing negative Braintree support sentiment" />

---

## Installation / Attempt to Go Live

### 1. Go Live / Get Production Account
Here is the “Get Production Account” section as shown on the Braintree site:

<img src="./figs/get-production-account.png" alt="Screenshot of the Braintree 'Get Production Account' page" />

### 2. Contacting Sales Through PayPal
You are directed to this contact form:
https://www.paypal.com/us/business/contact-sales?utm_campaign=Braintree_Migration&utm_medium=Website&utm_source=Braintree

Here is what the form looks like:

<img src="./figs/get-in-touch.png" alt="Screenshot of PayPal sales contact form" />

On **10 Nov 2025**, the form ended with an error.  
On **13 Nov 2025**, the form submitted successfully.  
Here is the confirmation message from the successful submission:

<img src="./figs/success-contact-sails.png" alt="Screenshot confirming successful submission of the PayPal sales contact form" />

### 3. Attempting the Sandbox → Production Path
Here is the sandbox page where developers expect to find a path to production:

<img src="./figs/go-live.png" alt="Screenshot showing the Go Live button on the Braintree sandbox page" />

When clicking **Go Live**, instead of Braintree onboarding, you are redirected to a generic PayPal page:

<img src="./figs/go-live-clicked.png" alt="Screenshot showing the PayPal page displayed after clicking Go Live" />

### 4. Sandbox vs Production Link Path
Here is the “Sandbox vs Production” documentation page that appears below the earlier section:

<img src="./figs/switch-from-sandbox-to-production.png" alt="Screenshot of Braintree documentation describing how to switch from sandbox to production" />

It directs you to a “Begin Your Production Integration” page, but provides **no path to actually request or obtain production credentials**.

---

## References
- https://developer.paypal.com/braintree/articles/  
- **My POC walkthrough video:** https://youtu.be/6u0aroHdIpM



<!-- # Braintree Production Keys: The Undocumented Maze

## Project Description
This repository documents my experience attempting to obtain **Braintree production (live) API keys**.  
Despite a smooth sandbox integration, the process of going live was unexpectedly difficult.  
Based on the behavior I encountered, it appears that **new merchants may no longer be a priority in Braintree’s onboarding pipeline**.

## Motivation
I planned to use Braintree to implement payment processing for **Post2Video**, my SaaS product.

## My Experience
- Spent several weeks learning the Braintree SDK and reading official documentation  
- Successfully integrated Braintree into Post2Video  
- Built a fully working sandbox POC (`paypal-poc`)  
- Reached the final step: obtaining production keys  
- Submitted the “Contact Sales” form:
  - **10 Nov 2025** — submission ended with a page error  
  - **13 Nov 2025** — submission succeeded  
- As of **3 Dec 2025**, I have received **no reply at all**  
- Ultimately, I had to remove all Braintree-related code and switch to a manual PayPal integration  
- Result: several weeks of development time lost

## Key Takeaways
- Getting sandbox keys and a sandbox merchant ID is easy  
- Getting *production* access is **unclear, slow, and appears unsupported**  
- For new projects, I cannot recommend starting with Braintree unless you already have a direct sales contact

## Community Sentiment (External Research)
To confirm my experience was not isolated, I searched for recent user feedback on **3 Dec 2025**.  
Using Perplexity AI, I collected summaries of recent discussions and reviews.

The findings match my experience:

### Main Complaints
- Support described as “practically nonexistent” or extremely slow  
- No reliable way to reach a human—phone lines reportedly non-functional or looping  
- Long delays on urgent issues (fraud, 3DS, chargebacks, access problems)  
- Merchants expressing frustration that communication happens only via slow email tickets

### Overall Sentiment
- Review platforms in **2024–2025** show very low ratings (≈ 1–1.5 / 5), mostly due to support  
- Many merchants publicly state they are migrating to alternatives such as Stripe

### Screenshot of Perplexity Results
<img src="./figs/perplexity-3-dec-2025.png" alt="Perplexity AI summary screenshot showing negative Braintree support sentiment" />

## Installation / Attempt to Go Live

### 1. Go Live / Get Production Account
<img src="./figs/get-production-account.png" alt="Screenshot of the Braintree 'Get Production Account' page" />

### 2. Contact Sales
Click **Get in Touch With Our Sales Team**:  
https://www.paypal.com/us/business/contact-sales?utm_campaign=Braintree_Migration&utm_medium=Website&utm_source=Braintree

<img src="./figs/get-in-touch.png" alt="PayPal sales contact form screenshot" />

- **10 Nov 2025:** form submission resulted in an error  
- **13 Nov 2025:** form submission succeeded  
- **No response** as of 3 Dec 2025

<img src="./figs/success-contact-sails.png" alt="Successful 'Contact Sales' form submission confirmation message" />

### 3. Using the Sandbox Page as an Alternative Path
Navigate to:  
https://apply.braintreegateway.com/signup/sandbox?utm_campaign=Braintree_Migration&utm_medium=Website&utm_source=Braintree

Scroll down and click **Go Live**.

Expected: Braintree onboarding  
Actual: Redirected to a generic PayPal page

<img src="./figs/go-live.png" alt="Go Live button on Braintree sandbox page" />  
<img src="./figs/go-live-clicked.png" alt="Redirect result showing PayPal page instead of Braintree" />

### 4. Sandbox vs Production Page
Below the earlier page is a link to **Sandbox vs Production**, which leads here:

<img src="./figs/switch-from-sandbox-to-production.png" alt="Braintree documentation page showing how to switch from sandbox to production" />

Clicking **Begin Your Production Integration**:  
https://developer.paypal.com/braintree/docs/start/go-live/ruby/

Still does not provide a path to request or obtain production credentials.

## References
- https://developer.paypal.com/braintree/articles/  
- **My POC walkthrough video:** https://youtu.be/6u0aroHdIpM



<!-- <h1>Braintree Production Keys: The Undocumented Maze</h1>

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
</ul> --> -->
