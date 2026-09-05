# FreeBike

A historical Android student-team project for finding Taipei YouBike stations, checking bike availability, walking to a nearby station, and setting a ride reminder.

**Status: preserved as a historical portfolio artifact. No longer maintained.** This is not a current YouBike client, a supported release, or a recommendation to install an old APK on a personal device. Compatibility with current Android versions and external services has not been tested.

## Background and team recognition

National Taipei University of Education reported that the Free Bike student team, including HuaDi Tsai (蔡華棣), received second place in the **台北生活好便利服務創新應用組** category of the **2012 第十七屆全國大專校院資訊應用服務創新競賽**. This was a team award under faculty supervision, not an individual award.

The university announcement describes using YouBike information to locate rental stations and plan journeys. It does not establish each team member's individual implementation scope. The repository's recorded import is from April 2014; that date is distinct from the 2012 competition, and the archived snapshot has not been verified as the exact competition submission.

University announcement, page 1: https://academicntue.ntue.edu.tw/var/file/2/1002/img/19/165.pdf

## Features visible in the preserved source

- Display bike rental stations using the original station data and map overlays.
- Search for an address and locate a nearby station.
- Request walking directions and draw the returned route. This is not a dedicated cycling route engine.
- Query the historical YouBike site for bike availability.
- Provide a countdown reminder during a ride.

These describe the source snapshot, not a claim that the functions still work against today's services.

## Original technical environment

| Area | Preserved configuration |
|---|---|
| Language | Java |
| Android manifest | minSdkVersion 8, targetSdkVersion 15 |
| Build target | Google APIs 17 in project.properties |
| Project style | Legacy Android/Ant configuration, not a modern Gradle project |
| Maps | Google Maps Android API v1 (com.google.android.maps) |
| Supporting library | Bundled android-support-v4.jar; exact version and notices not verified |

The source includes legacy HTTP integrations, fixed data and response-format assumptions, and old service configuration. Do not reuse the historical configuration or any embedded key strings. This documentation update did not test their validity, rotate keys, scrub Git history, build the application, or run an APK. Repository archival does not remove previously published history.

No current build or installation instructions are promised. Recreating the application today would require a separate modernization effort covering platform APIs, dependencies, service integration, transport security, location permissions, testing, and licensing.

## Preservation and attribution

- The original source and commit history are retained; this update adds documentation only.
- No repository-wide open-source license was found during the review. Do not assume the public repository grants an MIT, Apache, or other license.
- Third-party components retain their respective rights. Their presence does not make them the repository owner's original work.
- Any future rewrite should clearly distinguish the modern implementation from this historical student-team project.