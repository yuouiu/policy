# Privacy Policy — cryptobotmonitor

Effective date: November 24, 2026

Operator: Reddit user [u/PsychologicalBug261](https://www.reddit.com/user/PsychologicalBug261/).

Contact for support, privacy questions and removal requests: [send the operator a Reddit message](https://www.reddit.com/message/compose/?to=PsychologicalBug261).

## 1. Scope and purpose

cryptobotmonitor is an independently operated Reddit Developer Platform application. It checks configured public communities for posts that match keywords and engagement thresholds, and sends notifications to an operator-configured destination. Its current deployment uses a Lark custom bot webhook. Use and data access remain subject to Reddit's authorization, review requirements and applicable policies.

This policy describes the application and its static policy pages. It does not replace Reddit's privacy policy or the policies of the notification and hosting providers.

## 2. Information processed

The application processes public post identifiers, community names, post links, creation times, titles, available post text, net scores, comment counts and removal status. Titles and post text are used transiently to evaluate the configured rules. Post bodies are not saved in the application's persistent monitoring state.

Persistent operational records include configured community names and rules, scan checkpoints, candidate post identifiers and timestamps, deduplication markers, notification delivery state, notification receipts, the destination needed to manage an outstanding notification, and recent aggregate status or diagnostic codes.

When a person invokes an administrative menu action, their Reddit account identifier, username and moderator relationship may be processed to verify their permission. These account details are not included in post notifications or saved in the monitoring state.

Webhook URLs and optional signing keys are configured as Devvit secrets. Outstanding notification records may also retain the private destination URL so previously sent notifications can be managed after a destination change. The application's own diagnostics are designed to omit credentials, complete webhook addresses, post bodies and raw provider error messages.

## 3. How information is used

Information is used to find relevant posts, apply keyword and engagement rules, recheck posts that may become relevant later, avoid duplicate notifications, verify administrative access, diagnose failures, and process deletion or notification-expiry work.

The application does not sell monitoring data, build profiles of Reddit users, infer sensitive personal characteristics, or use Reddit content to train AI models. It does not perform trades or financial transactions, vote, post comments, or send private messages to post authors.

## 4. Notifications and recipients

In Lark mode, the application sends an operator-configured safety keyword, fixed notification text and a reference link to the original Reddit post. It does not copy the post title, body, author identity or engagement metrics into that message. A recipient can open the reference link and view the original post through Reddit. Link previews generated independently by a client or provider are outside the application's control.

If Discord or generic webhook modes are enabled, the notification may contain a community name, post identifier, link, creation time, net score, comment count and, only when enabled, the post title. Post bodies and author profiles are not sent. Any additional processing by a generic receiver must be disclosed by its operator.

The operator selects the destination and is responsible for controlling its audience. Messages can be visible to people who have access to that destination. Reddit hosts the application and its operational storage; the configured notification provider processes messages delivered to it. The public policy repository and any static host may process ordinary web-request information under their own policies.

## 5. Retention

Candidate posts are observed for the configured period, currently configurable between 1 and 48 hours after publication. Expired candidate records are removed during subsequent scheduled processing. Deduplication markers are scheduled to expire approximately 50 hours after a post's creation and are removed during subsequent processing.

Notification tracking lasts for the configured period, currently between 1 and 48 hours after delivery, subject to queued cleanup and retries. Records required to resolve delivery uncertainty or failed cleanup may remain until the issue is resolved. Scan checkpoints, configuration and the most recent operational status remain while needed to run the installation, until replaced or removed. Application-level secrets remain until cleared or changed by the operator; uninstalling one community installation does not necessarily clear global secrets.

These periods depend on scheduled tasks running. Pausing new monitoring leaves cleanup enabled, but uninstalling the application, stopping its scheduled tasks or platform outages can delay or prevent processing. The operator should resolve outstanding cleanup before removing an installation.

## 6. Deleted posts and destination limitations

The application periodically checks outstanding notifications for a post's removal or deletion. Supported Discord and generic destinations receive the corresponding deletion action or event. Generic receivers must implement the documented deletion, idempotency and independent expiry behavior.

Lark custom bot messages cannot be automatically recalled by this application. Lark mode therefore sends reference links only. When a tracked post is deleted or its tracking period ends, the application removes local tracking records and reports that any remaining group message requires manual attention. Local cleanup is not deletion of a Lark chat message. A group owner or administrator must perform any necessary chat cleanup.

The operator cannot delete content from Reddit itself, from copies made by other recipients, or from systems outside the operator's control. The operator will review removal requests and take appropriate action within systems they control, including coordinating with destination administrators where necessary.

## 7. Controls and requests

Authorized moderators can configure the application's installation settings, pause monitoring, enable preview mode and select permitted communities and rules. Only an authorized developer can configure global webhook secrets. Installations of the same application share those global secrets.

For access, correction, removal or privacy questions, contact the operator using the Reddit message link above. Include enough information to identify the relevant post or notification. Do not send passwords, webhook tokens, signing keys or other credentials with a request.

## 8. Policy-page analytics and changes

The policy documents themselves include no application analytics scripts, advertising code or tracking cookies. The service hosting or rendering them may apply its own logging, security and cookie practices.

If the application changes its data handling, this policy will be updated with a revised effective date. Questions about a change may be sent to the operator. Reddit's own processing is described in the [Reddit Privacy Policy](https://www.reddit.com/policies/privacy-policy).
