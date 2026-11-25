# 33CRM for Claude

The 33CRM Team is the product team of TriMed 33, the publisher of this integration. Official product and service domain: https://crm.trimed33.com. The GitHub repository is maintained under the Trimed33 organization.

33CRM connects authorized company administrators to business intelligence and operational workflows using their existing CRM account. This plugin includes ten skills that guide Claude through the eligible 33CRM MCP tools, with explanations of data limitations, reporting semantics and secure approval workflows. It is intended for business operations, not clinical decisions or medical advice.

## Connect and get started

Install the plugin in Claude, then connect 33CRM from its Connectors tab and sign in through the first-party OAuth flow. In Claude Code, use the plugin's remote MCP connection. An active 33CRM account, authorized company administrator access, and appropriate permissions are required. No API keys or credentials are bundled. The existing 33CRM connector is referenced by the same remote URL; a second backend is not required.

The server contract supports 61 tools when proposal permissions and features are enabled: 60 read-only operations and one stateful price-change proposal. Actual discovery depends on the connection's scopes, server configuration and eligibility. With read-only access, the underlying read registry contains 58 tools.

## Skills

| Skill | Example request |
| --- | --- |
| Business brief | Summarize our business performance for the last 30 days. |
| Sales and funnel | Where are leads dropping off this month? |
| Record review | Review an eligible non-sensitive deal by its reference. |
| Team operations | Summarize overdue follow-up workload by team. |
| Bookings and conversations | Summarize eligible aggregate attendance and response metrics. |
| Marketing performance | Compare stored Meta and TikTok campaign spend. |
| Attribution and finance | Report eligible revenue and collections by currency. |
| Alerts and data quality | Which operational alerts need attention? |
| Assistant and knowledge readiness | How complete is our approved business knowledge? |
| Knowledge change requests | Propose a new price for an eligible published fixed-price catalog item. |

## Permissions and limitations

The connector reads eligible data through OAuth. A connection with explicit write permission can create a price-change proposal; this does not itself change a catalog price. Review, identity verification, approval or rejection and execution occur in first-party 33CRM. Check the request status before claiming a change was applied. No direct customer messaging, booking changes, campaign launches, payments, document edits or assistant instruction edits are supported by this public bundle.

Do not submit authentication secrets or restricted data to Claude or the MCP. For healthcare, mixed or unclassified data, use only independently eligible business information or qualified aggregate reports; person-level workflows belong in the first-party CRM. Skill guidance is an additional safeguard, not a substitute for server-side controls. Stored provider reports may be delayed or incomplete; honor eligibility, withholding and suppression warnings. Availability depends on the account and connected integrations.

## Resources

- [33CRM](https://crm.trimed33.com)
- [Support](https://crm.trimed33.com/support)
- [Privacy policy](https://crm.trimed33.com/privacy)
- [Terms of service](https://crm.trimed33.com/terms)

This repository contains only the integration bundle, not the 33CRM application, its infrastructure or customer data. The license applies to the bundle files only; the hosted service and its terms remain separate.
