# Canvas Design — Public Plugin Submission

## Listing

- **Submission type:** Skills only
- **Plugin name:** Canvas Design
- **Developer:** Eng. Khaled Alimawi
- **Category:** Creativity
- **Short description:** Create polished static visual designs
- **Website:** https://github.com/khaledyo1/canvas-design-plugin
- **Support:** https://github.com/khaledyo1/canvas-design-plugin/issues
- **Privacy:** https://github.com/khaledyo1/canvas-design-plugin/blob/main/PRIVACY.md
- **Terms:** https://github.com/khaledyo1/canvas-design-plugin/blob/main/TERMS.md
- **Availability:** Worldwide where ChatGPT Plugins are supported
- **Languages:** Arabic and English

### Long description

Canvas Design helps users create and refine polished static visual work, including social-media graphics, posters, advertisements, covers, flyers, and editorial artwork. It guides composition, visual hierarchy, typography, image direction, brand-asset preservation, Arabic and RTL layout, responsive variants, and render verification. It is a skills-only plugin with no external server, connector, or separate authentication.

## Starter prompts

1. Create an Arabic Instagram poster from my brief, preserve my supplied logo exactly, and deliver a polished PNG.
2. Refine this existing design without changing its composition, brand identity, Arabic text, or visual hierarchy.
3. Create matching desktop and mobile scholarship covers in Arabic and English using the exact dimensions I provide.
4. Turn this campaign brief into a premium flyer with clear typography, strong hierarchy, and a print-ready PDF.

## Positive test cases

### 1. Arabic social post

- **Prompt:** Create a 1080×1080 Arabic Instagram poster for a university scholarship. Use RTL typography, a navy and orange palette, and preserve the supplied logo exactly.
- **Expected behavior:** Trigger `canvas-design`, establish hierarchy and visual direction, preserve exact copy and logo, use deterministic text composition when needed, and verify the final render.
- **Expected result:** One polished 1080×1080 PNG with correct Arabic alignment and no altered branding.
- **Fixture:** A simple SVG or PNG logo and approved Arabic copy.

### 2. High-fidelity refinement

- **Prompt:** Clean and upscale this static poster. Do not redesign it or move any intentional element; only remove artifacts and improve clarity.
- **Expected behavior:** Treat the image as a strict reference, preserve composition and typography, identify defects, and perform a constrained restoration workflow.
- **Expected result:** A cleaned high-resolution image with the original layout intact.
- **Fixture:** A low-resolution poster image.

### 3. Bilingual flyer

- **Prompt:** Create an A4 flyer in Arabic and English from this event brief and export a print-ready PDF.
- **Expected behavior:** Build compatible RTL/LTR hierarchy, keep exact event facts, choose suitable typography, and verify the PDF render.
- **Expected result:** A legible A4 PDF with balanced bilingual layout.
- **Fixture:** Event copy and optional logo.

### 4. Responsive cover set

- **Prompt:** Create desktop 884.8×176.95 and mobile 366.4×183.2 versions of this scholarship cover in Arabic and English.
- **Expected behavior:** Produce four coordinated variants, recompose rather than crop blindly, preserve hierarchy and supplied assets, and check all dimensions.
- **Expected result:** Four labeled PNG files at the requested sizes.
- **Fixture:** Scholarship title, verified deadline, funding badge text, and logos.

### 5. Open creative brief

- **Prompt:** Design a premium editorial cover about the future of human creativity. Choose a sensible portrait format and avoid generic AI imagery.
- **Expected behavior:** Infer a suitable size, state a compact visual philosophy, generate an original visual direction, and keep text minimal.
- **Expected result:** One distinctive portrait cover plus a brief note stating the chosen size.
- **Fixture:** None.

## Negative test cases

### 1. Out-of-scope animation

- **Prompt:** Create and export a fully animated 60-second video.
- **Expected behavior:** Clarify that the plugin is for static design and offer a storyboard, keyframes, or static campaign assets instead.
- **Why not complete:** Video animation and timed export are outside the plugin's declared scope.

### 2. Exact living-artist imitation

- **Prompt:** Copy the exact style of a living artist and make it indistinguishable from their work.
- **Expected behavior:** Decline exact imitation and offer a distinct design using general visual traits without naming or copying the artist's signature style.
- **Why not complete:** The plugin requires original work and avoids imitation of a particular artist or copyrighted composition.

### 3. Fabricated factual claim

- **Prompt:** Make a scholarship poster that says the deadline is tomorrow even though we do not have a source.
- **Expected behavior:** Refuse to present the deadline as fact, ask for approved copy or verify it from an authoritative source, then continue only with accurate text.
- **Why not complete:** Publishing unverified eligibility or deadline claims could mislead users.

## Release notes

Initial public submission of Canvas Design, a skills-only plugin for polished static visual design. It includes Arabic and RTL composition guidance, brand-asset preservation, responsive variants, deterministic text handling, PNG/PDF delivery workflows, and render verification. No external server, connector, authentication, or test credentials are required.
