## Click Jacking

There's a popular website xyz.com

Hacker builds a website abc.com and embeds xyz.com using iframe, embed etc., to attract users to his website. But he addes a anchor link on top of the whole website using z-index.
So When user clicks he will be redirected to the page of his choice. This is known as clickjacking.

# How to prevent?

Set a header on the app-server called x-frame-options. It can have only 2 values, i)DENY ii)SAMEORIGIN
Deny means don't allow embed of the website even on our website. SAMEORIGIN means allow embedding of website only on our site.
