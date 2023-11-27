---
title: "ShakeMap Atlas V4 and AtlasCat"
doi: 10.5066/p98atogz
date: 2023-11-16T20:29:48Z
categories: ['Dataset']
tags: ['Geophysics', 'Seismology']
publishers: ['U.S. Geological Survey']
author: ['Kristin Marano', 'Michael Hearne', 'Kishor Jaiswal', 'Eric Thompson', 'Bruce Worden', 'David J Wald']
affiliations: ['United States Geological Survey']
funders: []
---

# Abstract
The Atlas of ShakeMaps (~14,100 earthquakes, 1900-2020) provides a consistent and quantitative description of the distribution of shaking intensity for calibrating earthquake loss estimation methodologies, like those used in the USGS Prompt Assessment of Global Earthquakes for Response (PAGER)�system. Version 4 of the Atlas includes a vastly expanded compilation of ShakeMaps for consequential and widely felt earthquakes using updated ShakeMap (Version 4)�software. For each event, we have attempted to gather available macroseismic, recorded ground motions and finite fault inputs. AtlasCat�is the companion catalog to Atlas V4. For each event in the Atlas, AtlasCat contains population exposure to each intensity level, loss information, and summary data regarding the number of ground motion recordings, intensity observations, and availability of a finite fault. Please let us know if you know of additional datasets that could be added to specific events or sets of events. � Accessing the ShakeMap Atlas Select events or collections of events ShakeMap Atlas can be accessed via the USGS Earthquake Catalog Search�or with queries from the search tools we provide described below. � 1. Using the USGS Earthquake map interface The full ShakeMap Atlas is contains too many earthquakes to load in its entirety via the USGS Earthquake map interface. To access the Atlas using the catalog search tool, it is necessary to search for a smaller subset of events as search results displayed via the map interface is limited to 2,000 events. A sample search of Atlas ShakeMaps from 2000-2005 can be accessed here. To download a comma-separated value (csv) file of all or a subset of Atlas events using the same catalog search tool, go to the linked sample Atlas search page, click on the "gear" icon in the upper right banner and then click on the "Search Earthquake Catalog" button. Simply modify the query as needed, then change the "Output Options? -&gt; ?Format? -&gt; ?CSV?. � 2. Libcomcat and Getproducts Libcomcat is a Python library that allows command line tools easily access the ShakeMap Atlas, or specified subsets, and to then download any of the associated ShakeMap products and files for each event. One of the standard tools with libcomcat is getproducts, which greatly facilitates the retrieval of select earthquakes and associated products. Even more complex queries can be facilitated with other libcomcat tools. For example, view a sample ComCat search using an iPython Notebook.

# Access Points
https://www.sciencebase.gov/catalog/item/5e3b319ee4b0edb47bddae34