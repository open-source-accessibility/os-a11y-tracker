# Accessibility Statement

Accessibility is a core priority for **open-source projects**. We want everyone — including people with disabilities and people using assistive technology — to be able to read, navigate, and contribute to this site.

This document explains our accessibility commitment, how contributors can help us uphold it, and how to report accessibility issues.

## Goals

- **Conformance target:** We aim to meet [WCAG 2.2 Level AA](https://www.w3.org/TR/WCAG22) where feasible.
- **Primary priorities:**
  - **Keyboard support** — every interactive element must be reachable and operable with a keyboard alone, with a visible focus indicator and a logical tab order.
  - **Screen reader support** — content uses semantic HTML and a logical heading hierarchy so it can be navigated with VoiceOver, NVDA, JAWS, and similar tools.
  - **Readable content** — we use plain language, descriptive link text, sufficient color contrast, real lists, and meaningful alt text.
  - **Translations** — translated articles declare their language so assistive tech can pronounce them correctly.
- **Known limitations:**
  - Some older articles may not yet meet every guideline (for example, missing alt text or non-descriptive link text). We are working through these as we update content.
  - Embedded third-party content (videos, external images) may not always include captions or transcripts. Please open an issue if you find one.

## Contributor requirements

If you are contributing content or code, please follow these guardrails so we don't regress accessibility:

- **Testing**
  - For UI changes, test with an automated accessibility tool (such as [axe DevTools](https://www.deque.com/axe/devtools/) or the [GitHub Accessibility Scanner](https://github.com/github/accessibility-scanner)).
  - Do at least one keyboard-only pass on any interactive change.
  - Spot-check screen reader behavior for new components or significant content changes.
- **Documentation and content**
  - Use a logical heading hierarchy (do not skip levels).
  - Use unique, descriptive link text (avoid "click here" / "read more").
  - Provide meaningful alt text for images; refer to the [W3C alt Decision Tree](https://www.w3.org/WAI/tutorials/images/decision-tree/).
  - For complex images or diagrams, include a text alternative nearby.
  - For videos, provide captions and a transcript.
  - Don't use color as the only way to convey meaning.
- **CI/CD**
  - PRs may be blocked if they introduce accessibility violations detected by our linting or scanning workflows.
  - Resolve flagged issues, or document why a violation cannot be addressed in the PR description.

## Supported environments

This site is published as static HTML and is intended to work across:

- **Web (desktop):** latest two versions of Chrome, Edge, Firefox, and Safari.
- **Web (mobile):** latest two versions of Mobile Safari and Chrome on Android.
- **Assistive technology:** VoiceOver (macOS / iOS), NVDA (Windows), JAWS (Windows), TalkBack (Android).

Partial-support notes:

- Some translated languages may render with reduced typographic polish in older browsers.
- Embedded third-party widgets are supported on a best-effort basis.

## Reporting accessibility issues

If you run into an accessibility barrier, please let us know — we treat accessibility reports as expertise, not complaints.

1. **Open an issue** using the **accessibility issue template** (or apply the `accessibility` / `a11y` label) at: <https://github.com/github/accessibility-toolkit/issues/new/choose>.
2. Include, when possible:
   - What you were trying to do and what went wrong.
   - The page URL.
   - Your operating system, browser, and assistive technology (with versions).
   - A screen recording or screenshot, if you're comfortable sharing one.
   - Severity, using the [defined taxonomy](#severity).

### Severity

- **Critical:** Prevents you from completing a core task (for example, you cannot read an article at all).
- **High:** Significant difficulty, but a workaround exists.
- **Medium:** Annoyance or inconsistent experience.
- **Low:** Minor issue with minimal impact on usability.

### What to expect

- We will acknowledge accessibility reports as quickly as we can.
- We will be honest about status and timelines (for example, "We're working on this — tracking in #123").
- Where possible, we will suggest a workaround while a fix is in flight.
- We may follow up to confirm a fix works for you before we close the issue.

## Feedback

Accessibility is an ongoing practice, not a one-time fix. If you have suggestions for improving this statement or our practices, please open an issue or a pull request. Thank you for helping make Accessibility Toolkit usable by everyone.
