# AutoTrack

### RFID-Based Manufacturing Asset Tracking

AutoTrack is a manufacturing asset tracking system developed during my summer internship at **Limitless Hunch Pvt. Ltd.** between **June–August 2025**.

The project connected RFID-based asset identification with an automated data workflow and a web-based dashboard for monitoring machine and asset status, location, operator information, and activity.

The original system was developed and tested in a manufacturing environment. The current public deployment is retained as a demonstration of the application and workflow; it is no longer connected to the original factory RFID installation or its live data source.

---

## What I Built

The project was designed to reduce repetitive manual tracking and data-entry work in a manufacturing environment.

The workflow combined:

* RFID-based asset identification
* Excel-based production/tracking data
* UiPath browser automation
* AutoTrack web interface
* Inventory and activity monitoring

The overall workflow was:

```text
RFID-Tagged Machine / Asset
            ↓
       RFID Reader
            ↓
       Tracking Data
            ↓
          Excel
            ↓
       UiPath Bot
            ↓
     AutoTrack Web UI
            ↓
 Inventory + Status + Activity
```

During the internship, RFID-tagged machines and material stations were used to identify assets and capture information such as RFID ID, machine name, operational status, location, and timestamp.

---

## Key Features

### Asset Tracking

* RFID-based asset identification
* Asset status tracking
* Check-in / check-out workflow
* Operator assignment
* Location tracking
* Last-update information

### Dashboard

* Manufacturing asset inventory
* Total asset statistics
* Available and checked-out assets
* Activity history
* Recent activity feed
* Activity visualization

### Automation

* Excel data processing
* Automated browser interaction using UiPath
* Automatic form submission
* UI element validation
* Error handling and logging
* Reusable automation sequences

---

## RFID Integration

RFID was part of the original physical setup used during the internship.

RFID readers and tags were used to identify selected machines and material stations. The collected information was then processed through the automation workflow and reflected in the AutoTrack interface.

The original hardware setup included **125 kHz RFID readers and tags**, a PC for RPA execution, and Wi-Fi connectivity for communication with the web interface.

### Original data flow

```text
Physical Asset
      ↓
RFID Tag
      ↓
RFID Reader
      ↓
RFID / Tracking Record
      ↓
Excel
      ↓
UiPath
      ↓
AutoTrack
```

---

## AutoTrack Dashboard

The web interface was developed to provide a central view of tracked manufacturing assets.

The dashboard displays information including:

| Information     | Purpose                          |
| --------------- | -------------------------------- |
| RFID ID         | Asset identification             |
| Asset / Machine | Identifies the tracked unit      |
| Status          | Availability / operational state |
| Location        | Current or recorded location     |
| Operator        | Associated operator              |
| Timestamp       | Last recorded update             |
| Activity        | Recent tracking events           |

The interface also provides activity statistics and a manufacturing asset inventory view.

---

## RPA Workflow

UiPath was used to automate the transfer of tracking records into the AutoTrack interface.

The workflow followed this general sequence:

```text
Start
  ↓
Read Excel Data
  ↓
Open AutoTrack
  ↓
Process Each Record
  ↓
Enter Asset Information
  ↓
Submit Record
  ↓
Verify Result
  ↓
Log Status
  ↓
Next Record
  ↓
Finish
```

The automation was optimized using element-based synchronization, conditional checks, error handling, and logging rather than relying entirely on fixed delays.

---

## Results During Internship

The system was tested as part of the internship workflow.

The documented tests reported:

* Average automated data transfer time of approximately **2.3 seconds per record**
* Ten entries processed in **under 20 seconds**
* Consistent synchronization between the Excel records and AutoTrack interface during the recorded test runs
  These results refer to the internship deployment and test environment, not the current public deployment.

---

## Technology Stack

**Automation**

* UiPath Studio

**Data**

* Microsoft Excel

**Web Application**

* HTML5
* CSS3
* JavaScript
* Chart.js
* Font Awesome

**Hardware**

* RFID readers
* RFID tags
* PC/Laptop
* Wi-Fi connectivity

**Deployment**

* Netlify

---

## Current Public Version

The original project was developed and tested with the RFID hardware available at the internship site.

The physical installation is no longer connected to this public deployment, so the current website should be considered a **project demonstration rather than a live factory monitoring system**.

The repository preserves the web interface and software-side implementation from the project.

---

## Project Context

**Organization:** Limitless Hunch Pvt. Ltd.
**Project:** Automation Workflow for Factory Process Monitoring
**Duration:** June–August 2025
**Focus:** Manufacturing automation, RFID-based tracking, RPA and web-based monitoring

The internship provided hands-on exposure to automation workflow design, data handling, browser automation, debugging, and integration of digital tools within a manufacturing environment.

---

## Future Improvements

Potential extensions to the system include:

* Persistent backend database
* Direct RFID-to-application communication
* Real-time event streaming
* Multiple RFID reader locations
* Asset movement history
* User authentication
* Alerts for missing or misplaced assets
* Integration with other manufacturing systems
* IoT-based machine monitoring

---

## Project Status

**Completed internship project / public demonstration**

The original RFID-enabled workflow was developed and tested during the internship. The current public version is maintained as a demonstration of the application and project architecture rather than a live connection to the original factory environment.
