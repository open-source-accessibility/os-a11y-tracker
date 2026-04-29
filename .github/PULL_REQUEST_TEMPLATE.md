- [ ] Have you followed the [contributing guidelines](https://github.com/open-source-accessibility/accessibility-toolkit/blob/main/CONTRIBUTING.md)?
- [ ] Have you explained what your changes do, and why they add value to the project?

## Accessibility checklist

Accessibility is a priority for Accessibility Toolkit — please review our [Accessibility Statement](/ACCESSIBILITY.md) and confirm the items below that apply to your change. Check **N/A** for any item that doesn't apply (for example, content-only edits with no UI changes).

### Content changes (any change to articles, README, or docs)
- [ ] Headings follow a logical hierarchy and don't skip levels (`#`, `##`, `###`, …).
- [ ] Link text is unique and descriptive (no "click here" / "read more").
- [ ] Images have meaningful alt text, or are marked decorative when appropriate ([alt Decision Tree](https://www.w3.org/WAI/tutorials/images/decision-tree/)).
- [ ] Complex images and diagrams have a nearby text alternative.
- [ ] Real lists are used instead of manually typed numbering.
- [ ] Plain language is used; abbreviations are expanded on first use.
- [ ] Meaning isn't conveyed by color, position, or styling alone.
- [ ] Any embedded video has captions and a transcript.

### UI / code changes (only if you touched markup, styles, or interactive behavior)
- [ ] Keyboard navigation works end-to-end (everything interactive is reachable and operable without a mouse).
- [ ] Focus states are visible and follow a logical tab order.
- [ ] Forms have associated labels, and error messages are programmatically associated with their fields.
- [ ] Color isn't the only indicator of state, error, or meaning.
- [ ] Reduced motion is respected if animations were added (`prefers-reduced-motion`).
- [ ] Screen reader behavior was checked at least once (VoiceOver, NVDA, JAWS, or TalkBack).
- [ ] Native HTML elements are preferred over custom controls where possible; ARIA is used only when needed.
- [ ] Touch targets are at least **24×24 CSS pixels** with adequate spacing.
- [ ] Tested with an automated tool (e.g. [Axe DevTools](https://www.deque.com/axe/devtools/extension/#:~:text=Try%20Axe%20DevTools%20Extension%20in%20your%20browser%20of%20choice) or the [GitHub Accessibility Scanner](https://github.com/github/accessibility-scanner)) and any new violations are resolved or explained below.

### Notes
<!-- Optional: Describe any accessibility considerations, known limitations, or items intentionally left for follow-up issues. -->

**Please note: we will close your PR without comment if you do not check the boxes above and provide ALL requested information.**

-----

