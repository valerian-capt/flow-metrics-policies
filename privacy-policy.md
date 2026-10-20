# Flow Metrics for Jira — Privacy Policy

Effective date: 20 October 2026

Publisher: flowmetrics.expert
Privacy contact: flowmetrics.expert@cadensight.com

Scope: Flow Metrics for Jira, cloud production extension version 0.93.0. Data-handling
changes in later versions require an updated policy.

Flow Metrics for Jira is a browser extension for analysing work flow in Jira
Cloud. In this version, reports are calculated in your browser. The extension
has no Flow Metrics account, backend, telemetry, advertising or AI service.
The profile name “cloud” means that you can connect your own Jira Cloud site;
it does not mean that your reports are uploaded to a Flow Metrics server.

## Information the extension handles

When you connect a Jira site, the extension reads information your existing
Jira account is permitted to access, as needed for the selected boards,
filters and reports:

- Jira site addresses; board, project, workflow, status, filter and swimlane
  configuration; field definitions; and your session display name and timezone.
- Work-item identifiers and keys, creation/update times, statuses, types,
  labels, projects and parent relationships, including parent summaries returned
  with the parent field. Depending on the feature, it additionally requests
  work-item summaries, due dates, sprint membership, estimates,
  versions, relationships and values needed for enabled filters.
- Relevant history, including status, blocker flag, sprint, estimate, parent
  and version changes, and historical assignee display names.
- Current assignee and reporter account identifiers and display names, reduced
  from Jira responses for local filtering. These are handled during work-item
  loading, even if you have not selected a people filter or included people in
  an export. People pickers additionally handle reduced identifiers, display
  names and validated avatar references. People avatar images are loaded only
  from the connected active Jira site; other avatar URLs fall back to initials.
- For blocker-reason reports, comment responses for work items known to have
  blocker flag events. The extension uses comment timestamps and available
  author identifiers to match those events and identify blocker reasons. Other comment text
  is not used in reports or exports; author identifiers are used for matching,
  not displayed as comment authors or retained in the resulting reasons.

The extension does not request work-item descriptions, Jira attachment
contents or worklogs. It does not ask you for passwords or API tokens and does
not read authentication cookie values. Jira may include additional metadata
inside API responses; the extension reduces responses to the values needed
for its features rather than retaining raw user objects or raw responses.

When you click the toolbar icon, Chrome may make the current tab's address
available through `activeTab`. The extension uses it to recognise a Jira Cloud
site and numeric board ID, so it can suggest that site or open that board.
It does not read page content, track navigation or keep general browsing
history. Other URL parts are not kept as browsing records. The toolbar may
also show recently selected boards and load their project icons from their
connected Jira sites.

## How information is used and stored

Information is used to load your chosen scope, filter work items, calculate
metrics, display reports and produce the exports you request. It is not used
for advertising, profiling for unrelated purposes, or training AI models.

Work items, histories, summaries, blocker comments and calculated report data
are held in memory, not saved as an analytics cache. Closing all Flow Metrics
report and print tabs releases those in-memory datasets. The extension does
not keep a server copy or a publication history.

Configuration is stored in `chrome.storage.local` in your Chrome profile.
It includes connected site addresses, recent board identifiers/names and
project icon identifiers, workflow mappings, filters and JQL, selected people
filter identifiers/minimal labels, report preferences, dashboards, team and
calendar definitions, board standards and interface preferences. A saved
cadence-review definition may include its Confluence parent page ID. This is
configuration, not a saved report dataset. Configuration is separated by Jira
site where applicable. The extension does not use Chrome storage sync.

Configuration is retained until removed or replaced, or the extension's local
data is removed. Disconnecting a Jira site removes the saved connection and
requests revocation of its site permission; its board and interface settings
remain available if you reconnect. You can forget individual boards under
Settings → Jira and data. Removing the extension removes its extension-local
configuration; a browser/profile reset may also remove it.

## Network requests and exports

The extension communicates directly over HTTPS with the Jira Cloud sites you
connect. Each analysis uses one active site. Chrome attaches the existing
session credentials to permitted requests; the extension does not extract or
store those credentials. Jira requests include your chosen queries and the
identifiers needed to retrieve the reports. The extension does not edit Jira
work items. Atlassian and your organisation operate those sites and apply
their own access, logging and retention rules.

There is no automatic transmission of Jira content to the publisher, a Flow
Metrics server, analytics providers, AI providers or other third-party services.
Export happens when you choose it:

- PNG pictures, browser print/PDF, CSV files and configuration definitions can
  be saved, copied or handed to the operating system's sharing interface using
  the offered routes. The extension never reads the clipboard. Files, clipboard
  contents and copies you subsequently share are outside its in-memory lifetime.
- If you choose Confluence, the extension checks the selected destination and
  publishes to `/wiki` on the same site as the active Jira. It can attach PNG
  and CSV exports to an existing page, add attachment versions, or create a
  cadence-review page under your chosen parent. There is no scheduled or
  background publication. Recipients are the people who can access the page
  or attachment under your organisation's Confluence permissions.

Exports can contain confidential work information: item keys, links,
summaries, parent summaries, blocker reasons, metrics, scope and measurement
definitions, depending on the chosen report and export. Structured people
fields are excluded by default; include them only by selecting **Include
people** for the applicable export/publication. Known people labels may also
be masked in export text, but this does not guarantee anonymisation of arbitrary
free text in work-item titles, blocker reasons or configuration labels. Unknown
names or other sensitive information can remain. Review the selected content
and destination before exporting.

The cadence-review page body excludes work-item summaries and people fields;
chart/CSV attachments are separate artifacts with their own selected content.
Confluence retains published pages, attachments and versions according to your
site's policies. Closing or uninstalling Flow Metrics does not delete them.
Delete or restrict those copies in Confluence; remove local exported files
and clipboard/shared copies using the relevant application or operating system.
An interrupted upload may already have reached Confluence, and manually retrying
it can create another attachment version.

## Your choices, security and contact

You choose which Jira sites to connect, can deny or revoke site access in
Chrome, and can disconnect sites in Settings → Jira and data. Close report and
print tabs to stop using their in-memory data. Sign out of Jira using Jira's
own controls. Disconnecting the extension does not sign you out of Atlassian.

The extension uses HTTPS, a restrictive content security policy, local
executable resources and validated destinations. It does not provide its own
encryption layer for saved configuration or exported files; protect your
browser profile, device and exported copies using your organisation's controls.

The use of information received from Google APIs will adhere to the Chrome
Web Store User Data Policy, including the Limited Use requirements. More
generally, data handled by the extension is used only for its disclosed
user-facing features; it is not sold, rented, used for advertising or transferred
for creditworthiness or lending decisions.

For questions about this policy, contact flowmetrics.expert@cadensight.com. The publisher
does not receive your Jira dataset through normal extension operation. If you
contact support, share only the information needed for your question and avoid
sending confidential Jira content or credentials. Access or deletion requests
about Jira and Confluence records should also be directed to the administrator
of those services, who controls their stored copies.

Changes to data handling will be reflected in an updated policy and store
disclosures, with permissions or consent requested where required. Planned
accounts, settings sync, licensing, hosted sharing and AI capabilities are not
provided by the version covered by this policy.

## Visiting this policy website

This public policy website is hosted on GitHub Pages, separately from the
Flow Metrics extension. GitHub logs and stores visitors' IP addresses for
security purposes, whether or not they are signed into GitHub. See
[GitHub Pages data collection](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection)
and the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).
This website has no publisher-added analytics, advertising, cookies, forms,
remote fonts or executable JavaScript. Visiting it does not grant access to
your Jira data or connect the extension to GitHub.
