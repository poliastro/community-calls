---
tags: poliastro
---

# poliastro community meetings

- **Time**: Every Friday from 11:00 to 12:00 CE(S)T
- **Platform**: [Jitsi](https://meet.jit.si/poliastro)
- **Goals**: discuss design decisions, triage issues, plan roadmap, write code together it time permits
- **Process**: Write meeting notes here, inserting the most recent one on top. If you want to add specific topics to the agenda, do so before the meeting starts. No need to commit the notes to a wiki or repository for now.
- **Next meeting**: 2021-04-30

## Notes from 2021-04-30

- \[Add any topics here\]

## Notes from 2021-04-23

- NumFOCUS is working to be a Fiscal Host on Open Collective, this might benefit us
  - And perhaps make the transfer of the GSOC money that OpenAstronomy has for us easier?
- @juanlu is working at the moment on the documentation reorganziation, will push soon
- @jorge has almost finished the validation work, we agreed to improve the parametrization of the tests and use Jinja2 to generate the GMAT scripts
    - Turns out we almost completed [what we initially proposed](https://github.com/poliastro/numfocus_proposal/)!
    - We should open issues on poliastro for the problems we identified (lack of intermediate planetary reference frames)
    - Also, we will write a public report and a blog post
- We should review the [long standing animations PR](https://github.com/poliastro/poliastro/pull/1131)
- We need to find a way to simplify the "first contribution", let's speed up the creation of `contrib/`
- @juanlu plans to have everything ready for the beta release by next meeting

## Notes from 2021-04-17

- We had to postpone the meeting one day because of @juanlu schedule
- All GSOC drafts have been reviewed
- We agreed on adding a `contrib/` directory to make contributing rough scripts easier
- [Version 0.15](https://github.com/poliastro/poliastro/issues/1104)
- Ideas for Open Collective:
  - Visible name in main documentation page
  - Mention in release notes
  - "Thank you!" email
  - Fast-track support chat
  - poliastro stickers with a physical "Thank you!" note
- For the frame validation, Orekit uses an older version of the constants, so some tests will be marked as `xfail`
- We will add the GMAT scripts as well as their output, to avoid having to run GMAT in CI
- Validation trigger still not working properly, @jorge will start from scratch

## Notes from 2021-04-09

- Validation repository not being triggered, check token
- @juanlu will catch up with PR reviews and draft reviews
- [Version 0.15](https://github.com/poliastro/poliastro/issues/1104)
- @jorge found new classes in Orekit that might be applicable, will finish validating the frames
- After the GSOC period ends, @juanlu will give a final pass on the [0.15 milestone](https://github.com/poliastro/poliastro/milestone/16), especially on the two coding issues

## Notes from 2021-04-02

- [Rotating frames validation](https://github.com/poliastro/validation/pull/24) (@jorge)
  - We were using the wrong definition of MarsICRS in GMAT (we noticed because the results of MarsFixed were in the same plane, which doesn't make sense) and possibly in Orekit. @jorge will look at it.
- [Libre Space Foundation adherence](https://github.com/poliastro/poliastro/issues/1063) (@juanlu)
  - Not discussed
- [Version 0.15](https://github.com/poliastro/poliastro/issues/1104)
  - Not discussed
- All our meeting was consumed debugging the frames mismatch - for debugging, we should have a separate meeting (that doesn't need to be recurring)
- For next week, @juanlu will review all the pending drafts and catch up with notifications
- @jorge will ask in the Orekit forum about MarsICRS and finish the validation PR
