# A dev checklist

### If you are using this ...
- Use this at your peril - helps me ensure teams are doing the right things
- Some of these may not be applicable to single developer teams (but in an organisation)
- This is intended to be used continuously and not just at beginning stages (things do change)

## Source Control
- Source control IS being used
- Direct commits to main branch are prevented
- Merges to main branch are done through pull requests
- Pull requests clearly reference associated task
- Commits reference associated task
- Commits are carried out consistently and regularly
- Commit messages are informative
- Prevent failed builds from being merged

## Onboarding
- Must contain a README that details
  - What the project is about
  - Dependencies
  - How to get started
  - Build status
- Someone can build code locally within half a working day of being given access

## Task Management
- Tasks and issues are tracked through JIRA/Azure DevOps/Trello boards
- Boards are well organised (agreed swimlanes, versioned, epic) *
- Backlog is well maintained (regular grooming/management, no lingering tasks)

## Code Reviews
- All code (both application and infrastructure) goes through code review
- Merges should require at least one approval

## Team structure
- More than one developer on team
- Whole team takes responsibility for testing (doesnt matter if dedicated tester, or )

## Testing
- Unit testing coverage across majority of components (% definition to be agreed by team)
- Integration tests that run solution end-to-end (even if via hermetic servers)
- Accessibility test

## Collaboration
- Entire team speaks in the same language (subset of team isnt speaking in another language)
- Everyone is remote, or no one is remote (mixed teams shouldnt have some people in a meeting room and others on Teams/Skype/Zoom)

## CI/CD
- Each pull request triggers CI/CD pipeline
  - Runs CI with automated build and tests
  - Always produces versioned and redeployable artefacts
  - Uses CD to deploy to a non-production environment before pull request is merged

## Security
- Contains logs of threat modelling
- Runs SAST (ideally on PRs if you can apply company rules or manually - mindful of false positives etc)

## Developer environment
- Laptops/Machines are in working condition and fit for job (no exploding batteries)
- Must be able to run docker*
- Must be able to run solution offline (and locally) - contentious one