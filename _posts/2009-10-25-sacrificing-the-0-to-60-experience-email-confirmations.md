---
layout: post
title: "Sacrificing the 0 to 60 experience"
subtitle: "How email confirmations ruin the initial user experience"
category: 
tags: []
---
{% include JB/setup %}

<section class="row">
	<p class="span12">The 0 to 60 experience refers to the time from a user deciding to register, buy, or otherwise begin using your product to when they have successfully begun to use it.  Making the right impression during this window of time is imperative.</p>

	<blockquote class="span12">"...negative first impressions, once formed, take more work to change than impressions that start off as positive or even neutral."  <small>Dr. Gitte Lindgaard, NSERC/Cognos Industrial Research Chair in User-Centred Design</small></blockquote>

	<p class="span12">There are many things that can damage your initial impression, some easy to fix, some more involved.  In this post, I am going to focus on one practice, which, while sound from a technical perspective, involves making a significant trade-off in your 0 to 60: Email Confirmations. You know the one I mean: Click this link to activate your account. These, or similar, words are uttered by the ubiquitous confirmation email. You visit a site that promises some interesting function, sign up and all of a sudden your experience is interrupted while you are asked to wait for an email to arrive for you to confirm that you are, in fact, you. While validating the user did not mis-type and is using an active email address which they have access to are important, there is no denying the negative effect this process has on a users initial experience with your application.  At the time which you should be attempting to hook a new user, you force them to wait for an email, click a link, and complete the 'activation' process. By no means am I suggesting that all applications could, or should, eliminate email verification.  I am proposing that it a decision that should be made on an application by application basis.  Further, if you do have need, there are some other approaches that are less intrusive that you can employ:</p>
	<h4 class="span12">Verification within a period of time</h4>
	<p class="span12">This approach allows the user to create an account and use your application for a period of time without verifying their email address.  This is an approach that is frequently employed by trial software, but it works really well for email verification, as well.  A week is often a good length of time, but be sure to make the user aware of the need to verify their address as the deadline approaches.</p>
	<h4 class="span12">Automatic-login, with password emailed</h4>
	<p class="span12">This approach relies on the ability to automatically log the user in after signing up for an account.  The user creates an account without setting a password.  Upon account creation, the user is automatically logged in to the application for their first visit.  In order to access the site again, they must retrieve their password from an email which is sent to them (changing account information should also require this password, even on the initial visit).  The downside to this approach is that the user use a fairly unfriendly password from their email in order to log in and change their password to something more comfortable to them.</p>
	<h4 class="span12">Optimistic email verification (revoke link instead of confirm)</h4>
	<p class="span12">This approach is an optimistic email verification.  In other words, we assume that most people are correctly entering an email address that they own.  Instead of sending an email which the user must act on to verify their signup, we send a Welcome email which offers an easy mechanism to cancel the account if they did not sign up for it.  This emails serves two purposes:  In our nominal case, this email simply provides the user with confirmation that we have their email address and is a good place to provide tips to using the application, etc.  In the case of a user signing up for an account with a false email address, it provides the real owner of that email address an easy way to disable access.</p>
	<h4 class="span12">Summary</h4>
	<p class="span12">I hope this post gets you to rethink how you handle email verification and to always keep in mind your users first experience with your application.</p>
</section>