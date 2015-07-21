# Introduction #

Development documentation of the Mondrian App (or PlugIn) for Cytoscape 3. It is a Google summer of code project in 2012.

# Source #
Source code is hosted on:
http://code.google.com/p/cbio-cancer-genomics-portal/source/browse?repo=mondrian

There are two modules in the maven project:
  * cbioportal-client: This is a Java API for the cBio portal web services
  * mondrian-cy3-app: This is the Mondian app, which is dependent on cbioportal-client

# Getting Started #
After Cytoscape 3 starts and Mondrian is installed, use menu App -> Mondrian to start Mondrian.

Once Mondrian is started, you will see the following screen:

![http://wiki.cbio-cancer-genomics-portal.googlecode.com/hg/images/mondrian-1.png](http://wiki.cbio-cancer-genomics-portal.googlecode.com/hg/images/mondrian-1.png)

Clicking on the "Load" button in the small Mondrian panel on the right side of the Cytoscape window will pop up the CBio Data Import Dialog.

![http://wiki.cbio-cancer-genomics-portal.googlecode.com/hg/images/mondrian-2.png](http://wiki.cbio-cancer-genomics-portal.googlecode.com/hg/images/mondrian-2.png)

You can select a cancer study, choose one or more genetic profiles, and select a pateint/case set to import. At the bottom of the dialog, you have to choose the node attribute in your network that is annotated with gene symbols.

After clicking on OK, data will be imported from the cBio databases via the cBio web API. Now in Cytoscape, click on the Mondrian Control Panel, you will see heatmap table. Clicking on a cell in the table will update the color of the nodes in the network with values in the column of the selected cell. Above the heatmap table, you can use the drop down boxes to choose a different data type, or different tables accordingly.

![http://wiki.cbio-cancer-genomics-portal.googlecode.com/hg/images/mondrian-3.png](http://wiki.cbio-cancer-genomics-portal.googlecode.com/hg/images/mondrian-3.png)