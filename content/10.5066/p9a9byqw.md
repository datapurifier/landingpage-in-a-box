---
title: "Tracking Data for Bar-tailed Godwits (Limosa lapponica)"
doi: 10.5066/p9a9byqw
date: 2023-11-18T01:31:12Z
categories: ['Dataset']
tags: ['Animals/Vertebrates', 'Birds', 'Waders/Gulls/Auks and Allies', 'Migratory rates/routes', 'Species life history', 'Telemetry', 'Migratory birds', 'Seasonal distribution', 'Seasonal movement', 'Overwintering', 'Breeding sites', 'Capture-recapture studies', 'Tracking equipment', 'Tagging devices', 'Wildlife', 'Ornithology', 'Migratory species', 'Coastal ecosystems', 'Marine ecosystems', 'Animal tracking', 'Satellite transmitter', 'Platform Transmitter Terminal', 'PTT', 'Argos']
publishers: ['U.S. Geological Survey']
author: ['Lee Tibbitts', 'David C Douglas']
affiliations: ['United States Geological Survey']
funders: []
---

# Abstract
This metadata document describes the data contained in the "rawData" folder of this data package. This data package contains all data collected by the Argos System from 63 satellite transmitters attached to Bar-tailed Godwits on their breeding range in arctic and western Alaska, 2005-2010. Five data files are included in the "rawData" folder of this data package. Two data files (with identical content) contain the raw Argos DIAG (Diagnostic) data, one in the legacy verbose ASCII format and one in a tabular Comma Separate Value (CSV) format. Two other data files (with identical content) contain the raw Argos DS (Dispose) data, one in the legacy verbose ASCII format and one in a tabular CSV format. The fifth file, "deploymentAttributes", contains one record for each transmitter deployment in a CSV formatted table. The deployment attributes file contains information such as when the transmitter was attached to the animal, when tracking of a live animal ended, and a variety of variables describing the animal and transmitter. This table is identical to the "deploymentAttributes" table in the "processedData" folder of this data package. This metadata document describes the data contained in the "processedData" folder of this data package. This data package contains all data collected by the Argos System from 63 satellite transmitters attached to Bar-tailed Godwits on their breeding range in arctic and western Alaska, 2005-2010. The raw data were processed to accomplish two goals: flag implausible location estimates and decode raw sensor data. Three Comma Separate Value (CSV) tables are included in the "processedData" folder of this data package: 1) the "diag_filteredLocations" table contains one record for every Argos location estimate collected, accompanied by a binary flag that denotes an algorithm's plausibility check (based on distance, turning angle, and rate thresholds). Each record also includes a 'Tracking_Status' variable that denotes whether the location was collected from a live animal, a dead animal, or shed transmitter, 2) the "decodedSensor" table contains decoded sensor data such as the transmitter's temperature, battery voltage, and motion (activity), and 3) the "deploymentAttributes" table contains one record for each transmitter deployment in a CSV formatted table. The deployment attributes file contains information such as when the transmitter was attached to the animal, when tracking of a live animal ended, and a variety of variables describing the animal and transmitter. This table is identical to the "deploymentAttributes" table in the "rawData" folder of this data package.

# Access Points
https://www.usgs.gov/centers/alaska-science-center/science/tracking-data-bar-tailed-godwits-limosa-lapponica