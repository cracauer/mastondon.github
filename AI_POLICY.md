# AI Contribution Policy

[comments in brackets]

[first paragraph deleted, it didn't say anything. Maybe we want to add
one later]

Today, AI-assisted tools are being deployed in many coding
environments. Some of the "lower-end" features like keyword-driven
code completion can be useful aids; other tools make it very easy to
generate contributions not welcomed by FreeBSD, i.e. without the 
submitter fully understanding how
the code works, or the consequences of specific implementation
choices. These latter forms of AI assistance cause major overhead for
project members.

Our project is fundamentally about authentic human connection and
communication. These values are reflected in our policy towards
AI-generated contributions (below), just as much as they are embodied
in how we work together, and how FreeBSD enables anyone to connect on
the social web.

## 1. Accountability

FreeBSD is a human-to-human project, so even if you've used some
AI-based tools to support your work processes, in the end we expect
contributions to be made by you, the person doing the work.

**The human contributor is the sole party responsible for the contribution.**

If you submit a contribution that includes AI-generated code,
documentation, or comments:

- You must fully understand every line of code in the submission.
- You must be able to explain the "why" behind the implementation
  during the review process. 

"The AI generated it and it works for me" is never an acceptable
answer to a reviewer's question. Copy-and-pasting to and from an AI
chatbot during the process of code review is not acceptable (unless
this is only for translation to and from English). If a maintainer
suspects you do not understand your submission it will not be
accepted.

Autonomous AI agents may not submit submissions to FreeBSD. 
Humans will take time to review the code, and we expect
a human contributor to make the same commitment in handling the
submission themselves. Do not post comments on issues or PRs that are
AI-generated. Discussions on the FreeBSD repositories are for humans
only.

## 2. Disclosure

If AI was used to generate a significant portion of your contribution
(i.e. beyond simple autocomplete), we require you to **disclose it**
in the submission description. Note that you should not use AI to
create the description itself (unless you’ve used it for
translation) - as discussed above, we expect contributions to be submitted by
humans.

Transparency helps maintainers calibrate their review focus. Please
add a trailer to your commit message in the following format:

```text
Assisted-by: Name of AI
```

Examples:

```text
Assisted-by: ChatGPT 5.2
Assisted-by: Claude Opus 4.5
Assisted-by: Google Gemini 3
```

You are encouraged to describe in more detail how and where you used
an LLM (code generation, code review, documentation etc.).

## 3. Intentionality

FreeBSD is a project with code written by humans and interfaces
designed by humans - for everyone. It is not a testing ground for AI
experimentation.

We do not accept contributions and bug reports that result from running an
AI tool over the codebase to find improvements without prior context
or alignment with the project.

- **Focused changes:** Do not submit PRs that perform broad
  refactoring or cleanup suggested by AI unless a maintainer
  specifically requests it. 
- **Design First:** For any non-trivial change, we strongly recommend
  opening a **bug report** or discuss it on the **Mailing Lists**
  first. Contributions that arrive out
  of the blue with significant AI-generated logic that doesn't align
  with our roadmap or architecture will not be accepted. 
- **Quality over Quantity:** We value one thoughtful, manually crafted
  PR over ten AI-assisted fixes for nonexistent or trivial issues. 
- **Size:** As with human-made contributions it is much more likely to be
  accepted if it comes in small chunks. Splitting up large code
  changes is highly encouraged.

Note that these guidelines apply equally to human-created
contributions. Please consider whether the change is meaningful and
wanted by the project before submitting a PR.

## 4. Copyright & Legal

By submitting a contribution to Mastodon, you represent and warrant that:

1. You have the legal right to submit the contribution under the
project's (or specific repository) licence. 
2. The contribution does not violate the intellectual property rights
of any third party. 
3. If AI was used, the resulting code does not violate the terms of
service of the AI provider and does not include "regurgitated" code
from libraries with incompatible licences to the repository you’re
submitting it to. 

If you cannot guarantee the provenance and legal safety of the
AI-generated code, **do not submit it**. 

## 5. Prohibited Uses

The following are strictly prohibited and will result in immediate
rejection of the contribution and potentially a block from the
organisation: 

- **Automated Descriptions:** Using AI to write submission descriptions
  that are vague, overly flowery, or fail to accurately describe the
  technical changes. We want to hear from *you* - the developer -
  why this change matters (see points 1 & 2). 
- **Unvetted Boilerplate:** Submitting large blocks of AI-generated
  boilerplate that hasn't been trimmed to what's actually
  necessary. If you don't understand what the code does, don't submit
  it. 
- **Hallucinated Features:** Submitting PRs for features or bug fixes
  that don't exist, based on AI hallucinations about the project's
  capabilities. 

## 6. Enforcement

The FreeBSD project reserves the right to reject any submission
that appears to be a low-effort AI contribution, without
providing a detailed technical critique. We are a small team
supporting a production project; our time is best spent working with
contributors who understand the project's technical requirements, and
the safety of our users' data.

Cases of repeated violations of these (or any of our other contributor
guidelines) could result in a ban from future submissions.

### Acknowledgement

This policy was written by humans, based on the work in the
[Mastodon AI
Policy](https://github.com/mastodon/.github/blob/main/AI_POLICY.md),
which was based on the [CloudNativePG AI
Policy](https://github.com/cloudnative-pg/governance/blob/main/AI_POLICY.md),
which in turn was inspired by the [Ghostty AI
Policy](https://github.com/ghostty-org/ghostty/blob/main/AI_POLICY.md)
and with acknowledgement to the Linux Foundation's [Generative AI
Policy](https://www.linuxfoundation.org/legal/generative-ai).
