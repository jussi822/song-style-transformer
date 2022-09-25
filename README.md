# Song style transformer

Project to experiment with editing songs towards a selected style, e.g. more Mozart-like

## Summary

Take any piece of music and apply a selected filter to edit it. 
Filters can be built by user by feeding any set of songs they like
Building AI course project

## Background

I don't know whether something similar has been built before.

Someone might find it fun to be able to convert pieces of music (or speech or their mom's yelling or whatever) to be more like a well-known style.

## How is it used?

Mobile device or computer needed to use the app: User picks a piece of music, then selects a filter they want to apply and uses a slider to  

Ideally there would be an UI that enables to pick any file or source containing voice: e.g. song file on the device memory, Spotify song, Youtube video, recording through the device microphone.



<!-- Describe the process of using the solution. In what kind situations is the solution needed (environment, time, etc.)? Who are the users, what kinds of needs should be taken into account?

Images will make your README look nice!
Once you upload an image to your repository, you can link link to it like this (replace the URL with file path, if you've uploaded an image to Github.)
![Cat](https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg)

If you need to resize images, you have to use an HTML tag, like this:
<img src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Sleeping_cat_on_her_back.jpg" width="300">

This is how you create code examples:
```
def main():
   countries = ['Denmark', 'Finland', 'Iceland', 'Norway', 'Sweden']
   pop = [5615000, 5439000, 324000, 5080000, 9609000]   # not actually needed in this exercise...
   fishers = [1891, 2652, 3800, 11611, 1757]

   totPop = sum(pop)
   totFish = sum(fishers)

   # write your solution here

   for i in range(len(countries)):
      print("%s %.2f%%" % (countries[i], 100.0))    # current just prints 100%

main()
```
-->


## Data sources and AI methods



Filters could be built as ML algorithms taught by using a set of songs, e.g. library of violin solos for violin filter, all Mozart's songs for Mozart filter, library of birds singing for bird filter, etc.

Open questions around approach:
1. Where to get sufficiently large library of songs to train the filter?
2. How to input the audio to the ML algorithm? What is the best way to reduce dimensionality of the training songs, if/when necessary, but still make it produce high-quality audio?
3. What ML methods to use as filter?


For 3., potentially could learn a neural network to classify music as Mozart or non-Mozart (requires also other types of music, because otherwise it will classify everything as Mozart...). Then we could use the partial derivatives of the input song data elements vs. the output of the model to adjust the input song by small steps towards more Mozart.



<!-- Where does your data come from? Do you collect it yourself or do you use data collected by someone else?
If you need to use links, here's an example:
[Twitter API](https://developer.twitter.com/en/docs)

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
-->

## Challenges

Need to understand what copyright issues might be relevant. 

## What next?

Examples of possible improvements:
* Add more filters
* Enable to mix several filters
* Enable on-the-fly voice transformation, e.g. during a phone call
* Integrate to existing solutions, e.g. enable WhatsApp user to transform their speech messages before sending
* Build an AI composer that creates e.g. Mozart-like music from scratch
* Score all Mozart's songs in terms of how Mozart-like they are

## Acknowledgments

<!-- 
* list here the sources of inspiration 
* do not use code, images, data etc. from others without permission
* when you have permission to use other people's materials, always mention the original creator and the open source / Creative Commons licence they've used
  <br>For example: [Sleeping Cat on Her Back by Umberto Salvagnin](https://commons.wikimedia.org/wiki/File:Sleeping_cat_on_her_back.jpg#filelinks) / [CC BY 2.0](https://creativecommons.org/licenses/by/2.0)
* etc  -->
