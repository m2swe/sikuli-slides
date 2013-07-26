---
layout: default
title: Documentation
---
<style>
div .info {
	height:150px;
}
</style>

## Basic Mouse/Keyboard Actions

<ul class="thumbnails">
		{% assign docid = '1mWe81kAkt7kWe0tBSt_VvRUXPCtdWUFhSF_yq4jH2xE' %}
		{% assign name = 'Click' %}
		{% assign description = 'Execute a mouse left click action on the target marked by the rectangle.' %}		
		{% include actions.html %}


		{% assign docid = '1rCvCfqRe3ke7jv2qDkNxLS2Yi79doG1t08Pzkr1OB3k' %}
		{% assign name = 'Double Click' %}
		{% assign description = 'Execute a mouse double left click action on the target marked by the rectangle.' %}		
		{% include actions.html %}


		{% assign docid = '1WGhC9ycp4Yd61W071YJMjGOoGAq3y5ChP6xn7Z2N8E8' %}
		{% assign name = 'Right Click' %}
		{% assign description = 'Execute a mouse right click action on the target marked by the rectangle.' %}		
		{% include actions.html %}


		{% assign docid = '1OHEfMB8ehcaw4GclYyCHHufcZRV3G4Wz-6MlynkJQvI' %}
		{% assign name = 'Type' %}
		{% assign description = 'Type in the target marked by the rectangle. The content to type is inside the rectangle.' %}
		{% include actions.html %}
		
		{% assign docid = '11F7ldEw8jOUZwDPiAtYxADCHc-WUch_Z-K-iKpv2ywk' %}
		{% assign name = 'Drag and Drop' %}
		{% assign description = 'Drag the target in one rectangle to the area in another rectangle.' %}
		{% include actions.html %}		

</ul>


## Other Actions

<ul class="thumbnails">
		{% assign docid = '1-3SuDlrJB86sVo0lg1QP4R53n0j1qcx-qxikBjVq-YI' %}
		{% assign name = 'Caption' %}
		{% assign description = 'Display caption text on the screen in a rectangle in yellow background.' %}
		{% include actions.html %}
		
		{% assign docid = '10Oa1jp3j8pO016V-bWz6jQ2Ppfn_DRLvx7SvNb2Rc4M' %}
		{% assign name = 'Browser' %}
		{% assign description = 'Open the default web browser and load the URL written inside the cloud symbol.' %}
		{% include actions.html %}
		
		{% assign docid = '1Bfud47ZtFQQCOEvaBNUkaXvHT4G-7V6rNvcQM2EvvwI' %}
		{% assign name = 'Delay' %}
		{% assign description = 'Delay the execution by some amount of time. In this example, the execution of slide 3 is delayed by 10 seconds.' %}
		{% include actions.html %}


		{% assign docid = '18euvQySosDfnS9wO2LLmKWRf_QvvIW248cMvBi5VxaY' %}
		{% assign name = 'Exist' %}
		{% assign description = 'Check if the target marked by the rectangle exists. If not, the execution is aborted.' %}
		{% include actions.html %}
		
</ul>


### Audio

Note: The audio feature is only supported in PowerPoint. Google Presentation does not support adding audio clips.

## Modes

Sikuli Slides can be executed in three modes: automation, tutorial, and help.

<dl>
  <dt>Automation</dt>
  <dd>This is the default execution mode. On each slide, once the target is found, the mouse or keyboard action indicated on the slide is performed. Then the execution moves to the next step. </dd>
  <dt>Tutorial</dt>
  <dd>The purpose of the tutorial mode is to teach a user how to perform a sequence of steps, rather than actually executing those steps. On each slide, once the target is found, it is highlighted by a rectangle to bring the user's attention to the target. A text box appears next to the target and displays the action that should be formed. The user can navigate the tutorial in his/her own pace. The user can decide when to move to the next slide, return to the previous slide, or jump to any slide in the sequence.
  </dd>
  <dt>Help</dt>
  <dd>
	The purpose of the help mode is to assist a user to perform a sequence of steps. It is assumed that the user is somewhat familiar with the sequence, but just needs some extra reminder. Similar to the tutorial mode, the user will be able to see targets highlighted along the sequence and will have to click or type on targets on his/her own. But unlike the tutorial mode, the user does not need to explicitly tell the system to move to the next step. Rather, the system can automatically detect if user has clicked or typed on the right target. If so, it will automatically advance to the next slide. 
  </dd>
</dl>

## Parameters

There are several parameters that can be set at the command line to control the execution behavior of Sikuli Slides.

* **MinScore:** The minimum similar score for a target to be considered a match
* **Delay:** The delay interval between two slides.