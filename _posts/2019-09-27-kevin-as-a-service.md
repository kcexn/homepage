---
layout: post
title: Kevin As A Service
categories: [Angular, Firebase]
date: 2019-09-27 12:47
lead: "Firebase functions, Angular SPA, and 
Google's oAuth2 playground."
---

# Email Notifications

A couple of conversations in the office after misaligned schedules and missed communications 
led to a few missed lunch break catchups led to me cracking the joke that obviously the 
solution to all of our communications problems was if I present a public API that others can 
interface with. 

In hindsight the joke is not very funny (the joke wasn't funny not in hindsight either). It did 
lead me to think about how I would build such an application. Obviously there would need to be 
some kind of front end user interface that my ~~co-workers~~ users can interact with. There needs 
to be an email notifications system so that I can receive what my users send me.

In the end I decided I would build a little application with an Angular front end, and Firebase 
in the backend using Google's email API to pass notifications back to me. Go take a look 
[here](https://sendgridmail-228a0.web.app).

<img src="{{ site.baseurl }}/assets/posts/2019-09-27-kevin-as-a-service/FlowDiagram.png" class="img-fluid d-block mx-auto">

# Angular App

The Angular front end is pretty simple, using Bootstrap as styling I put an image, caption, and 
an angular form into a carousel to produce a **very** simple view. I chose to use angular forms 
so that potentially, if I ever come back to this project I can create a more dynamic form than 
the incrediby boring form that I have right now.

<img src="{{ site.baseurl }}/assets/posts/2019-09-27-kevin-as-a-service/Splash.png" class="img-fluid d-block mx-auto">

<img src="{{ site.baseurl }}/assets/posts/2019-09-27-kevin-as-a-service/BoringForm.png" class="img-fluid d-block mx-auto">

Maybe if I have some time and interest I'll revisit this project in the future and make these views a 
bit prettier, and also add extra dynamic features to the web form so it feels much more like the 
JSON schema that started the idea for this project to begin with.

# Firebase and Google oAuth2

I decided to use Firebase as the hosting and back end solution, since it has a generous hobbyist 
allowance, and free and easy integration with google's APIs. Following some Medium tutorials like 
[this](https://medium.com/@edigleyssonsilva/cloud-functions-for-firebase-sending-e-mail-1f2631d1022e) one, and playing with the google oAuth2 playground [here](https://developers.google.com/oauthplayground), following this guide provided [over here](https://android.jlelse.eu/firebase-functions-send-email-using-google-oauth2-20c552da6b3e).

I'm reasonably happy with the final result, especially given the amount of time I've had recently 
outside of work hours to pursue projects of interest has not been as much as I'd like.

<br/>