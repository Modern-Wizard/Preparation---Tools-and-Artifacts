# Preparation---Tools-and-Artifacts

In this task, we will prepare the artefacts and introduce the tools needed for the investigation.

## Compare by hash
Before conducting the investigation, one of the most important steps is to compare the artefacts by their hashes. It is a common practice to verify if the artefacts are expected as it is.

You can get the hashes of each artefact by running Powershell from the taskbar and executing the following commands:

<div>
<img src="https://github.com/Modern-Wizard/Tempest/blob/main/ss1.png" />
</div>

## Toolset
The toolset needed for this task is focused on analysing Sysmon Logs, Windows Event Logs, and Packet Capture.

## Endpoint Logs
To analyse Windows artefacts such as Windows Event Logs and Sysmon logs, we will use the following tools:

    EvtxEcmd
    Timeline Explorer
    SysmonView
    Event Viewer

## Network Logs
To analyse the provided packet capture, we will use the following tools:

    Wireshark
    Brim

## EvtxEcmd & Timeline Explorer
Eric Zimmerman has created a set of forensic tools used to analyse Windows artefacts called EZTools (Eric Zimmerman's Tools). For this task, we will focus on EvtxEcmd and Timeline Explorer, as these tools are mainly used for parsing and analysing Evtx logs.

﻿EvtxEcmd is a command-line tool which parses Windows Event Logs into different formats such as CSV, JSON, XML, etc. You may use this tool in conjunction with Timeline Explorer, created by the same author. Timeline Explorer is a GUI-based tool that functions as a data filtering and navigating application to ease incident responders in handling raw data.

To parse the provided logs, we need first to convert the EVTX logs into CSV using EvtxEcmd and then feed it into Timeline Explorer.

<div>
<img src="https://github.com/Modern-Wizard/Tempest/blob/main/ss2.png" />
</div>
