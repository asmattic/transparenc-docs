Function Reference
==================

.. Variables
.. include:: vars.rst

General function specifications for |AppName|_.

Campaigns
---------

Currently implemented to handle just adwords campaign data. To see future features, `check the project on Basecamp <https://basecamp.com/2947829/projects/12128091>`_ .

Campaigns
~~~~~~~~~

``addCampaigns``

* Appends all campaigns to the menu and sets up their id based on the name of the campaign by replacing spaces with a dash and converting any capitol letters to lower case using ``toLower``

``getCampaignMeta``

* Returns all campaign metadata ...

``getCurrentCampaign``

``getGoalIds``

``getCampaignTypes``

``accountForMargin``

* gets the client specific margin and incoorporates that and cost values

``prepareCampaigns``

* Format and filter out unnessescary data

``renderGraph``

* Grabs the query and prints to the graph the data returned

``renderCampaignGraphs``

* Gets all of the campaign types including a list of already pre-conficured campaign types like then ``rendersGraph

Views
~~~~~

Info about the unserscore templates used

Page Setup
~~~~~~~~~~~

``setupPage``

* Grabs goad ids of specific capampaign page
* Prints the graph templates using ``getGraph`` 
* Updates all of the graphs are updated with ``updateAllEmbedGraphs``

