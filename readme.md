KISS
======
KISS is a *blazingly* fast launcher for android requiring nearly no memory to run.

Download for free: [Play Store](https://play.google.com/store/apps/details?id=fr.neamar.kiss).
Join the [G+ community](https://plus.google.com/communities/116489528310489783081) to get download instruction for the beta version.

What is it?
------------
KISS is a fast launcher for your Android.

Search through you app, contacts and settings lightning fast.
No more time spent trying to find the app you need to launch : enter a few characters from the name and press enter.
Need to phone someone ? Don't meddle with the call log, just give three letters of his name and push the "phone" button.

KISS becomes smarter and smarter as you uses it, pushing forward results you're more likely to select.

Get ready to be amazed.

Previews
---------------------

![Preview](https://lh3.googleusercontent.com/1B-Vc9Tqh6bfGCVyKXkYSZycwY9Z4g6NxX3ULAKdCPgi9pmGHoyIelC4nsVbQK8d5l0i)
![Preview](https://lh3.googleusercontent.com/ADlhgu6JBVOJRn_XS-BbFbw6HtGopVABpBSdBMfANXpGpicFY3jxVLcuBhnJ9QkSshTp)
![Preview](https://lh3.googleusercontent.com/17JTZKi0wh8ReNTMmhEzoR1Iu_mirK867_H2GbMwDhFf8QwpqhxzccpBLAFo5DbFdg)


How does it work?
-------------------
Different data types can be aggregated via KISS simple interface : apps, contacts, settings...

Each data types uses four classes :

* A *loader*, which retrieve all available items at startup
* A *provider*, which knows all of its items (e.g. all contacts), and responsible for filtering those records according to the query
* A *pojo*, which is a POJO storing simple data for one item (e.g. contact name, display name, phone number, photo)
* A *result*, which ensure the *pojo* is properly displayed in the list

Controlling the workflow is *SummonActivity*, initializing the UI, dispatching the query to the providers and ordering the results according to their relevance and user search history.

### Adding new content sources
This is clearly not as easy as it ought to be.

