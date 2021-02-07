js-vido — JavaScript Video Download Optimizer
=============================================

A JavaScript library for optimizing html pages with video content that prevents videos from loading on mobile devices.

What it does
------------

Prevents videos with the "optimize-video" class from being downloaded to mobile devices by displaying the poster image instead. This is done by creating the source element of the video node through the data-src attribute only in case the device used is a laptop or desktop computer.

One of the cases where this functionality can be useful is verified with auto-play videos used in web page backgrounds, because auto-play does not work on mobile devices, the video would be downloaded unnecessarily, slowing down the loading of the page and consuming mobile data.
