# WCAG 2.2 criterion index

[Knowledge map](../KNOWLEDGE-MAP.md) · [Audit workflow](README.md) · [Sources](sources.md)

The index covers 86 active success criteria across 13 guidelines. The 55 A and AA criteria form the WCAG 2.2 AA baseline. The 31 AAA criteria are listed for projects that evaluate them. The historical entry for 4.1.1 is shown separately in the table as **Removed**.

Each row links to the W3C requirement and its informative explanation. The PANTIK test is a starting point for an audit. Read the requirement, definitions and exceptions before assigning a result.

## 1. Perceivable

### 1.1 Text alternatives

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [1.1.1 Non-text Content](https://www.w3.org/TR/WCAG22/#non-text-content) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/non-text-content.html) | A | 2.0 | Inspect meaningful images, icon-only controls, and decorative images in the accessibility tree. Compare each exposed alternative with the asset's purpose. |

### 1.2 Time-based media

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [1.2.1 Audio-only and Video-only (Prerecorded)](https://www.w3.org/TR/WCAG22/#audio-only-and-video-only-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/audio-only-and-video-only-prerecorded.html) | A | 2.0 | For prerecorded audio-only and silent video, locate equivalent text or an applicable audio alternative. Compare it with the entire source. |
| [1.2.2 Captions (Prerecorded)](https://www.w3.org/TR/WCAG22/#captions-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/captions-prerecorded.html) | A | 2.0 | Play prerecorded synchronized media and compare captions with speech, speaker changes, relevant sounds, and timing. |
| [1.2.3 Audio Description or Media Alternative (Prerecorded)](https://www.w3.org/TR/WCAG22/#audio-description-or-media-alternative-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/audio-description-or-media-alternative-prerecorded.html) | A | 2.0 | Play prerecorded video with the display hidden. Verify that an audio-description track or a media alternative conveys relevant visual events. |
| [1.2.4 Captions (Live)](https://www.w3.org/TR/WCAG22/#captions-live) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/captions-live.html) | AA | 2.0 | Join a live media session and verify captions capture speech and meaningful audio during the event. |
| [1.2.5 Audio Description (Prerecorded)](https://www.w3.org/TR/WCAG22/#audio-description-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/audio-description-prerecorded.html) | AA | 2.0 | Play prerecorded synchronized video and verify that meaningful visual information is conveyed in the audio or an audio-description track. |
| [1.2.6 Sign Language (Prerecorded)](https://www.w3.org/TR/WCAG22/#sign-language-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/sign-language-prerecorded.html) | AAA | 2.0 | Play prerecorded synchronized media and check that a sign-language version covers the audio information. |
| [1.2.7 Extended Audio Description (Prerecorded)](https://www.w3.org/TR/WCAG22/#extended-audio-description-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/extended-audio-description-prerecorded.html) | AAA | 2.0 | Check key visuals in a description track. Where ordinary pauses are too short, verify extended description is available. |
| [1.2.8 Media Alternative (Prerecorded)](https://www.w3.org/TR/WCAG22/#media-alternative-prerecorded) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/media-alternative-prerecorded.html) | AAA | 2.0 | Compare a full media alternative with the prerecorded video and check that it conveys relevant audio, visuals, order, and interactions. |
| [1.2.9 Audio-only (Live)](https://www.w3.org/TR/WCAG22/#audio-only-live) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/audio-only-live.html) | AAA | 2.0 | Follow live audio-only content alongside its accessible alternative and check that the information is equivalent. |

### 1.3 Adaptable content

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [1.3.1 Info and Relationships](https://www.w3.org/TR/WCAG22/#info-and-relationships) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/info-and-relationships.html) | A | 2.0 | Inspect headings, field labels, groups, lists, and table headers in the DOM and accessibility tree. |
| [1.3.2 Meaningful Sequence](https://www.w3.org/TR/WCAG22/#meaningful-sequence) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/meaningful-sequence.html) | A | 2.0 | Compare visual and programmatic reading order for content whose meaning depends on its sequence. |
| [1.3.3 Sensory Characteristics](https://www.w3.org/TR/WCAG22/#sensory-characteristics) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/sensory-characteristics.html) | A | 2.0 | Read instructions without using visual position, shape, color, or sound as a cue. Verify the referenced action can still be identified. |
| [1.3.4 Orientation](https://www.w3.org/TR/WCAG22/#orientation) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/orientation.html) | AA | 2.1 | Rotate a supported device in both directions and verify content and controls work unless one orientation is essential. |
| [1.3.5 Identify Input Purpose](https://www.w3.org/TR/WCAG22/#identify-input-purpose) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/identify-input-purpose.html) | AA | 2.1 | Inspect personal-data inputs against the WCAG input-purpose list and verify appropriate autocomplete semantics where supported. |
| [1.3.6 Identify Purpose](https://www.w3.org/TR/WCAG22/#identify-purpose) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/identify-purpose.html) | AAA | 2.1 | Inspect the programmatic purpose of interface components, icons, and regions in markup. |

### 1.4 Distinguishable content

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [1.4.1 Use of Color](https://www.w3.org/TR/WCAG22/#use-of-color) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/use-of-color.html) | A | 2.0 | Disable color cues or view in grayscale. Check links, errors, charts, and selected states for a second identifying cue. |
| [1.4.2 Audio Control](https://www.w3.org/TR/WCAG22/#audio-control) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/audio-control.html) | A | 2.0 | Load a page with autoplay audio. If playback exceeds three seconds, verify a pause, stop, or independent volume control. |
| [1.4.3 Contrast (Minimum)](https://www.w3.org/TR/WCAG22/#contrast-minimum) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html) | AA | 2.0 | Measure actual text against its rendered backgrounds in each state. Check 4.5:1 for regular text and 3:1 for large text, with listed exceptions. |
| [1.4.4 Resize Text](https://www.w3.org/TR/WCAG22/#resize-text) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/resize-text.html) | AA | 2.0 | Increase text to 200% and check clipping, overlapping controls, missing content, and lost functionality. |
| [1.4.5 Images of Text](https://www.w3.org/TR/WCAG22/#images-of-text) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/images-of-text.html) | AA | 2.0 | Inspect banners and images containing styled text. Verify that text is rendered as text where the technology supports it, subject to exceptions. |
| [1.4.6 Contrast (Enhanced)](https://www.w3.org/TR/WCAG22/#contrast-enhanced) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/contrast-enhanced.html) | AAA | 2.0 | Measure rendered text against its background. Check 7:1 for regular text and 4.5:1 for large text, with listed exceptions. |
| [1.4.7 Low or No Background Audio](https://www.w3.org/TR/WCAG22/#low-or-no-background-audio) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/low-or-no-background-audio.html) | AAA | 2.0 | For eligible speech-first recordings, check for absent, switchable, or sufficiently quiet background audio using the criterion's conditions. |
| [1.4.8 Visual Presentation](https://www.w3.org/TR/WCAG22/#visual-presentation) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/visual-presentation.html) | AAA | 2.0 | For blocks of text, verify users can control colors and meet line length, alignment, spacing, and resizing conditions. |
| [1.4.9 Images of Text (No Exception)](https://www.w3.org/TR/WCAG22/#images-of-text-no-exception) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/images-of-text-no-exception.html) | AAA | 2.0 | Inspect informational images of text. Confirm every example qualifies as purely decorative or essential. |
| [1.4.10 Reflow](https://www.w3.org/TR/WCAG22/#reflow) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/reflow.html) | AA | 2.1 | Test vertically scrolling content at 320 CSS px wide and horizontally scrolling content at 256 CSS px high. Verify content and usage without two-direction scrolling, subject to exceptions. |
| [1.4.11 Non-text Contrast](https://www.w3.org/TR/WCAG22/#non-text-contrast) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html) | AA | 2.1 | Measure visual boundaries, states, and meaningful graphics against adjacent colors. Check 3:1 and record applicable exceptions. |
| [1.4.12 Text Spacing](https://www.w3.org/TR/WCAG22/#text-spacing) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/text-spacing.html) | AA | 2.1 | Apply the WCAG line, paragraph, letter, and word spacing overrides together. Check for loss of content or functionality. |
| [1.4.13 Content on Hover or Focus](https://www.w3.org/TR/WCAG22/#content-on-hover-or-focus) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/content-on-hover-or-focus.html) | AA | 2.1 | Trigger tooltips and popovers using mouse and keyboard. Check dismissal, hover movement into the content, and persistence. |

## 2. Operable

### 2.1 Keyboard access

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [2.1.1 Keyboard](https://www.w3.org/TR/WCAG22/#keyboard) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/keyboard.html) | A | 2.0 | Complete each applicable task using only the keyboard. Record any operation that requires pointer input and evaluate the path-dependent exception. |
| [2.1.2 No Keyboard Trap](https://www.w3.org/TR/WCAG22/#no-keyboard-trap) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/no-keyboard-trap.html) | A | 2.0 | Enter and exit widgets using the keyboard. Check that any nonstandard exit is communicated. |
| [2.1.3 Keyboard (No Exception)](https://www.w3.org/TR/WCAG22/#keyboard-no-exception) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/keyboard-no-exception.html) | AAA | 2.0 | Complete every function using only the keyboard, including flows involving path-dependent pointer interaction. |
| [2.1.4 Character Key Shortcuts](https://www.w3.org/TR/WCAG22/#character-key-shortcuts) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/character-key-shortcuts.html) | A | 2.1 | Find single-character shortcuts and verify they can be disabled, remapped, or work only when the relevant control has focus. |

### 2.2 Timing

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [2.2.1 Timing Adjustable](https://www.w3.org/TR/WCAG22/#timing-adjustable) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/timing-adjustable.html) | A | 2.0 | Trigger each time limit and verify adjustment, deactivation, or extension under the criterion's timing rules. Document exceptions. |
| [2.2.2 Pause, Stop, Hide](https://www.w3.org/TR/WCAG22/#pause-stop-hide) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/pause-stop-hide.html) | A | 2.0 | Check moving content and auto-updating regions shown alongside other content. Test an applicable stop, pause, hide, or frequency control. |
| [2.2.3 No Timing](https://www.w3.org/TR/WCAG22/#no-timing) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/no-timing.html) | AAA | 2.0 | Inventory time-dependent tasks and determine whether each time constraint falls within a listed exception. |
| [2.2.4 Interruptions](https://www.w3.org/TR/WCAG22/#interruptions) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/interruptions.html) | AAA | 2.0 | Trigger interruptions during a flow and verify users can postpone or suppress them, except emergencies. |
| [2.2.5 Re-authenticating](https://www.w3.org/TR/WCAG22/#re-authenticating) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/re-authenticating.html) | AAA | 2.0 | Let a session expire while editing. Reauthenticate and check that entered data and the task remain available. |
| [2.2.6 Timeouts](https://www.w3.org/TR/WCAG22/#timeouts) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/timeouts.html) | AAA | 2.1 | Check inactivity limits that can cause data loss. Verify users are told the duration unless data is preserved for at least 20 hours. |

### 2.3 Flashing and motion

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [2.3.1 Three Flashes or Below Threshold](https://www.w3.org/TR/WCAG22/#three-flashes-or-below-threshold) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/three-flashes-or-below-threshold.html) | A | 2.0 | Review flashing content in each relevant viewport. Use threshold analysis where flash frequency exceeds three in any one second. |
| [2.3.2 Three Flashes](https://www.w3.org/TR/WCAG22/#three-flashes) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/three-flashes.html) | AAA | 2.0 | Check that nothing flashes more than three times during any one-second period. |
| [2.3.3 Animation from Interactions](https://www.w3.org/TR/WCAG22/#animation-from-interactions) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/animation-from-interactions.html) | AAA | 2.1 | Trigger motion through user interaction. Verify disablement for motion that is inessential to functionality or information. |

### 2.4 Navigation and focus

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [2.4.1 Bypass Blocks](https://www.w3.org/TR/WCAG22/#bypass-blocks) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/bypass-blocks.html) | A | 2.0 | Use landmark navigation or a skip mechanism to bypass repeated blocks and reach main content. |
| [2.4.2 Page Titled](https://www.w3.org/TR/WCAG22/#page-titled) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/page-titled.html) | A | 2.0 | Inspect browser titles across routes and verify each identifies the page topic or purpose. |
| [2.4.3 Focus Order](https://www.w3.org/TR/WCAG22/#focus-order) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/focus-order.html) | A | 2.0 | Tab through the interface including menus, dialogs, and return paths. Confirm the sequence preserves meaning and operation. |
| [2.4.4 Link Purpose (In Context)](https://www.w3.org/TR/WCAG22/#link-purpose-in-context) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/link-purpose-in-context.html) | A | 2.0 | Read links with their programmatically available surrounding context. Verify that the destination or action can be identified. |
| [2.4.5 Multiple Ways](https://www.w3.org/TR/WCAG22/#multiple-ways) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/multiple-ways.html) | AA | 2.0 | Find each applicable page through two mechanisms, such as navigation and search. Check the process-page exception. |
| [2.4.6 Headings and Labels](https://www.w3.org/TR/WCAG22/#headings-and-labels) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/headings-and-labels.html) | AA | 2.0 | Read headings and labels apart from body text and verify they describe each section or control. |
| [2.4.7 Focus Visible](https://www.w3.org/TR/WCAG22/#focus-visible) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/focus-visible.html) | AA | 2.0 | Tab through links and controls in each theme and verify an observable keyboard focus indicator. |
| [2.4.8 Location](https://www.w3.org/TR/WCAG22/#location) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/location.html) | AAA | 2.0 | Verify that users can determine their current location within the site or related page set. |
| [2.4.9 Link Purpose (Link Only)](https://www.w3.org/TR/WCAG22/#link-purpose-link-only) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/link-purpose-link-only.html) | AAA | 2.0 | Read links without surrounding context and verify each purpose can be determined, subject to the ambiguity exception. |
| [2.4.10 Section Headings](https://www.w3.org/TR/WCAG22/#section-headings) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/section-headings.html) | AAA | 2.0 | Review long content and confirm that sections use descriptive headings. |
| [2.4.11 Focus Not Obscured (Minimum)](https://www.w3.org/TR/WCAG22/#focus-not-obscured-minimum) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-minimum.html) | AA | 2.2 | Tab through elements near sticky bars, banners, and dialogs. Check that author-created content never hides the focused component entirely. |
| [2.4.12 Focus Not Obscured (Enhanced)](https://www.w3.org/TR/WCAG22/#focus-not-obscured-enhanced) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/focus-not-obscured-enhanced.html) | AAA | 2.2 | Repeat the occlusion test and verify that no part of the focused component is hidden by author-created content. |
| [2.4.13 Focus Appearance](https://www.w3.org/TR/WCAG22/#focus-appearance) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/focus-appearance.html) | AAA | 2.2 | Measure the keyboard focus indicator against the equivalent two-CSS-pixel perimeter area and the 3:1 state-change contrast rule. Check exceptions. |

### 2.5 Pointer and alternative input

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [2.5.1 Pointer Gestures](https://www.w3.org/TR/WCAG22/#pointer-gestures) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/pointer-gestures.html) | A | 2.1 | Test multipoint and path-based gestures using a single pointer without following a path. Document any essential gesture. |
| [2.5.2 Pointer Cancellation](https://www.w3.org/TR/WCAG22/#pointer-cancellation) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/pointer-cancellation.html) | A | 2.1 | Press on a target and release outside it. Verify the action can be avoided, aborted, undone, or reversed as specified. |
| [2.5.3 Label in Name](https://www.w3.org/TR/WCAG22/#label-in-name) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/label-in-name.html) | A | 2.1 | Compare visible text on each control with its computed accessible name. Try speaking the visible label with voice control. |
| [2.5.4 Motion Actuation](https://www.w3.org/TR/WCAG22/#motion-actuation) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/motion-actuation.html) | A | 2.1 | Try motion-triggered actions using normal controls and verify motion response can be disabled, subject to applicable exceptions. |
| [2.5.5 Target Size (Enhanced)](https://www.w3.org/TR/WCAG22/#target-size-enhanced) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/target-size-enhanced.html) | AAA | 2.1 | Measure pointer targets against 44 by 44 CSS px and document any applicable exception. |
| [2.5.6 Concurrent Input Mechanisms](https://www.w3.org/TR/WCAG22/#concurrent-input-mechanisms) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/concurrent-input-mechanisms.html) | AAA | 2.1 | Switch among supported pointer, keyboard, and other inputs while completing the same task. Check any restrictions against exceptions. |
| [2.5.7 Dragging Movements](https://www.w3.org/TR/WCAG22/#dragging-movements) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/dragging-movements.html) | AA | 2.2 | For every drag operation, complete the same task with a single pointer and no dragging. Record essential or user-agent exceptions. |
| [2.5.8 Target Size (Minimum)](https://www.w3.org/TR/WCAG22/#target-size-minimum) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html) | AA | 2.2 | Measure pointer targets against 24 by 24 CSS px. For undersized targets claiming spacing, test the 24 CSS px circle geometry against nearby targets. |

## 3. Understandable

### 3.1 Language and readability

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [3.1.1 Language of Page](https://www.w3.org/TR/WCAG22/#language-of-page) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/language-of-page.html) | A | 2.0 | Inspect the default document language and verify that screen readers pronounce the primary content using the expected language. |
| [3.1.2 Language of Parts](https://www.w3.org/TR/WCAG22/#language-of-parts) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/language-of-parts.html) | AA | 2.0 | Inspect mixed-language passages for programmatic language changes and review the listed exceptions. |
| [3.1.3 Unusual Words](https://www.w3.org/TR/WCAG22/#unusual-words) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/unusual-words.html) | AAA | 2.0 | Locate unusual terms, jargon, and idioms. Verify readers can reach an appropriate definition. |
| [3.1.4 Abbreviations](https://www.w3.org/TR/WCAG22/#abbreviations) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/abbreviations.html) | AAA | 2.0 | Locate abbreviations and verify a mechanism supplies the expansion or meaning. |
| [3.1.5 Reading Level](https://www.w3.org/TR/WCAG22/#reading-level) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/reading-level.html) | AAA | 2.0 | Evaluate difficult text against the reading-level requirement and verify that an accessible simpler version or supplemental content is provided when required. |
| [3.1.6 Pronunciation](https://www.w3.org/TR/WCAG22/#pronunciation) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/pronunciation.html) | AAA | 2.0 | Identify words whose meaning depends on pronunciation and verify a user can obtain that pronunciation. |

### 3.2 Predictable behavior

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [3.2.1 On Focus](https://www.w3.org/TR/WCAG22/#on-focus) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/on-focus.html) | A | 2.0 | Move focus onto interactive controls without activating them and check for unexpected context changes. |
| [3.2.2 On Input](https://www.w3.org/TR/WCAG22/#on-input) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/on-input.html) | A | 2.0 | Change values in selects, toggles, and fields. Confirm that automatic context changes are explained before use. |
| [3.2.3 Consistent Navigation](https://www.w3.org/TR/WCAG22/#consistent-navigation) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/consistent-navigation.html) | AA | 2.0 | Compare repeated navigation across pages in the same set and verify its relative order is consistent unless the user changes it. |
| [3.2.4 Consistent Identification](https://www.w3.org/TR/WCAG22/#consistent-identification) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/consistent-identification.html) | AA | 2.0 | Compare components that perform the same function across pages. Check their visible and programmatic identification. |
| [3.2.5 Change on Request](https://www.w3.org/TR/WCAG22/#change-on-request) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/change-on-request.html) | AAA | 2.0 | Trigger flows that cause context changes and verify they occur on request or can be disabled. |
| [3.2.6 Consistent Help](https://www.w3.org/TR/WCAG22/#consistent-help) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/consistent-help.html) | A | 2.2 | Compare the order of repeated help mechanisms across pages at the same presentation size, accounting for user-initiated changes. |

### 3.3 Input assistance

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [3.3.1 Error Identification](https://www.w3.org/TR/WCAG22/#error-identification) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/error-identification.html) | A | 2.0 | Submit invalid data. Verify the affected field and the specific error are identified in text. |
| [3.3.2 Labels or Instructions](https://www.w3.org/TR/WCAG22/#labels-or-instructions) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/labels-or-instructions.html) | A | 2.0 | Review input controls before submitting. Verify required labels, formats, and other instructions are provided. |
| [3.3.3 Error Suggestion](https://www.w3.org/TR/WCAG22/#error-suggestion) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/error-suggestion.html) | AA | 2.0 | Trigger errors with known corrections. Verify helpful suggestions are available unless they undermine security or purpose. |
| [3.3.4 Error Prevention (Legal, Financial, Data)](https://www.w3.org/TR/WCAG22/#error-prevention-legal-financial-data) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/error-prevention-legal-financial-data.html) | AA | 2.0 | Try a qualifying legal, financial, test, or user-data submission. Check that it can be reversed, corrected after checking, or confirmed before final submission. |
| [3.3.5 Help](https://www.w3.org/TR/WCAG22/#help) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/help.html) | AAA | 2.0 | Look for context-sensitive guidance near inputs or other tasks that require it. |
| [3.3.6 Error Prevention (All)](https://www.w3.org/TR/WCAG22/#error-prevention-all) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/error-prevention-all.html) | AAA | 2.0 | Try a form that submits information and verify reversal, validation with correction, or review and confirmation. |
| [3.3.7 Redundant Entry](https://www.w3.org/TR/WCAG22/#redundant-entry) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/redundant-entry.html) | A | 2.2 | Repeat information within one process. Verify automatic population or selection of the previous entry, subject to the criterion's exceptions. |
| [3.3.8 Accessible Authentication (Minimum)](https://www.w3.org/TR/WCAG22/#accessible-authentication-minimum) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/accessible-authentication-minimum.html) | AA | 2.2 | Test sign-in, MFA, and recovery. Check cognitive test alternatives or assistance, including paste and password-manager support where applicable. |
| [3.3.9 Accessible Authentication (Enhanced)](https://www.w3.org/TR/WCAG22/#accessible-authentication-enhanced) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/accessible-authentication-enhanced.html) | AAA | 2.2 | Test authentication steps requiring memory, transcription, object recognition, or personal content recognition. Verify a qualifying alternative or assistance. |

## 4. Robust

### 4.1 Compatibility with assistive technology

| Criterion | Level | Since | PANTIK test |
| --- | --- | --- | --- |
| [4.1.1 Parsing (Obsolete and removed)](https://www.w3.org/TR/WCAG22/#parsing) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/parsing.html) | Removed | 2.0 | Historical entry. Check the applicable older edition when auditing against WCAG 2.0 or 2.1. |
| [4.1.2 Name, Role, Value](https://www.w3.org/TR/WCAG22/#name-role-value) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html) | A | 2.0 | Inspect computed names, roles, values, and states. Change widget state with assistive technology and verify it is reported. |
| [4.1.3 Status Messages](https://www.w3.org/TR/WCAG22/#status-messages) · [Understanding](https://www.w3.org/WAI/WCAG22/Understanding/status-messages.html) | AA | 2.1 | Trigger search results, confirmations, progress, and errors without moving focus. Verify appropriate announcements to assistive technology. |
