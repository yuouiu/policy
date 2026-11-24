# Terms of Use — cryptobotmonitor

Effective date: November 24, 2026

Operator: Reddit user [u/PsychologicalBug261](https://www.reddit.com/user/PsychologicalBug261/).

Contact: [send the operator a Reddit message](https://www.reddit.com/message/compose/?to=PsychologicalBug261).

## 1. Service

cryptobotmonitor is an independent Reddit Developer Platform application that checks configured public communities, filters posts by keywords and engagement thresholds, and sends notifications to a configured destination. The current deployment uses a Lark custom bot webhook. The application does not execute financial transactions or provide investment recommendations.

Use is limited to communities, actions, purposes and destinations permitted by Reddit and any applicable notification provider. Installing the application in one community does not itself authorize access to every other community. Commercial use or additional data uses require any separate approval that Reddit requires.

The application's data practices are described in its [Privacy Policy](privacy.md).

## 2. Configuration and access

Installation settings must be managed only by authorized community moderators. The developer is responsible for global credentials, application maintenance and the approval of requested external domains. The operator must accurately describe the actual use case to Reddit and must obtain any required permissions before enabling it.

The operator is responsible for choosing the destination, restricting its audience, protecting webhook URLs and signing keys, and ensuring that people receiving notifications are authorized to access that destination. Do not publish credentials or place them in a public source repository.

The current application has no built-in payment or billing feature. Reddit, hosting and notification services are separate services and may have their own terms or charges.

## 3. Permitted use

Use the application for the disclosed monitoring and notification purpose. Do not use it to spam, harass, manipulate votes or engagement, bypass access controls or rate limits, collect private content without permission, identify sensitive personal characteristics, or repurpose data beyond approved uses.

Do not sell Reddit data, redistribute copied content or use it to train AI models without the necessary rights and express approvals. You remain responsible for complying with applicable law, Reddit's terms and policies, the rights of content owners, and the rules of the configured destination.

## 4. Notification content and removal

Lark custom bot mode sends a reference link and fixed notification text rather than copying post titles, bodies, author identities or scores. The original content remains on Reddit. This application cannot automatically recall Lark custom bot messages; local expiry or deletion of tracking records does not remove a chat message. Group owners or administrators are responsible for any necessary manual removal.

Discord and generic modes may send the documented additional post metadata and an optional title. Generic receivers must implement idempotency, deletion and expiry handling and must not recreate content after receiving a deletion event.

The operator must address removal requests, resolve uncertain deliveries and complete appropriate destination cleanup before disabling scheduled tasks or uninstalling the application. Information beyond the operator's control may require action by Reddit, the notification provider or a destination administrator.

## 5. Availability and accuracy

Post scores, comment counts, listings, search results and schedules may be delayed, unavailable or change after a notification. Keyword matching and engagement thresholds do not establish that a post is accurate, safe, useful or endorsed by the operator.

The application is designed for bounded monitoring. It does not promise exhaustive coverage, real-time delivery or exactly-once delivery across independent services. Notifications can be missed or delayed during outages, permission failures, queue limits, observation-window expiry or ambiguous network results. Review the source post before relying on its contents.

The operator may pause, update or discontinue the application when required for maintenance, platform changes, safety or compliance. Reddit may independently restrict or remove access. These terms do not limit any mandatory rights or remedies that cannot lawfully be excluded.

## 6. Third-party services and independence

Reddit, Lark and other configured providers operate independently and apply their own terms and privacy policies. Existing Reddit content belongs to its respective rights holders. This application is not endorsed by Reddit, Lark or the authors of monitored posts.

The application does not require recipients to provide their Reddit passwords, and a notification is not a request to disclose credentials or to take a financial action.

## 7. Changes and support

These terms may be updated as the application changes, with a revised effective date on this page. Contact the operator using the link above for support, questions or removal requests.
