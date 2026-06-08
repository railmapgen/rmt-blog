---
title: Using AI Agents to Speed Up Resource Review for the Rail Map Painter Gallery
date: 2026-06-07 00:00:00
lang: en-US
tags:
  - RMP
  - Gallery
  - AI
---

The Rail Map Painter Gallery keeps growing because of support from every contributor. New cities, new lines, and updated works all make the resource library more complete, and they help more users start drawing from existing templates.

Resource review, however, has always taken a lot of time and attention. A submission cannot be merged just because it looks close enough. It needs to be checked against the official network map, including station names, English spellings, route directions, opening status, and the reliability of reference links. Sometimes several update issues for the same city also need to be reviewed in chronological order. Because maintainer time is limited, many submissions could not be reviewed immediately and gradually became a backlog.

Recently, as AI agents have become more capable, we started using a new way to handle this work. We organized a resource review Standard Operating Procedure for the Rail Map Painter Gallery, and began asking AI agents to assist according to that process: build the same-city queue, collect issues, pull requests, reference links, and updated maps, compare them with official maps, identify verifiable differences, and draft review conclusions and replies.

This does not lower the review standard, and it does not bypass human confirmation. The value of AI agents is that they can carry out repetitive, detailed, and easy-to-miss checks more consistently. Each conclusion should point to a concrete line, section, station name, or reference problem whenever possible. Final actions such as merging, closing, or deleting branches still happen only after explicit confirmation under the Standard Operating Procedure.

Here are the recent statistics for resource submissions reviewed with AI-agent assistance.

![Rail Map Painter Gallery resource review overview](/rmt-blog/images/rmp-gallery-review-2026/rmp-gallery-ai-gent-summary.en-US.png)

The statistics cover May 1, 2026 through June 7, 2026, and include only resource submission issues titled `Resources: New work of <city>` or `Resources: Update work of <city>`. Donation issues are excluded. The issue count represents handled work submissions, while the pull request count represents bot-generated artifacts handled during the process; the two should not be added together.

During this period, 101 resource issues were handled: 74 updates to existing resources and 27 new resource submissions. There were also 112 related resource pull requests, of which 28 were merged and 84 were closed or left unmerged. The pull request count is higher than the issue count because some review chains involve rebuilding bot artifacts, handling duplicate submissions, or closing pull requests after failed reviews.

![Pull request review outcomes](/rmt-blog/images/rmp-gallery-review-2026/rmp-gallery-ai-gent-pull-request-outcomes.en-US.png)

The pull request chart is shown separately because it describes bot-generated artifacts, not additional resource submissions.

![Weekly review volume](/rmt-blog/images/rmp-gallery-review-2026/rmp-gallery-ai-gent-weekly.en-US.png)

Most of the work happened from late May to early June. The busiest week was May 18 to May 24, when 43 resource issues were closed and 51 resource pull requests were handled.

![Issue review outcomes](/rmt-blog/images/rmp-gallery-review-2026/rmp-gallery-ai-gent-issue-outcomes.en-US.png)

Among the 101 resource issues, 28 passed or were merged, 49 required fixes from contributors, 13 were closed because a better version already existed, 5 were duplicate submissions, and a small number had invalid content or invalid format.

“Needs fixing” was the largest outcome group. Looking closer at those issues, most failures came from verifiable detail errors rather than subjective preferences.

![Primary closing reasons for issues needing fixes](/rmt-blog/images/rmp-gallery-review-2026/rmp-gallery-ai-gent-need-fixing-primary-reasons.en-US.png)

When each “needs fixing” issue is assigned one primary closing reason, text-related problems such as station names, English names, and numbering account for the largest share. Common examples include station-name typos, English names that do not match official maps, and incorrect line numbers or legend text.

The second largest category is invalid reference links or reference scopes. Some submissions used unofficial maps, individually maintained pages, or reference links that did not cover the submitted update. For gallery resources, references must be reliable enough to verify whether a work matches official information.

This data also reminds us that the most helpful submission is not simply one that “looks more similar,” but one that clearly explains what changed and uses reliable sources to prove those changes. Details such as station names, English spellings, line numbers, unopened status, and interchange labels are often the points most likely to require fixes.

![Cities with the most review activity](/rmt-blog/images/rmp-gallery-review-2026/rmp-gallery-ai-gent-top-cities.en-US.png)

The cities with concentrated review activity included Chongqing, Guangdong Intercity, Hangzhou, Jinan, Dubai, Kaohsiung, Guangzhou, Jinhua-Yiwu-Dongyang, Shenzhen, and Paris. Some cities received multiple update issues in a short period, making queue-based review especially important to avoid same-city submissions overwriting or duplicating one another.

If you plan to submit a new resource or update an existing one for the Rail Map Painter Gallery, please read the Chinese Standard Operating Procedure first:

[Resource update issue review and handling Standard Operating Procedure](https://github.com/railmapgen/rmp-gallery/blob/main/docs/resources-issue-review-sop-zh.md)

The document explains which resource issues are covered, how same-city queues are handled, which cases can pass, which cases require fixes, when bot artifacts need to be rebuilt, and how review replies and labels are used. Understanding the process can help everyone submit more efficiently and reduce rejections caused by unclear references, station details, or update scopes.

Thank you for supporting the Rail Map Painter Gallery. With a clearer Standard Operating Procedure and assistance from AI agents, we hope the gallery can keep its review quality while clearing the backlog faster and accepting more reliable, high-quality works.

