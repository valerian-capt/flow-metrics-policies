# Flow Metrics for Jira — Privacy Policy

Effective date: 20 October 2026

Reviewed for extension version: 0.93.1 (cloud production)

Last reviewed: 2026-10-20

Publisher: flowmetrics.expert

Contact: flowmetrics.expert@cadensight.com

## What the extension does

Flow Metrics analyses Jira Cloud work in your browser using your existing Jira
session and access rights. This version has no Flow Metrics account, backend,
settings sync, telemetry, advertising or AI service. The “cloud” profile lets
you connect your Jira site; it does not upload reports to our servers.

## Information we process

The extension reads site, board, project, workflow, filter and field settings;
your session display name and timezone; work-item identifiers, summaries,
parent relationships and summaries, dates, types, statuses, labels, estimates,
sprints, versions, relationships, filter values and relevant change history.

Current assignee/reporter identifiers and names are processed during loading,
even without a people filter or export. History can include assignee names.
People pickers use identifiers, names and avatar references; avatar images and
project icons load only from the connected Jira site.

For blocker reports, the extension retrieves comments for work items with
blocker-flag events, matching timestamps and available author identifiers to
identify reasons. Unmatched comment text is not used in reports or exports;
comment authors are not retained with reasons.

We do not request descriptions, attachment contents or worklogs. Responses are
reduced to feature-relevant information. We do not request passwords/API tokens
or read cookie values. On a toolbar click, Chrome's `activeTab` permission
provides the tab address to recognise the Jira site and board ID. We do not
read page content, track navigation or retain general browsing history.

## Use, storage and removal

Data is used for your selected filters, metrics, reports and exports. Jira
work items, histories, comments and report datasets stay in memory; closing all
report and print tabs releases them. We keep no server copy or analytics cache.

Configuration stays in `chrome.storage.local`, without Chrome sync: connected
sites, recent boards/icons, mappings, filters/JQL, selected people's identifiers
and labels, report/dashboard/team/calendar settings, standards, preferences and
saved Confluence parent-page references. Site-specific settings are separated.

Settings remain until replaced or removed. Disconnecting revokes the saved
connection and requests removal of site permission, but retains board/interface
settings. Forget boards in Settings → Jira and data. Uninstalling removes
extension-local settings; browser/profile resets may also remove them.

## Connections, exports and recipients

Requests go directly over HTTPS to your connected Jira sites, one per analysis,
using browser-managed credentials. We do not edit Jira work items or
automatically send Jira content to the publisher, analytics/AI providers or
other external services. Atlassian and your organisation apply their own
access, logging and retention rules.

Only when you choose, PNG, PDF/print, CSV and configuration exports can be
saved, copied or shared through available system controls. We never read the
clipboard. Explicit Confluence publication checks your destination and writes
to `/wiki` on the active Jira site: attachments/versions or a cadence-review
page. There is no scheduled publication. Recipients are people with access
under that site's permissions.

Exports may contain keys, links, summaries, parent summaries, blocker reasons,
metrics and measurement context. Structured people fields are off by default;
**Include people** enables them where offered. Masking does not anonymise
arbitrary titles, reasons or labels. Review content and recipients before sharing.
Cadence-review page bodies exclude summaries/people; attachments have their
own selected content.

Exported files, clipboard/shared copies and Confluence pages/versions outlive
report tabs and uninstalling. Remove them through the relevant service or
application. An interrupted upload may already exist; retrying can add a version.

## Your choices and security

Choose/revoke site access in Chrome or disconnect in Settings. Disconnecting
does not sign you out of Jira. Direct Jira/Confluence access or deletion
requests to your site administrator. Share only necessary support information;
avoid confidential Jira data and credentials.

We use HTTPS, a restrictive content security policy, local executable resources
and validated destinations. We provide no separate encryption layer for saved
settings or exports; protect your browser profile, device and files.

Data is not sold, rented, used for advertising, unrelated profiling, AI training,
or creditworthiness/lending decisions. Information received from Google APIs
is used in accordance with the Chrome Web Store User Data Policy, including
Limited Use requirements.

## This website and policy updates

GitHub Pages hosts this website separately from the extension and logs visitor
IP addresses for security, including signed-out visitors; see the
[GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
We add no analytics, advertising, cookies, forms, remote fonts or JavaScript.
Visiting this page grants no access to Jira.

We review and publish policy metadata for every Chrome Web Store version.
Changed practices require updated disclosures and notice/consent where required.
Contact flowmetrics.expert@cadensight.com with privacy questions.
