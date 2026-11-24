# PERSONA — A voice, under license

Live website: https://persona-delta-blush.vercel.app/

Independent source repository: https://github.com/JuniceLin/persona (private).

CD490 Project 2: Alignment. A speculative artifact by Haowen Tian and Yihong Lin.

## What is included

Four situations (family, friends, workplace, academic), each with six complete versions: an original reserved/blunt voice, plus Humorous, Gentle, Empathetic, Professional and Polite. Every version has exactly seven exchanges: one utterance by the protagonist and one reply by the counterpart, fourteen messages total. The opening prompt is displayed separately as context and is not counted as an exchange. The artifact contains 336 authored messages.

Conversations are fiction, not recordings or model outputs generated at runtime. They share each scenario's practical decisions and deadlines, while relationship dynamics differ. The original voice is not assigned a lower personality score. The optimized version is not guaranteed a better social outcome.

## Interaction

Select a context. Selecting any persona opens its company policy profile. Inspect Definition, Policy code, Theory & evidence, or Control rights; activate the persona to load the full seven-exchange version. Closing the modal cancels the change. Reopen the current profile with Inspect policy. Replay, Pause, Next exchange and Expand all 7 control presentation; they do not generate or alter messages. The two conversations align exchange heights inside one native scroll viewport. Scrolling over either column moves both; there are no reciprocal JavaScript scroll handlers. The viewport also supports keyboard scrolling. Expand all 7 opens a full-page view.

The profile modal is intentionally company-centered: the visitor chooses a catalogue item, while PERSONA owns the definition, objective, fixed weights and rules. Code is an illustrative, read-only policy specification, not an executing model or a measurement of the visitor. No trait inference, neural data, ratings or psychological assessment runs. All numeric weights are fictional.

The subscription flow includes monthly and annual pricing, four catalogue plans, a permissions comparison, FAQs, organization seats (5–100), itemized order review and an explicit simulation acknowledgment. Selection changes the displayed license and control-rights view in this tab. All five personas remain available for exhibition access. Prices, entitlements, retention windows, administrator powers and contracts belong to the fictional product. No payment, personal billing details, real contract, server log retention or actual organizational surveillance exists.

Export comparison downloads the full pair of transcripts, fixed decisions, profile rules, fictional weights and the research reference as JSON to the visitor's device. No conversation database, local storage, API, model service, account or API key is used.

## Run or package

Serve this directory with any static server; for example `python3 -m http.server 8790`. Open http://127.0.0.1:8790. This is the independent PERSONA repository. Deploy its root to a separate Vercel project; the site does not depend on the personal-website repository.

With Node.js available, run `node build.mjs` to regenerate `data.mjs` from the authored `dialogues.json` and the self-contained `output/PERSONA-offline.html`. The build also copies the five runtime files and the offline HTML into `dist/`, the Vercel output directory. The offline HTML can be opened directly without a server. Google Fonts is an optional network font resource; system fonts are the fallback when offline. Conversation functionality does not depend on a network service.

Run `node --test tests.mjs` to check version counts, seven-exchange lengths, short turns, shared deadline details, references, policy ranges, and absence of an API dependency. These checks do not validate psychological claims; there are no such validated product claims.

## Research and critical framing

- Martin et al. (2003). Individual differences in uses of humor and their relation to psychological well-being: Development of the Humor Styles Questionnaire. https://doi.org/10.1016/S0092-6566(02)00534-2
- Gross & John (2003). Individual differences in two emotion regulation processes: Implications for affect, relationships, and well-being. https://doi.org/10.1037/0022-3514.85.2.348
- Decety & Jackson (2004). The functional architecture of human empathy. https://doi.org/10.1177/1534582304267187
- AHRQ / TeamSTEPPS. Tool: SBAR. https://www.ahrq.gov/teamstepps-program/curriculum/communication/tools/sbar.html
- Brown & Levinson (1987). Politeness: Some Universals in Language Usage. https://doi.org/10.1017/CBO9780511813085

These are real sources, not endorsements. The exhibit explicitly distinguishes what each source discusses from PERSONA's fictional commercial appropriation. Research on humor styles, empathy, emotion regulation, politeness or clinical team communication does not establish that buying a linguistic preset creates a better personality. The company weights and policy hierarchy are an authored critique of governance, not scientific findings.

## Independent Vercel deployment

Import this GitHub repository as an Other framework project. Use Node.js 22+ (24.x is supported), build command `npm run build`, output directory `dist`, and repository root as the Root Directory. No environment variables or API key are needed. Git pushes to `main` trigger Vercel deployment after the repository connection is established. Build output, environment files and local hosting state are ignored by Git.
